# Bilal's Portfolio

Personal portfolio site — Muhammad Bilal, Senior Frontend & AI Engineer.
Single static `index.html` (no build step), plus `cv.html` and its PDF export. Deployed on Vercel.

## Structure

- `index.html` — the whole site: markup, styles and script inline.
- `fonts/` — self-hosted variable fonts (Plus Jakarta Sans, JetBrains Mono).
- `vendor/` — GSAP 3.15 (ScrollTrigger, SplitText) and Lenis 1.3 smooth scrolling, loaded locally (no CDN).
  `lenis.min.js` is wrapped in a function scope because the published build leaks short global names.
- `media/` — portrait, link-preview image and case-study demo videos.

## Behaviour worth knowing

- Light theme with a moving colour-mesh background; navigation is a dock fixed to the bottom of the screen.
- About is shown as a streamed chat answer, Skills as auto-advancing tabs, Experience as a horizontal track on large screens, and the case studies as a console with a project list and one open study at a time.
- Without JavaScript, every tab panel and case study is shown in full, and the case-study list links jump to each study.
- Animation and smooth scrolling are skipped for visitors who prefer reduced motion; demo videos get controls instead of autoplay.

## Preview locally

```bash
python3 -m http.server 4173
```

Then open http://127.0.0.1:4173/.
