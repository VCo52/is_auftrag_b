# Kalenderwoche 38
!!! note "Gruppeneinteilung Projekte"

    * Die Gruppeneinteilung wird selbst vorgenommen .. jeweils 4 Schüler.
    * Die drei Themen werden unter den Gruppen aufgeteilt.

!!! note "Gruppen nutzen einen gemeinsamen GitHub-Account für Dokumentation"

    * Erstellung eines Mkdocs-Gerüstes für die Projektdokumentation ... Wiki-Charakter!
    * Jede Gruppe besitzt **einen gemeinsamen** Github-Account für die Dokumentation. Alle Dinge zum Projekt werden hier gespeichert. 
        * Alle Gruppenmitglieder haben Zugriff auf den Account durchgeführt und haben das Passwort (Schlüssel) für ihren Account sicher verwahrt.
        * Die Dokumentation wird über gh-pages als Webseite bereitgestellt.  

!!! note "Continous Deployment mit GitHub"

    Die Mkdocs-Dokumentation soll automatisiert in eine Webseite umgesetzt werden.

    * Diese soll von beliebigen Rechnern mit Windows oder Linux erfolgen können. Ein Git-Client wird als vorhanden angenommen.
    * Auf dem Rechner ist keine Mkdocs-Installation verfügbar.
    * Die Dokumentation ändern Sie mit einem vorhandenen Editor bzw. Dateimanager.
    * Nutzen Sie eine GitHub-Action (Continuous Deployment), um die Mkdocs-Dokumentation als gh-pages-Webseite automatisiert erstellen zu lassen.

!!! note "Anbinden von Visual-Studio-Projekten an GitHub"

    * Sie nutzen das Visual-Studio-Plugin, um C#-Projekte mit einem git-Repository abzugleichen.

!!! Nutzwertanalyse für im Rahmen des Projektes erstellen

    Für das Projekt sind aktuelle Werkzeuge für das automatisierte Bereitstellen von Diensten hinsichtlich der Auswahlkriterien in einer Nutzwertanalyse zu vergleichen. Beispielhaft sind hier Werzeuge wie Docker, Ansible, Vagrant, GitHub, GitLab, Kubernetes, Openshift, OPNsense, IPfire, Google Cloud, Azure genannt. 

!!! note "Vorbereitung Schulung der Gruppe Anwendungsentwickler"

    Am 28.09. werden Sie einen Workshop (Kundenschulung) der Gruppe Anwendungsentwickler im Raum B3 vornehmen. Die Schulung erfolgt in drei Modulen. Jede Gruppe ist für die Vorbereitung eines Moduls zuständig. Bereiten Sie die Schulung so vor, dass diese den Charakter einer Kundenschulung besitzt.
    Die Schulung umfasst dabei 180 Minuten. Die Verteilung der Zeitfenster zwischen den Gruppen kann abgestimmt werden.

    Organisatorischer Ablauf:

    * Pro Modul wird die verantwortliche Gruppe in einen oder zwei Moderatoren (Vortrag, Präsentation) und zwei/drei Assistenten aufgeteilt. Die Assistenten stellen während des Moduls sicher, dass die Schulungsteilnehmer rasch mitkommen. Die Mitglieder der anderen Gruppe werden zur Partnerarbeit mit je einem Anwendungsentwickler eingeteilt.
    * Folgende drei Module sind abzudecken:
        * Einführung in Mkdocs, PortableApps, Visual-Studio-Code - **Ziel:** Alle Teilnehmer haben im Anschluss eine PortableApps-Version zum Starten von Mkdocs, eine eigene Vorlage für eine Mkdocs-Dokumentation und eine Übersicht über den Workflow. 
            * Dateistruktur Mkdocs vorstellen
            * Workflow erklären
            * Komponenten von Mkdocs vorstellen und gleichzeitig durch Teilnehmer mit erstellen lassen
            * Eigene portable Software in PortableApps integrieren
            * VisualStudio-Code kurz mit Extensions vorstellen
        * GitHub-Einführung und gh-Pages - **Ziel:** Alle Teilnehmer haben im Anschluss einen GitHub-Account, ihre Mkdocs-Dokumentation ins Repository eingepflegt und wieder aus dem Remote-Repository gezogen. Ebenso liegt die Mkdocs-Dokumentation als gh-pages-Webseite vor. 
            * Account anlegen
            * Remote-Repository anlegen
            * git-Kommandos auf der Kommandozeile vorstellen
            * Abgleich mit Local-Repository
            * Mkdocs-Vorlage in Remote-Repository                
        * GitHub-Nutzung mit Continuous-Deployment und Beispielprojekt in C# - **Ziel:** Jeder Teilnehmer integriert das Continous Deployment in GitHub und integriert ein C#-Projekt in GitHub mit Hilfe von Visual Studio.
            * GitHub-Action vorstellen
            * Mkdocs-Dokumentation automatisiert erstellen
            * C#-Projekt kurz vorstellen
            * C#-Projekt als GitHub-Repository
