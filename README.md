# Bilal's Portfolio

Personal portfolio site — Muhammad Bilal, Senior Frontend & AI Engineer.
Single static `index.html` (no build step), plus `cv.html` and its PDF export. Deployed on Vercel.

## Structure

- `index.html` — the whole site: markup, styles and script inline.
- `fonts/` — self-hosted variable fonts (Archivo with width and weight axes, JetBrains Mono).
- `vendor/` — GSAP 3.15 (ScrollTrigger, SplitText) and Lenis 1.3 smooth scrolling, loaded locally (no CDN).
  `lenis.min.js` is wrapped in a function scope because the published build leaks short global names.
- `media/` — portrait, link-preview image and case-study demo videos.

## Behaviour worth knowing

- Case studies are an index: each row opens into the full write-up. Without JavaScript every case study is shown expanded.
- Animation and smooth scrolling are skipped for visitors who prefer reduced motion, and demo videos get controls instead of autoplay.

## Preview locally

```bash
python3 -m http.server 4173
```

Then open http://127.0.0.1:4173/.
