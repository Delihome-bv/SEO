# Retailer & Route Matrix — Worktops Benchmark

This file is the canonical house for retailer availability and retailer-route eligibility for the benchmark.

## Source basis
Primary source supplied by Zoë:
`Micro-site data-feed 3.22.20-PROD.xlsm`, sheet `Micro-site FEED`, feed version 3.22.20-PROD, peildatum 17-07-2026.

Additional benchmark reconciliation:
- current CanDo/DEK worktop line and FAB/no-name line must remain separate;
- BE-FR uses the same Belgian retailers as BE-NL, not the French retailers;
- Advance and Signature rollout per retailer is NOT confirmed by this source and is therefore `OPEN`.

## Hard rules
1. If `cando_series_story_allowed = no`, the CanDo Essential/Advance/Signature story may not route to that retailer.
2. `OPEN` is not `yes`.
3. Never extrapolate Essential availability or delivery time to Advance or Signature.
4. France (`fr-FR`) is not Belgian French (`fr-BE`).
5. A retailer present in the feed is not automatically safe for consumer communication if its channel status is unresolved.
6. CTA URLs still have to be validated against the locale sitemap/live route.
7. This file owns retailer availability/route eligibility. It does not own product specs or page copy.

## Benchmark conflict
The current feed confirms the existing Essential-equivalent line at several retailers.
It does NOT confirm rollout of Advance and Signature.

A strong AI should therefore:
- describe Advance and Signature from product truth where allowed;
- NOT claim they are already orderable at every Essential retailer;
- NOT invent delivery times for them;
- flag retailer rollout as unresolved if the final CTA depends on it.
