# Github-Repository in Visual Studio klonen

## Ausgangspunkt (IST)
Im Laufwerk "Projekte" befindet sich der Projektordner "Handelskalkulation zum dazugehörigen Code als ZIP-Datei.

## Ziel (Soll)
Ziel ist es jetzt dafür zu sorgen, dass das Projekt sowohl in Github implementiert wird, als auch das Änderungen automatisch übernommen werden.

## Vorgehensweise
Gegebenenfalls muss zuerst der Proxy neu eingestellt werden: git config --global http.proxy http://kjs-04.lan.dd-schulen.de:3128
![Proxy einstellen](bilder/Proxy%20einstellen.png)

1. neues Repository auf GitHub erstellen
2. lokalen Speicherort wählen und Repository klonen
4. C#-Projekt in lokalem Repository speichern/einfügen
6. "git add ." alle Änderungen hinzufügen und danach "git commit" alles bestätigen
7. Commit-Nachricht hinzufügen
8. Repository auf GitHub pushen
9. Visual Studio öffnen (die Normale, nicht die lokale Version)
10. "Repository klonen" auswählen und Link von GitHub-Repo einfügen
![Repository in von Github in VS klonen](bilder/Repository%20klonen.png)
11. in geöffnetem Code eine Änderung zum Test vornehmen
12. alles hinzufügen (add), Nachricht eingeben (commit) und commit ausführen
![alle Änderungen hinzufügen](bilder/alle%20%C3%84nderungen%20adden.png)
![commit message und commit ausführen](bilder/commit%20message%20%2B%20commit.png)
13. push ausführen um Änderung auf Github Repository zu übertragen (erneute Authentifizierung)
![pushen](bilder/push%20(github).png)
![authentifizieren](bilder/mit%20Accountdaten%20verifizieren.png)
