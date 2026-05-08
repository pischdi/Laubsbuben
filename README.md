# Steel Dart Zähler

Eigenständiger Browser-Zähler für Steel Dart (X01) — eine einzige `index.html`,
keine Build-Tools, keine externen Abhängigkeiten.

## Features

- **Spielmodi**: 301 / 501 / 701, Single-Out / Double-Out / Master-Out
- **Anklickbare SVG-Dartscheibe** mit allen Single-/Double-/Triple-Feldern,
  Bull (25) und Bullseye (50)
- **Match-Modus** „First to N Legs" mit rotierendem Anwurf
- **Turnier (Jeder gegen Jeden)** mit Round-Robin-Spielplan, dynamischer
  Tabelle und optimierter Match-Reihenfolge (Greedy-Scheduler verteilt
  Wartezeiten gleichmäßig)
- **Live-Statistik pro Match**: 3-Dart-Average, First-9-Average, Highest
  Visit/Dart, 100+/140+/180-Counter, Highest Checkout, Triples, Doubles,
  Bulls, Misses, Busts
- **Hit-Verteilung** pro Spieler — welches Feld wie oft getroffen wurde
- **Verlauf-Statistik** über wählbare Zeiträume (Heute / 7 / 30 Tage / Alles
  / Benutzerdef.) mit Sektionen: Sieg-/Leg-/Wurf-/Trefferraten/Hohe Aufnahmen/
  Felder-Statistiken / Checkout
- **Persistente Spieler-Liste** (Schnellauswahl + Autocomplete im Setup,
  Filter-Chips im Verlauf)
- **Setup wird gemerkt** und ist mit einem Klick wiederholbar
- **Checkout-Vorschläge** ab Restpunktzahl ≤ 170 (Double-Out)
- **Verlauf-Export/Import** als JSON

## Lokal verwenden

Datei `index.html` einfach im Browser öffnen — fertig.

## Auf dem Tablet

1. `index.html` aufs Tablet kopieren (AirDrop / iCloud / E-Mail / USB)
2. In Safari/Chrome öffnen
3. „Zum Home-Bildschirm hinzufügen" → läuft offline wie eine App

## Online via GitHub Pages

In den Repository-Settings unter **Pages** als Source „Deploy from a branch"
wählen, Branch `main` und Ordner `/ (root)`. Nach 1–2 Minuten ist die App
unter `https://<username>.github.io/<repo>/` erreichbar.

## Datenspeicherung

Alle Daten (Spielverlauf, Setup, Spielernamen) liegen ausschließlich im
`localStorage` des jeweiligen Browsers — kein Server, kein Tracking, keine
Cloud. Über die Export/Import-Funktion im Verlauf-Tab lassen sich Daten
zwischen Geräten übertragen.
