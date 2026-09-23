# Content Architecture — Worktops Benchmark

## 1. One concept, market-specific routes
The strategic page job can be shared across markets. The URL/link graph cannot be assumed to be identical.

Per market:
- validate the owner route;
- validate parent/sideways/forward links;
- use that market's sitemap;
- confirm redirects/live state where relevant.

## 2. Sitemap ownership
- NL: `07-LINKS/sitemap-nl.csv`
- BE-NL: `07-LINKS/sitemap-be-nl.csv`
- BE-FR: `07-LINKS/sitemap-be-fr.csv`

The sitemap is the first link universe. Live web validation confirms current state. Never invent a translated URL.

## 3. Link directions
UP: direct parent in that locale's tree.
SIDEWAYS: direct local alternatives / comparison content that actually exists.
FORWARD: next decision or retailer handoff for that locale.

## 4. Different locale link structures are allowed
A localized page does not need to have the same internal-link set as NL.
If NL has a choice page but BE-FR does not, BE-FR must not invent it. Use the best valid local route instead and log the structural difference.

## 5. Retailer handoff
Use only retailer/route destinations valid for that locale and proposition.
Do not route CanDo three-series content into an unrelated no-name/FAB proposition.

## 6. Measurement
Primary observable action on W8: outgoing retailer click.
Secondary: retailer-configurator click, sample request, decision-content interaction.
Do not equate click-out with purchase.
