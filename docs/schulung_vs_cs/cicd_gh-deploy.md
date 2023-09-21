# Automatisierung von gh-deploy
## Ausgangssituation (IST)
Eine in einem GitHub-Repo gespeicherte MKDocs Webseite wird mithilfe des 'mkdocs.exe gh-deploy'-Befehls in eine GitHub-Pages kompatible Version umgewandelt und auf dem Branch 'gh-pages' hochgeladen. Jedes mal, wenn eine Änderung der Webseite erfolgt, wird der Befehl erneut ausgeführt und so die Webseite auf GitHub-Pages aktualisiert.

## Ziel (SOLL)
Nach jeder Änderung im GitHub-Repository soll die Webseite automatisch aktualisiert werden.

## Einführung in GitHub-Actions
Die GitHub-Actions sind eine Methode von GitHub um 