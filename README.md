# restaurant-tracker

An app / map / database that tracks restaurants and scores them on:

- Ownership by or funding from **private equity**
- Ownership by or funding from **Wonder** (with nuanced signals: owned_kitchen, platform_brand, service_customer, etc.)
- Produce sourcing: **Sysco** vs local sources

## Current seed data (NYC pilot)

- `seed/companies.json` — PE firms and Wonder
- `seed/brands.json` — PE-backed brands
- `seed/schema_signals.json` — signal vocabulary (v1.1)
- `seed/score_formula.json` — scoring formula
- `seed/claim_phrases.json` — phrases for detecting ownership/sourcing claims
- `seed/claims_gold.json` — gold examples for claim detection
- `seed/wonder_locations.json` — Wonder kitchens
- `seed/nyc_pe_matched.json` — PE brand matches in NYC
- `map/` — Leaflet smoke-test map for NYC

Scoring starts at 70 and applies penalties/bonuses based on known signals. Unknown data is neutral. Ownership penalties only apply to owned_kitchen / platform_brand (not B2B service_customer).

Data sourced from public records (NYC DOHMH), company sites, and manual curation. Always include source, reliability, and last-updated.
