# Automatisierung von gh-deploy
## Ausgangssituation (IST)
Eine in einem GitHub-Repo gespeicherte MKDocs Webseite wird mithilfe des 'mkdocs.exe gh-deploy'-Befehls in eine GitHub-Pages kompatible Version umgewandelt und auf dem Branch 'gh-pages' hochgeladen. Jedes mal, wenn eine Änderung der Webseite erfolgt, wird der Befehl erneut ausgeführt und so die Webseite auf GitHub-Pages aktualisiert.

## Ziel (SOLL)
Nach jeder Änderung im GitHub-Repository soll die Webseite automatisch aktualisiert werden.

## Umsetzung des Ziels mittels GitHub Actions
1. Lese/Schreib Zugriff für GitHub-Actions Bot erlauben
    1. GitHub Repo > Einstellungen > Actions > Allgemein > Workflow Berechtigungen aus Lese/Schreib Zugriff erlauben
![Lese/Schreibzugriff erlauben](bilder/github-actions-settings-page-rw-permissions.png)
2. Anlegen der Datei .github/workflows/gh-deploy.yml
3. konfigurieren der GitHub-Action:
```
name: gh-deploy 
on:
  push:
    branches:
      - main
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: actions/setup-python@v2
        with:
          python-version: 3.x
      - run: pip install mkdocs-material 
      - run: mkdocs gh-deploy --force
```
4. Änderungen committen und pushen

Die oben erstellte gh-deploy.yml installiert, nach jedem Push auf dem Branch 'main', Python und mkdocs in einer Ubuntu Umgebung. Anschließend führt sie den gh-deploy Befehl aus.

| Linie | Inhalt                                                      | Beschreibung                                                                                                                              |
|-------|-------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|
| 2-5   | on:  push:     branches:       - main                       | Auführung bei Push auf 'main'-Branch                                                                                                      |
| 10-11 | - uses: actions/checkout@v2 - uses: actions/setup-python@v2 | Führt von GitHub vordefinierte Befehle aus: - checkout: macht das Repository für die Action verwendbar - setup-python: installiere Python |
| 12    | with:   python-version: 3.x                                 | benutze/installiere Python Version 3 im 'setup-python' Befehl                                                                             |
| 13    | - run: pip install mkdocs-material                          | installiere das pip(Python) modul 'mkdocs-material'                                                                                       |
| 14    | - run: mkdocs gh-deploy --force                             | führe den 'mkdocs gh-deploy'-Befehl aus                                                                                                   |
