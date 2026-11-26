# Versionsverlauf

Übernommen aus dem Updatelog des Programms (Stand Version 3.6).

## v3.6 (2026-11-04)

- Neu (nur Classic): NACHTWACHE (F9) - holt in einstellbaren Zyklen fertige Verkäufe ab (rote Box, max. 44), erstellt Buy-Orders und verkauft die Items neu; bei Preis 0 wird der Average Price aus der 4-Wochen-History eingetragen
- Texterkennung über Windows-OCR (ocr.ps1), Bilder werden nach jedem Zyklus gelöscht
- Kalibrierung: drei optionale Schritte für die Nachtwache (Completed Transactions, Verkaufsfenster mit aus- und eingeklappter History) mit anonymisierten Beispielbildern

## v3.0 (2026-11-04)

- Komplett neu in Python: Launcher mit Moduswahl (Classic und Python-Variante), alle Kauf-/Verkauf-/Kreislauf-/Post-Routinen, Statistik, Preis-Tracker und Kalibrierung portiert
- Lizenz und Version werden vom Launcher geprüft; das Programm startet nur über den Launcher
- Umhänge: Scroll-Stand wird beim Kauf per Screenshot nachgemessen und korrigiert

## v2.9 (2026-11-03)

- Neu: Taschen (Bag / Satchel of Insight, einzeln oder beide in einem Durchlauf) und Umhänge (15 Stück ab T4) im Kauf-Makro
- Umhänge: Scrollen per Klick auf die Scrollleiste statt Ziehen; Kalibrierung per Screenshot (Button im Umhänge-Feld), gespeichert in den Einstellungen
- Kalibrierung: Marktansicht + graue Bestätigungsbox (+ Postfach optional); Auflösung = echter Bildschirm

## v2.8 (2026-11-03)

- Launcher: Lizenz-Login mit Geräte-ID (kopierbar), gespeicherter Schlüssel wird bei jedem Start geprüft
- Starten-Button: ist eine neuere Version veroeffentlicht, wird sie automatisch geladen, geprüft und installiert; die alte Version wird gelöscht
- Kalibrierung über Screenshots (Auflösung + UI-Skalierung); die manuelle Auflösungs-Auswahl entfällt
- Post-Wöhler nutzt die Skalierung aus dem Postfach-Screenshot

## v2.7 (2026-11-01)

- Auto-Update über GitHub: beim Start wird nach einer neuen Version gesucht, Download mit Prüfsumme, Austausch und Neustart
- Pflicht-Updates möglich (min_version): aeltere Versionen starten dann erst nach dem Update
- Lizenz und Version werden vor jeder Aktion (F1, F6, F7, F8) online geprüft

## v2.6 (2026-11-01)

- Online-Lizenzprüfung: Freischaltung wird regelmäßig mit einer Liste im Internet abgeglichen (Widerruf jederzeit möglich)
- Ohne Internet läuft das Programm bis zu 48 Stunden nach der letzten erfolgreichen Prüfung weiter

## v2.5 (2026-11-01)

- Oberfläche bei Windows-Skalierung über 100% korrigiert (Hintergrund und Elemente waren verschoben)

## v2.4 (2026-10-09)

- 2560x1440 korrigiert: Faktor 1.789 (proportional zur Höhe) statt 1.44, Klicks lagen daneben

## v2.3 (2026-10-03)

- 1920x1080 korrigiert: Faktor 1.342 aus deinen Skripten gemessen (war 1.08, Klicks lagen daneben)
- Einstellungen: SAT-Ordner wählbar (Suchen-Knopf), leer = automatisch suchen

## v2.2 (2026-10-02)

- Einstellungen: Eingabefelder mit dunkler Schrift auf hellem Feld (waren unleserlich)

## v2.1 (2026-10-02)

- Revierkarte: neue Spalte Saldo (Umsatz minus Ausgegeben = reiner Gewinn)
- Erlös (netto) heisst jetzt Umsatz (Markt-, Tages-Liste, Chroniken, Zusammenfassung)
- Neuer Tab Beute-Charts: alle Items nach Tier und Verzauberung, meistgekauft zuerst
- Gewinn-Ranking: Umsatz minus Kaufpreis der verkauften Stück, nur Items mit Kaufpreis
- Zeilen löschen: Wühlkasse/Chroniken endgültig, Revierkarte/Charts ausblenden
- Rechtsklick auf die Liste: Auswahl löschen oder Ausgeblendetes wiederherstellen
- Export/Import aller Statistiken in eine Textdatei (Läufe, Mails, Ausgeblendetes)
- Mail-Archiv stats_archive.csv: Statistik bleibt, auch wenn SAT seine Daten leert

## v2.0 (2026-10-02)

- Post-Wühler klickt eine der unteren Mails (Zeile 7) statt der ersten, schneller

## v1.9 (2026-10-02)

- Updatelog-Tab in der Statistik (diese Liste, Datei updatelog.txt)
- Revierkarte: Markt per Doppelklick wählen, dann alle Tage dieses Marktes einzeln

## v1.8 (2026-10-02)

- POST-WUEHLER (F8): Mail anklicken, dann Delete, in Schleife
- Einstellungen (F4): Post-Pause pro Klick (ms) und Post-Durchläufe (0 = endlos)
- Dritte Taste im Kasten Waschbär Beutezug (Verscherbeln, Kreislauf, Post-Wühler)

## v1.7 (2026-10-01)

- Statistics Analysis Tool (SAT) angebunden: Trades.json und Market.json
- Revierkarte aus den Spiel-Mails: Käufe, Ausgaben, Verkäufe, Erlös, Unerfüllt
- Erlös (Sofortverkauf, netto) in Verscherbel-Chronik und Kreislauf-Kapriolen
- SAT-Ordner wird automatisch gefunden; Portal-Städte und Dens zählen zum Stadtmarkt
- Preise nach Kauf-Läufen zuerst aus SAT Market.json, dann Data Project

## v1.6 (2026-10-01)

- Preis-Tracker: Kaufstadt im Hauptfenster wählen (Klick = nächste Stadt)
- Nach jedem Kauf-Lauf: höchste Buy-Order-Preise holen und Silbersumme berechnen
- Statistik mit vier Tabs: Wühlkasse, Verscherbel-Chronik, Kreislauf-Kapriolen, Revierkarte
- Spalten: Operation, Stadt, Dauer, Tempo (Items/min), Items, Silber

## v1.5

- Hotkeys als Umschalter: F6 und F7 starten/stoppen, F2 Pause/Fortsetzen, F3 Stopp

## v1.4

- Waffenreihenfolge wie im Spielmenü (Bogen bis Gestaltwandlerstab)
- Kaufskript-Option aus dem Hauptfenster entfernt
- Dunkles Auflösungs-Dropdown in den Einstellungen mit weiteren Auflösungen

## v1.3

- Design Waschbär Schnapper: dunkles Theme, orange Akzente, Waschbär-Logo
- GUI als Bild-Overlay (bg_*.png, layout_*.txt, chk_on/off.png)

## v1.2

- Zwei Verkaufs-Modi aus Sell.ahk und Re_Sell.ahk:
- BEUTE VERSCHERBELN (F6) und SCHNAPP-KREISLAUF (F7), Durchläufe einstellbar

## v1.1

- Statistik (F5): Session-Verlauf mit Datum, Items und Dauer, nach Neustart erhalten
- Geschätzte Laufzeit vor dem Start aus gemessenen Zeiten der gewählten Items

## v1.0

- Grundversion Buy-Order-Automator (swag.ahk): Kategorien, Tiers, Verzauberungen
