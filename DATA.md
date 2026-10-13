# Data notes

Large files not yet in the repo (size limits / API constraints):

- `seed/nyc_restaurants_enriched.json` (~10 MB) — full NYC DOHMH restaurant list with enrichment
- `seed/nyc_pe_matched.json` (~300 KB) — PE brand matches
- `seed/wonder_locations.json` — Wonder kitchen locations (to be added)
- `map/nyc-smoke-map.html` — Leaflet smoke-test map
- `map/nyc-smoke-points.json` — point data for the map
- `map/nyc-smoke-preview.png` — preview screenshot
- `Independence-Map-NYC.html` — standalone map

These can be added via git push from a local clone or Git LFS for the largest ones.

Core scoring schema, formula, PE companies/brands, claim detection, and gold examples are in `seed/`.
