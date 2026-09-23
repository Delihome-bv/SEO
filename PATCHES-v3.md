# Patches for benchmark v3

## PATCH 1 — 00-ROOT.md
Add to the canonical houses table:

| Which retailer carries which worktop route / may receive the CanDo series story? | `07-RETAILER-ROUTES.csv` |

Add under conflict rules:
- Retailer availability and route eligibility are owned by `07-RETAILER-ROUTES.csv`.
- Product truth may not be used to infer retailer availability.
- A locale sitemap may prove a URL exists, but it does not prove that the retailer carries the CanDo three-series proposition.
- `OPEN` retailer rollout must remain unresolved.

## PATCH 2 — 01-ORCHESTRATOR.md
In PREPARE, load:
- `07-RETAILER-ROUTES.csv`

Add to Gate 0:
- retailer route matrix exists;
- at least one valid retailer route exists for the requested locale;
- any OPEN rollout dependency is identified before BUILD.

In RESEARCH/RESOLVE:
- verify proposed CTA destinations against BOTH:
  1. locale sitemap/live web;
  2. `07-RETAILER-ROUTES.csv`.

A valid URL is not enough if the retailer route is not valid for the CanDo series.

## PATCH 3 — 06-CONTENT-WORKBOOK.md
Under CTA role add:

Retailer selection is governed by `07-RETAILER-ROUTES.csv`.
Do not infer that every retailer selling a worktop carries Essential/Advance/Signature.
If Advance/Signature retailer rollout is OPEN, the page may describe the series but must not present confirmed retailer availability for those series.

## PATCH 4 — skills/seo-page-build/SKILL.md
Add `07-RETAILER-ROUTES.csv` to required inputs.

Add to Source Decision Log:
- retailer eligibility;
- DEK/CanDo versus FAB/no-name;
- whether series availability is CONFIRMED or OPEN;
- delivery-time applicability by series.

## PATCH 5 — skills/commercial-localization/SKILL.md
Add `07-RETAILER-ROUTES.csv` to required inputs.

Under link localization:
- first select retailers/routes valid for the target locale and product proposition;
- then validate the URL using that locale's sitemap/live web;
- never replace a missing BE-FR route with a French retailer.

## PATCH 6 — 09-QA-GATE.md
Add:

### I. Retailer / route governance
PASS only if:
- no CanDo series story routes to FAB/no-name retailers;
- BE-FR uses Belgian retailer routes, not FR retailers;
- Bouwmaat is not consumer-facing while status is OPEN;
- Essential delivery is not copied to Advance/Signature;
- OPEN Advance/Signature retailer rollout is not presented as confirmed;
- every CTA destination is valid in both retailer matrix and locale sitemap/live check.

Any invented retailer-series availability = CRITICAL DEFECT.
