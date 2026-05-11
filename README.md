# Japan — November · Roy & Family

An interactive travel guide for a two-week Japan trip: Roy's solo week in Tokyo, followed by a family week in Osaka. Built as a single self-contained HTML file — no build step, no framework, no dependencies to install.

## Features

- **Interactive maps** — Leaflet.js maps on every day, pinning each location with clickable markers that open Google Maps
- **Sticky journey timeline** — visual route timeline at the top, highlights the current section as you scroll
- **Expandable travel tips** — accordion sections covering transport, luggage, money, and connectivity
- **Light/dark mode** — auto-detects system preference, manual toggle in the header, map tiles switch too
- **PDF export** — print-ready layout via `window.print()`, with text fallbacks replacing maps

## Structure

```
Roy — Tokyo Solo (Days 1–5)
  Day 1  Ueno + Akihabara
  Day 2  Harajuku + Shibuya
  Day 3  Yokohama (day trip)
  Day 4–5  Hakone (overnight, ryokan)

Roy + Family — Osaka (Days 1–7)
  Day 1  Arrive + Dotonbori
  Day 2  Kuromon Market + Shopping
  Day 3  Osaka Aquarium
  Day 4  Nara (day trip)
  Day 5  Osaka Castle
  Day 6–7  Kyoto (overnight)
  Optional  Hiroshima
```

## Usage

Open `index.html` directly in a browser — no server required.

To deploy, push to a GitHub repository and enable GitHub Pages pointing at the root.

## Stack

| Concern | Solution |
|---|---|
| Maps | Leaflet.js 1.9.4 via CDN |
| Tiles | CartoDB Light / Dark Matter |
| Fonts | Playfair Display + DM Sans via Google Fonts |
| Interactivity | Vanilla JS (no framework) |
| Scroll tracking | IntersectionObserver |
