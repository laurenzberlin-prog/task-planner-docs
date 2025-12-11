Der  Task Planner ist eine  Webanwendung mit der Nutzer
ihre Aufgaben für die kommende Woche planen können. Statt eine klassische
To-do-Liste zu verwenden, wird ein Punktesystem eingesetzt:
Pro Woche steht ein begrenztes Punktekonto zur Verfügung, bisher 100 Punkte.
Jede Aufgabe bekommt eine bestimmte Anzahl an Punkten, abhängig von
Wichtigkeit und erwartetem Zeitaufwand. Durch den Vergleich von vergebenen vs. erledigten Punkten soll der eigene Fortschritt sichtbar werden.
Ziel ist es, Prioritäten bewusster zu setzen und eine realistische Wochenplanung
zu unterstützen.

Aktueller Stand der Implementierung

Momentan besteht eine grundlegenden Struktur:
Wir haben eine Flask-App mit definierten URL-Routen, ein Basis-Templates für die wichtigsten Screens

Was noch geplant ist, sind das Speichern von Aufgaben, Verteilung der Punkte über mehrere Tage und die Fortschrittsberechnung auf Basis echter Daten



Aktuelles Datenmodell:
erDiagram
    TASK {
        int id
        string title
        string description
        int points_total
        int points_done
        string weekday
        string status
