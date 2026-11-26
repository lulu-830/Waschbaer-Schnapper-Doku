# Kalibrierung

Damit die Klicks an den richtigen Stellen landen, muss das Programm die **Auflösung** und die **UI-Skalierung** des Spiels kennen. Statt sie von Hand zu wählen, misst es sie aus Screenshots.

## Ablauf

1. In den Einstellungen auf **Kalibrieren** klicken.
2. Der Assistent bittet der Reihe nach um Bildschirmfotos aus dem Spiel:
   - **Marktansicht** (Pflicht)
   - **Graue Bestätigungsbox** (Pflicht)
   - **Postfach** (optional, für den Post-Wühler)
   - **Umhänge-Scrollleiste** (eigener Button im Umhänge-Feld)
   - **Nachtwache** (optional, nur Classic): Completed Transactions sowie das Verkaufsfenster mit aus- und eingeklappter Historie
3. Das Programm vergleicht die Bilder mit mitgelieferten Beispielen und berechnet daraus Auflösung und Skalierung.
4. Das Ergebnis steht in den Einstellungen und gilt für alle Läufe.

Die Auflösung ist die **echte Bildschirmauflösung**, nicht die Spielauflösung.

## Beispielbilder

Zu jedem Schritt gibt es ein anonymisiertes Beispielbild, damit man weiß, welcher Bildschirmausschnitt gemeint ist. Die Messung selbst übernimmt in der Python-Version eine Bildanalyse mit numpy.

## Wann neu kalibrieren

- nach einer Änderung der Bildschirmauflösung
- nach einer Änderung der Windows-Skalierung
- nach einem Wechsel des Spiel-UI-Maßstabs
- wenn Klicks erkennbar danebenliegen
