# Garment Tech Radar

A lightweight news dashboard for tracking garment manufacturing tech, automation, and digital tooling news. Built to match the visual language of the main portfolio (`hello-portfolio.hoeurnhello.workers.dev`).

## What's in this zip
```
tools/
└── garment-tech-radar.html   ← the full tool, ready to deploy
```

## Adding it to your portfolio repo

1. Copy the `tools/` folder into the root of your portfolio repo, alongside `index.html`, `projects/`, etc.
2. Commit and push:
   ```bash
   git add tools/garment-tech-radar.html
   git commit -m "Add Garment Tech Radar tool"
   git push
   ```
3. It will publish at:
   ```
   https://hello-portfolio.hoeurnhello.workers.dev/tools/garment-tech-radar.html
   ```
4. Optional — link it from your nav in `index.html`:
   ```html
   <li><a href="tools/garment-tech-radar.html">Tech Radar</a></li>
   ```
5. Optional — add it to `sitemap.xml`:
   ```xml
   <url><loc>https://hello-portfolio.hoeurnhello.workers.dev/tools/garment-tech-radar.html</loc></url>
   ```

## Notes
- Custom feeds you add are saved via `localStorage` — persistent per browser/device, no server sync.
- Preloaded default feeds (Apparel Resources, Just Style, Fibre2Fashion) — worth double-checking their RSS URLs are still live, since publications change endpoints occasionally.
- News fetching uses the free rss2json API client-side; no backend required.
