# Github-Repository in Visual Studio klonen

## Ausgangspunkt (IST)
Im Repository befindet sich eine ZIP-Datei mit dem zugehörigen Projekt "handelskalkulation", geführt unter dem Ordner Projekte &rarr; Schulung Github
![Handelskalkulation](Projekte/Schulung%20Github.zip)

## Ziel (Soll)
Ziel ist es jetzt dafür zu sorgen, dass das Projekt sowohl in Github implementiert wird, als auch das Änderungen automatisch übernommen werden.

## Vorgehensweise
Gegebenenfalls muss zuerst der Proxy neu eingestellt werden: git config --global http.proxy http://kjs-04.lan.dd-schulen.de:3128
![Proxy einstellen](bilder/Proxy%20einstellen.png)

1. neues Repository auf GitHub erstellen
</br>
2. lokalen Speicherort wählen und Repository klonen
</br>
3. C#-Projekt in lokalem Repository speichern/einfügen
</br>
4. "git add ." alle Änderungen hinzufügen und danach "git commit" alles bestätigen
</br>
5. Commit-Nachricht hinzufügen
</br>
6. Repository auf GitHub pushen
</br>
7. Visual Studio öffnen (die Normale, nicht die lokale Version)
</br>
8. "Repository klonen" auswählen und Link von GitHub-Repo einfügen
![Repository in von Github in VS klonen](bilder/Repository%20klonen.png)
</br>
9. in geöffnetem Code eine Änderung zum Test vornehmen
</br>
10. alles hinzufügen (add), Nachricht eingeben (commit) und commit ausführen
![alle Änderungen hinzufügen](bilder/alle%20%C3%84nderungen%20adden.png)
![commit message und commit ausführen](bilder/commit%20message%20%2B%20commit.png)
</br>
11. push ausführen um Änderung auf Github Repository zu übertragen (erneute Authentifizierung)
</br>
![pushen](bilder/push%20(github).png)
![authentifizieren](bilder/mit%20Accountdaten%20verifizieren.png)
