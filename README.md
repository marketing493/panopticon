# IA Panopticon

The one-stop hub for competitive intelligence at Impact Analytics. A single, self-contained page (`index.html`) that tells the story of five instruments and links into each one.

| # | Verb | Instrument | One-liner | URL |
|---|------|------------|-----------|-----|
| I | See | RivaLens | Their client list. Your line of sight. | https://rivalens-psi.vercel.app/ |
| II | Know | Account Scanner | X-ray any account before the first hello. | https://ia-account-scanner-odd0.onrender.com/ |
| III | Arm | Battlecard Builder | Win the head-to-head before the meeting starts. | https://ia-smart-battlecard-builder.onrender.com/ |
| IV | Host | NRF Venue RFP | Retail's biggest week. Every venue asked in one click. | https://nrf-venue-rfp.onrender.com/ |
| V | Expand | London Venue RFP | Your London stage, requested in one click. | https://london-venue.vercel.app/ |

## What is on the page

1. **The tower.** A plan view of Bentham's Panopticon. Five lit cells are the five instruments. The eye follows the cursor and turns to any cell you point at.
2. **The idea.** Why the name fits, revealed word by word as you scroll.
3. **The lifeline.** One chapter per instrument, joined by a heartbeat line that draws itself as you scroll. Each chapter says what the tool answers and what it hands to the next one.
4. **Plays.** Five ways to chain the instruments (The Displacement, The Transatlantic, The Shield, The Full House, The Mirror). Pick one and the route draws itself across the ring.
5. **The console.** Launch cards for all five tools. The page pings each tool when it loads, so sleeping Render servers start waking before anyone clicks.
6. **Command palette.** Press `Cmd K` (Mac) or `Ctrl K` (Windows) anywhere to jump to a tool, play or section.

## Light and dark versions

`index.html` is the default. It uses the IA Off-White background, with Black text and Impact Blue accents. The console band is Impact Blue and the footer uses the full-color IA logo.

`dark.html` is the same page on a Black background, with the white IA logo in the footer. To make it the default again, swap the two file names.

## Deploy

The page has no build step and no dependencies. Fonts load from Google Fonts. The logos are embedded.

**Render (Blueprint)**
1. New, then Blueprint, then pick this repository.
2. Render reads `render.yaml` and creates a static site called `ia-panopticon`.

**Render (static site, by hand)**
1. New, then Static Site, then pick this repository.
2. Build command: leave empty.
3. Publish directory: `.`

**Vercel**
1. Add New Project, then import this repository.
2. Framework preset: Other. Leave the root directory as is.
3. Deploy.

Any other static host works too. Upload `index.html`.

## Editing

* **Change a tool URL or one-liner:** search `index.html` and `dark.html` for the old URL or text and replace every match. Each tool appears in its chapter, its console card, the footer and the `INSTRUMENTS` list in the script.
* **Add or change a play:** edit the `PLAYS` list in the script. `path` uses instrument positions, from 0 (RivaLens) to 4 (London Venue RFP).
* The page sets `noindex, nofollow` so search engines skip it. Remove that meta tag if the page should be public.

## Brand notes

* Colors: Impact Blue, Off-White, Black, White, Grays, Data and Intelligence Blue (the only solution color used) and Accent Orange for live signals only.
* Type: Spectral Light (the Google alternate for ABC Otto) for headlines, Inter Tight for everything else.
* Logo: the blue logo mark in the nav and the full-color primary logo in the footer (the white version in `dark.html`), both above minimum size.
* Copy follows the IA voice rules. It has no em or en dashes and no invented statistics. The visuals inside each chapter are marked as illustrative.
