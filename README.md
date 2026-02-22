# 🇩🇪 Länderfinanzausgleich Visualisierung (1950–2024)

Interaktive Darstellung des deutschen Länderfinanzausgleichs im engeren Sinne als HTML-Einzeldatei – keine Dependencies, kein Build-Prozess, einfach öffnen.

![Preview](preview.png)

## Features

- **Liniendiagramm** mit allen 16 Bundesländern über den gesamten Zeitraum 1950–2024
- **Rot** = Nehmerländer (positive Werte / Empfänger), **Grün** = Geberländer (negative Werte / Zahler)
- Individuelle **Strichmuster & Farbnuancen** pro Bundesland für bessere Unterscheidbarkeit auch im Druck
- **End-Labels** direkt an den Linien mit automatischer Kollisionsvermeidung
- **Vollbildmodus** (wie YouTube) – Chart skaliert dynamisch mit ⛶-Button
- **Tooltip** bei Mouseover mit allen Länderwerten für das jeweilige Jahr (fixiert auf ¾ der Chart-Höhe)
- **Zusammenfassung** der kumulierten Gesamtbeträge aller Geber- und Nehmerländer
- **Datentabelle** mit allen Jahreswerten, farbcodiert nach individuellem Vorzeichen (nicht nach Kategorie)

## Datenquelle

Wikipedia – [Länderfinanzausgleich](https://de.wikipedia.org/wiki/L%C3%A4nderfinanzausgleich)  
Ursprungsquelle: Wissenschaftlicher Dienst des Bundestages / Bundesfinanzministerium

## Verwendung

```bash
git clone https://github.com/dein-name/laenderfinanzausgleich.git
# Datei im Browser öffnen – fertig.
open laenderfinanzausgleich.html
```

Keine Installation, keine Abhängigkeiten außer einer Internetverbindung für das CDN-Loading von [Chart.js](https://www.chartjs.org/) (v4.4.1).

## Technik

- HTML / CSS / Vanilla JavaScript
- [Chart.js 4.4.1](https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.min.js) via CDN
- Custom Chart.js Plugin für End-Labels und Tooltip-Positionierung
- Fullscreen API (mit webkit-Fallback)

## Lizenz

MIT
