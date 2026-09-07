# Stabaliser weight visualiser

Design archery stabiliser weight stacks in 3D — set outer diameter, thickness,
bore, chamfer and quantity per disc, see the live mass in grams and ounces,
and export the result for printing or machining.

- **Live 3D preview** — turned discs with real chamfers, viewed stacked or
  laid out side by side.
- **Turned seams** — a global "seams every N oz" finish that visually splits
  a thick disc into what looks like a stack of smaller ones (e.g. a 6 oz part
  reading as 3 × 2 oz), without actually being separate pieces.
- **Exports**
  - **STL** — binary, millimetres, ready to 3D print a test fit.
  - **Part list (CSV)** — every dimension per disc, for a machinist to quote
    or cut from steel.
  - **SVG / DXF** — 1:1 mm profiles for a laser or waterjet.

No backend, no build step — it's a single static `index.html` with no
dependencies beyond two CDN-hosted libraries (Three.js for the 3D view,
Google Fonts for type). Open the file directly in a browser, or deploy it
anywhere that serves static files.

## Deploying

This is a single static HTML file — any static host works. For Vercel:

```
npx vercel
```

or connect this repo in the Vercel dashboard and deploy with no build
command (it's plain HTML, nothing to build).
