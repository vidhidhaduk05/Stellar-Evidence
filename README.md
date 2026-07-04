# Stellar Evidence — Hackathon Submission

Landing page for **Stellar Evidence**, a systematic-review AI product built for
the evidence-based medicine hackathon. A single self-contained HTML file — all
CSS, JavaScript, animations, and images embedded — designed to work with zero
build tooling and zero external dependencies at runtime.

## Quick start

Open `index.html` in any modern browser:

```bash
# macOS
open index.html

# Linux
xdg-open index.html

# Windows
start index.html
```

Or serve it locally on a lightweight HTTP server:

```bash
# Python 3
python3 -m http.server 8000
# then visit http://localhost:8000

# Or Node (npx)
npx serve .
```

## Repository contents

```
.
├── index.html   # Full landing page — ~960 KB, self-contained
├── README.md    # This file
└── .gitignore
```

## Deploying

Because it's a single static HTML file, you can host it anywhere that serves
static files:

- **GitHub Pages**: push to `main`, then enable Pages under
  *Settings → Pages → Deploy from a branch → main / (root)*.
- **Netlify / Vercel / Cloudflare Pages**: drop the folder in via the dashboard.
- **Any static host / S3 / R2**: upload `index.html` and browse to it.

## What's inside

The page includes the following sections (matching the eyebrow numbering
`[ 01 ]` — `[ 11 ]`):

1. Hero with parallax product mockup (an 8-year-old pediatric FCE case report
   flowing into PICO extraction cards)
2. Features grid with the *"01 // EXTRACT"* compact FCE mockup
3. Human-in-the-loop verification workflow
4. Sticky-note research board with a *"Coming soon — In preparation"* validation
   ribbon banner
5. Methods / TRIPOD-LLM alignment
6. Implementation study
7. Precision features with a fuller *"Field-level confidence scoring"* FCE mockup
8. Team collaboration section (with its own dashboard mockup)
9. Testimonials
10. FAQ
11. Why this matters — patient / researcher / rigor framing

Every fade-up, tilt, scroll-triggered animation, and the corkboard sticky-note
layout is driven by inline JavaScript at the bottom of the file — nothing is
loaded from a CDN, so it will render identically wherever you host it.

## License

See `LICENSE`. If you don't intend to publish an open license, delete the
`LICENSE` file before pushing.
