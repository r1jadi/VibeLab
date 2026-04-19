# VibeLab ✦ Aesthetic Generator

> Describe a mood. Get a complete design aesthetic — instantly.

VibeLab is a single-file web app that turns any mood, theme, or feeling into a full design system: color palette, font pairing, imagery keywords, soundtrack suggestion, and a design philosophy. No API keys, no backend, no dependencies.

---

## Demo

Type anything into the generator:

- *"golden hour rooftop party"* → warm ambers, terracotta, Cormorant Garamond, Fred again..
- *"neon Tokyo convenience store at 2am"* → hot magenta, electric cyan, Space Mono, Burial
- *"dark academia library at midnight"* → aged gold, walnut, Playfair Display, Bill Evans

---

## Features

- **Instant generation** — runs entirely in the browser, zero latency
- **6 aesthetic categories** — warm, cool, neon, dark, nature, luxury
- **Full design output** — palette, fonts, imagery, soundtrack, design principle
- **One-click copy** — exports the full vibe summary to clipboard
- **Featured vibe cards** — clickable presets to get started fast
- **Bold landing page** — animated hero, custom cursor, scrolling ticker, responsive layout
- **Single HTML file** — no build step, no npm, no config

---

## Getting Started

### Run locally

Just open the file in a browser:

```bash
git clone https://github.com/yourusername/vibelab.git
cd vibelab
open index.html
```

No install step. No server needed.

### Deploy to Vercel

```bash
npm i -g vercel
vercel
```

Or drag and drop the folder into [vercel.com/new](https://vercel.com/new). Done in 30 seconds.

### Deploy to Netlify / GitHub Pages

Works with any static host — just serve `index.html` at the root.

---

## Project Structure

```
vibelab/
└── index.html   # entire app — HTML, CSS, JS in one file
```

That's it.

---

## How It Works

VibeLab uses a keyword-matching engine to classify your input into one of six aesthetic categories, then maps that category to a handcrafted design system:

```
input text
    → keyword scoring across 6 categories
    → classify to best-matching aesthetic type
    → render palette, fonts, imagery, soundtrack, principle
```

Each aesthetic category has its own:

- 5-color palette with named swatches
- Heading + body font pairing with rationale
- 5 imagery and texture keywords
- Curated soundtrack suggestion
- One-sentence design philosophy

---

## Aesthetic Categories

| Category | Mood | Example input |
|----------|------|---------------|
| Warm | Warm & euphoric | golden hour, sunset, rooftop, amber |
| Cool | Clear & contemplative | ocean, fog, nordic, minimal |
| Neon | Quietly electric | neon, tokyo, 2am, synthwave |
| Dark | Rich & brooding | jazz, academia, noir, gothic |
| Nature | Grounded & alive | forest, cottage, botanical, cabin |
| Luxury | Refined & magnetic | marble, silk, champagne, editorial |

---

## Customization

All vibes are defined in the `VIBES` object inside `index.html`. To add a new aesthetic category:

1. Add keywords to `VIBES.keywords`
2. Add a 5-color palette to `VIBES.palettes`
3. Add font pairing to `VIBES.fonts`
4. Add mood/energy labels to `VIBES.moods`
5. Add imagery tags to `VIBES.imagery`
6. Add a soundtrack to `VIBES.soundtracks`
7. Add a design principle to `VIBES.principles`

---

## Tech Stack

- Vanilla HTML / CSS / JavaScript
- [Syne](https://fonts.google.com/specimen/Syne) — display font
- [DM Sans](https://fonts.google.com/specimen/DM+Sans) — body font
- [DM Mono](https://fonts.google.com/specimen/DM+Mono) — monospace accents
- Google Fonts CDN (only external dependency)

---

## License

MIT — do whatever you want with it.

---

*Built with [VibeLab](https://github.com/yourusername/vibelab) · What's your vibe?*
