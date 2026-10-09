# Bayelsa: Documented Spill Recurrence and Contextual Exposure (2006–2018)

**Status:** G12 R2 technically completed. G12 R3 cartography prepared for FINAL VISUAL QA. Publication not yet approved.

## Purpose and scientific position
Provide exploratory, spatially explicit evidence of documented oil-spill recurrence and contextual receptors in Bayelsa State, Nigeria. The primary analysis concerns reports and their recurrence, **not physical spill probability, field-measured contamination or causal attribution**.

## Validated source counts
- 3,109 documented events in 2006–2018 on 107,133 model cells (nominal 300 m).
- 3,078 of these events are pre-2018; 2018 has 31 recorded events in 29 positive cells.
- The 2018 recurrence classes use ONLY 2017-and-earlier incidents. Observed 2018 labels appear exclusively in independent evaluation summaries.

## Descriptive 2018 recurrence evidence
- Cells with at least one recorded event during 2015–2017: **312**, representing **0.291%** of model cells.
- These cells contained **14 of 31** documented 2018 events (**45.2%**). This does not demonstrate reliable performance at new, previously unrecorded locations.

| Recurrence class | Model cells | 2018 documented events |
|---|---:|---:|
| 4+ events in 2015-17 | 48 | 7 |
| 2-3 events in 2015-17 | 83 | 2 |
| 1 event in 2015-17 | 181 | 5 |
| Older history only | 465 | 5 |
| No prior recorded spill | 106,356 | 12 |

## Machine-learning comparison and limitations
- Rolling 2016–2018 holdout AP: logistic ML **0.189978**; simple recent-three-year count **0.241718**.
- The simple recurrence benchmark outperformed ML. Novel-location discrimination was weak. The scores must not be interpreted as calibrated physical spill probabilities.
- Validation was rolling annual using strictly earlier history, rather than a three-year 2015-frozen forecast. Discrete count ties make exact top-k screening thresholds ambiguous.

## Contextual population, built area, and historic water
- WorldPop 2018 modelled population: approximately 2,040,673 in the source-supported allocated cells; 104,718/107,133 cells supported.
- GHSL 2015 reconstructed built surface: 38,279,288 m² approximate allocated total; 106,838/107,133 cells supported.
- WorldPop and GHSL estimates use native-grid pixel-centre allocation and have boundary and modelling uncertainty. These are NOT numbers of people or structures affected by spills.
- GHSL 2015 represents an R2023A historical reconstruction, not a contemporaneous published 2015 layer. JRC 2015–2017 surface-water occurrence does not reveal oil pollution.

## Cartographic changes at R3
- Five A3 landscape maps (PNG and PDF). Occurrence and recurrence maps use scaled point symbols at computational-cell centres and two count-density-selected insets. Marker sizes are symbolic, not physical spill extent.
- Population and built-area maps use log-scaled positive-value displays capped at the 99th percentile for visualization only. Underlying data remain unchanged. Missing coverage is separate from a valid zero.
- Include UTM coordinate frame, north arrow, scale bar, scientific disclaimer, and map-specific attribution. Insets are labelled A and B without asserting unverified named settlements.

## Data and attribution
- Accepted NOSDRA documented spill records (2006–2018); accepted HDX Bayelsa boundary; 300 m model grid.
- Satellite and ancillary sources from locked earlier processing: JRC Global Surface Water, Landsat, CHIRPS, NASADEM.
- WorldPop GP 2018; JRC GHSL GHS-BUILT-S R2023A (2015 reconstructed epoch).
- Model and audit: G10C.2, G11, G11B. This R3 reads checksum-verified G12 R2 results and does not retrain or recompute the scientific baseline.

## Scientific restrictions
- Unknown/unreported spills are not observable zeros. No confirmed spatial contaminated extent, remediation cost, direct damage or health exposure is mapped.
- No oil-infrastructure presence/absence model can be claimed. Infrastructure coverage was deemed insufficient for historical backtesting.
- Do not label maps as oil-spill probability or confirmed environmental contamination. Descriptive screening should guide field verification, not substitute for it.
- Web preview is local and depends on MapLibre CDN and OSM tiles; it is not hosted or externally verified.

## Publication gate
R3 production does not automatically approve its own cartography. Review the REAL A3 PDF renders and all map captions, then explicitly approve or request corrections.

Revision: `G12R3_FINAL_CARTOGRAPHY_20261009`
