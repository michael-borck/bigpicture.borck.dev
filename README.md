# bigpicture.borck.dev

The **big picture** — a single, theme-first map of Michael Borck's AI teaching, tools, and
research at Curtin. Not a product site (those live at `tools.borck.education`, `locolabo.org`,
`books.borck.education`, …); this is the layer *above* them that ties the scattered work into one
story. Point people here when they ask *"what do you do / what are you working on?"*

Built in the same minimal **Astro** style as `borck.dev`, deployed to **GitHub Pages**.

## Develop

```bash
npm install
npm run dev      # http://localhost:4321
npm run build    # → dist/
npm run preview
```

## Content

All copy lives in the frontmatter arrays at the top of `src/pages/index.astro`
(`work`, `collab`, `exploring`) — edit there, no templating needed. Each entry leads with the
outcome/benefit and keeps an honest "what didn't work" note.

## Deploy

Pushing to `main` triggers `.github/workflows/deploy-pages.yml` (build → GitHub Pages).
`public/CNAME` sets the custom domain `bigpicture.borck.dev` — add the matching DNS record
(CNAME → `michael-borck.github.io`) and enable Pages → "GitHub Actions" in the repo settings.

## Source of the content

This started life as the Festival of AI 2026 EOI portfolio, reframed from "submissions" into an
evergreen, outcome-first overview of the body of work (including collaborations fronted by others).
