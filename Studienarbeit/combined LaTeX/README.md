# Template für die DHBW

## Literaturverwaltung
- Allgemein
    - sehr wichtig zu verwenden
    - Autoimport von Quellen immer direkt am Anfang auf Richtigkeit überprüfen
    - am besten vorher informieren, was das beste Produkte ist, da ein Umstieg während einer Arbeit nicht mehr möglich ist
- Produkte
    - Citavi
        - Webversion ist extrem langsam -> Desktop-Client nutzen (idealerweise mit lokalem Projekt)
    - [Zotero & Obsidian](https://www.marianamontes.me/post/obsidian-and-zotero/)

## OnePager.tex

[Beispiel](/OnePager-example.pdf)

Ist eher für Bachelor-/Masterarbeiten interessant.
Der OnePager wird vor der Arbeit verfasst, um sich etwas mit dem Thema zu beschäftigen.
Es sollte eine Themeneinführung mit Motivation und groben Projektplan enthalten.

## Main.tex

[Beispiel](/main-example.pdf)


Das ist ein Template für die wissenschaftliche Arbeit (nach DHBW Vorschrift), das folgendes enthält:

- Titelseite
- Eidesstattliche Erklärung
- Inhaltsverzeichnis
    - 2x Latex kompilieren, damit es korrekt aktualisert wird
- Anleitung mit Copy-Paste Snippets
    - vor der Abgabe löschen :D
    - enthält z.B.: Tabellen/Bilder/Formeln/Zitate
- Kapitelstruktur
    - Standardstruktur für wissenschaftliche Texte
    - falls deine sehr stark abweicht, schreibst du eventuell keinen wissenschaftlichen Text
- Abbildungs-, Formel- und Tabellenverzeichnis
    - falls leer muss es manuell gelöscht werden
    - es existieren immer Beispiel im Anleitungsteil
- Literaturverzeichnis

## Wie nutze ich das Template für mein Projekt?
- oben rechts neben dem Namen auf den Button fork klicken
- Name + Namespace auswählen und entsprechend Repository generieren lassen
- dadurch existiert sogar ein GitLab Banner mit Forked aus :D

## Wie kriege ich aktuelle Änderungen aus dem Template in mein Repository?

Voraussetzung: dein Repo muss ein Klon vom Template sein (also z.B. über diese Anleitung erstellt sein)


1. Rebase erlauben
    - Variante 1: "Push-Force"
        - Links in der Leiste auf Settings/Repository gehen
        - zu Protected Branches navigieren
        - das Recht für Push-Force im Main-Branch erlauben 
        - wichtig, damit du später Rebase auf dem Master durchführen kannst
    - Variante 2: "anderer Branch"
        - erstelle einen neuen Branch (Name ist egal)
        - der Branch darf nicht Push-Force protected sein!
        - main-branch: zuständig um immer den aktuellen Stand aus dem Template zu haben
        - dein-branch: alle deine Änderungen für deine Arbeit
2. Template mit deinem Repository verbinden (alle Befehle lokal im Terminal ausführen)
    - ```git remote add upstream git@gitlab.cas.de:youth-league/templates/dhbw.git``` 
    - ```git pull upstream``` 
    - ```git checkout master```
    - ```git rebase upstream/master```
        - am besten mit Tool machen und nicht über Command-Line für eventuelle Konflikte
    - ```git push --force```
        - muss mit Force-Flag geschehen, da sich durch den Rebase die Commit-Hashes ändern
