# Bayelsa Evidence Atlas — documented oil-spill recurrence (2006–2018)

Interactive historical evidence dashboard by **Gabriel Bahago Samuel**.

The atlas shows 300 m analysis cells associated with accepted documented NOSDRA spill records. Enlarged symbols help interpretation; they **do not** depict spill footprints, environmental contamination or validated event probabilities.

## Public deployment

This repository is a stand-alone, static GitHub Pages project. Files are already arranged in the site root.

1. Enable **Settings → Pages → Deploy from a branch → main / (root)**.
2. Verify `https://bahagogabriel.github.io/bayelsa-evidence-atlas/` after the Pages deployment finishes.
3. Test the six filters, map markers, zoom-to-cell polygons, focus control and Methods page.
4. Confirm only the API-key-free OpenFreeMap Positron basemap is displayed.

The `.nojekyll` file preserves static assets without Jekyll processing.

## Data and interpretation

- Recorded spill incidents, 2006–2018: **3,109**.
- Historical pre-2018 evidence cells: **777**.
- Cells with at least one documented event in 2015–2017: **312**.
- First-recorded 2018 cells: **11** (12 events), shown separately for evaluation only.
- A model using past three-year event count outperformed the more complex machine-learning model in temporal holdout average precision (0.2417 vs 0.1900).

Recorded absence is **not** proof of no physical spill. This is historical recurrence screening, not a contamination map or operational spill probability product.

For full methodology and limitations, see [`methods.html`](methods.html) and [`G12R3_Scientific_Report.md`](G12R3_Scientific_Report.md).

## Local testing

From this folder run `python -m http.server 8000`, then open `http://localhost:8000/`. Basemap tiles and MapLibre libraries require internet access.

## Data preservation

The two GeoJSON inputs are byte-for-byte copied from the accepted G12R4.2 package. No scientific classification or geometry is edited for this publishing release.
