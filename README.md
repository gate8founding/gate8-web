# GATE8 — Brochure Site

Single-page brochure site for **GATE8**, a mindset brand and movement founded by 9× BMX World Champion Shanaze Reade.

Primary audience: funding institutions, schools and education partners, sports brands, and athletes/creators interested in GATE8 Media representation.

## Stack

Plain HTML, CSS and vanilla JS — one self-contained `index.html` plus an `assets/` folder. No build step.

Fonts load from Google Fonts (Poppins, Archivo, Instrument Serif, JetBrains Mono).

## Run it locally

Open `index.html` directly in a browser, or serve the folder:

```sh
python3 -m http.server 8080
# then visit http://localhost:8080
```

## Structure

```
gate8-brochure/
├── index.html           # full site — markup, styles, and scroll/parallax JS
└── assets/
    ├── gate8-logo.png / gate8-logo-inverse.png
    ├── gate8-labs.png / gate8-labs-inverse.png
    ├── gate8-media.png / gate8-media-inverse.png
    ├── gate8-foundation.png / gate8-foundation-inverse.png
    ├── shanaze-portrait-jersey.png
    ├── shanaze-academy.png
    └── shanaze-bench.png
```

## Sections

Hero · Manifesto · Lane counter (1–8) · Pinned pillars (Labs / Media / Foundation) · Problems · Why now · Founder · Quote ticker · Impact stats · Demand · Funder value prop · Media call · Contact · Socials · Footer.

## Notes

The partnership inquiry form is currently front-end only — submissions are not posted anywhere. Wire it to Formspree, Resend, a Slack webhook, or similar before going live.
