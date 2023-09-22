# Github-Repository in Visual Studio klonen

## Ausgangspunkt (IST)
Im Laufwerk "Projekte" befindet sich der Projektordner "Handelskalkulation zum dazugehörigen Code als ZIP-Datei.

## Ziel (Soll)
Ziel ist es jetzt dafür zu sorgen, dass das Projekt sowohl in Github implementiert wird, als auch das Änderungen automatisch übernommen werden.

## Vorgehensweise
Gegebenenfalls muss zuerst der Proxy neu eingestellt werden: git config --global http.proxy http://kjs-04.lan.dd-schulen.de:3128
![Proxy einstellen](Proxy einstellen.png)

1. neues Repository auf GitHub erstellen
2. lokalen Speicherort wählen und Repository klonen
4. C#-Projekt in lokalem Repository speichern/einfügen
6. "git add ." alle Änderungen hinzufügen und danach "git commit" alles bestätigen
7. Commit-Nachricht hinzufügen
8. Repository auf GitHub pushen
9. Visual Studio öffnen (die Normale, nicht die lokale Version)
10. "Repository klonen" auswählen und Link von GitHub-Repo einfügen
![Repository in von Github in VS klonen](Repository klonen.png)
11. in geöffnetem Code eine Änderung zum Test vornehmen
12. alles hinzufügen (add), Nachricht eingeben (commit) und commit ausführen
![alle Änderungen hinzufügen](alle Änderungen adden.png)
![commit message und commit ausführen](commit message + commit.png)
13. push ausführen um Änderung auf Github Repository zu übertragen (erneute Authentifizierung)
![pushen](push (github).png)
![authentifizieren](mit Accountdaten verifizieren.png)
