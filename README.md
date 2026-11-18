# Bilal's Portfolio

Personal portfolio site — Muhammad Bilal, Senior Frontend & AI Engineer.
Single static `index.html` (no build step), plus `cv.html` and its PDF export. Deployed on Vercel.

## Structure

- `index.html` — the whole site: markup, styles and script inline.
- `fonts/` — self-hosted variable fonts (Bricolage Grotesque, Instrument Sans, JetBrains Mono).
- `vendor/` — GSAP 3.15 with ScrollTrigger and SplitText, loaded locally (no CDN).
- `media/` — portrait, link-preview image and case-study demo videos.

## Preview locally

```bash
python3 -m http.server 4173
```

Then open http://127.0.0.1:4173/. Animation is skipped for visitors who prefer reduced motion, and the page stays readable if scripts fail to load.
