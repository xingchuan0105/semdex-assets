# Semdex

Pre-compile your website into static Markdown, JSON, and progressive chunks for AI agents — with `Accept: text/markdown` content negotiation, strong ETags, `/llms.txt`, `/sitemap.xml`, and `Content-Signal` headers.

Your origin remains the source of truth for auth, payments, and dynamic UI. Semdex compiles public pages at write time so AI crawlers and coding agents hit edge-cached semantic artifacts instead of re-scraping SSR HTML.

## Try the live semantic replica

Our own SaaS site (`contextlm.top` / `app.contextlm.top`) is tenant #1 (`agent.contextlm.top`):

```bash
curl -sS -H 'Accept: text/markdown' https://agent.contextlm.top/ | head -n 25
curl -sSI -H 'Accept: text/markdown' https://agent.contextlm.top/compare
curl -sS https://agent.contextlm.top/llms.txt
```

- Live agent-compiled replica & side-by-side diff: https://agent.contextlm.top/compare
- Free URL Agent-Readability & GEO Grader: https://semdex.contextlm.top/grader
- Product overview & 7-day trial: https://semdex.contextlm.top/en.html
- Product Hunt launch (2026-11-17): https://www.producthunt.com/products/semdex?launch=semdex

## Assets in this repository

- `logo-240.png` — 240×240 product mark
- `g1-negotiation.png` — HTTP `Accept: text/markdown` content negotiation & strong ETag headers
- `g2-agent-view.png` — Agent-facing semantic view & progressive chunks
- `g3-scenarios.png` — Public scenarios & `/llms.txt` index
- `g4-compare.png` — Side-by-side HTML vs compiled Markdown comparison
