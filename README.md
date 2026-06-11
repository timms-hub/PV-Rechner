# PV-Rechner

Ein Wirtschaftlichkeitsrechner für Photovoltaik-Anlagen mit Batteriespeicher,
Wärmepumpen- und E-Auto-Berücksichtigung. Läuft vollständig im Browser –
ohne Server, ohne Build-Schritt, ohne externe Abhängigkeiten. Eine einzige
HTML-Datei.

## Funktionen

- **Mehrere PV-Strings** mit individueller Ausrichtung (Himmelsrichtung oder
  freier Azimut-Winkel) und Neigung
- **Stündliche Jahressimulation** (8760 h) aus typisierten Erzeugungs- und
  Lastprofilen
- **Speicher-Sweep**: vergleicht Speichergrößen und empfiehlt die wirtschaftlich
  sinnvollste Stufe
- **Wirtschaftlichkeit**: Investition, Cashflow über die Laufzeit,
  Amortisationszeit, Autarkie- und Eigenverbrauchsquote
- **Wärmepumpen-Vergleich**: WP mit PV-Eigenanteil gegen die bisherige Heizung
  (Gas/Öl/Pellets/Fernwärme/Strom)
- **E-Auto-Last** optional integrierbar
- **Regionaler Ertrag** über PLZ-Zuordnung
- **Druck-/PDF-Ansicht** für ein sauberes Angebots-/Berichtslayout
- **Speichern & Laden** der Eingaben als JSON-Datei

## Nutzung

Es gibt nichts zu installieren. `index.html` im Browser öffnen – fertig.
Entweder lokal per Doppelklick oder online, sobald die Datei auf einem
Webspace liegt (siehe unten).

## Hosting auf dem eigenen Webspace

Da es sich um eine einzelne statische Datei ohne Backend handelt, genügt es,
`index.html` in das öffentliche Verzeichnis des Webspace zu legen (oft
`public_html/`, `htdocs/` oder `www/`). Liegt sie direkt im Wurzelverzeichnis,
ist die App anschließend unter der Domain erreichbar (z. B.
`https://deine-domain.de/`). In einem Unterordner entsprechend unter
`https://deine-domain.de/pv-rechner/`.

## Technik

Vanilla JavaScript, CSS-Variablen fürs Theming, SVG-Charts – alles inline in
einer Datei. Keine Frameworks, kein npm, kein Build.

## Lizenz

Siehe [LICENSE](LICENSE).
