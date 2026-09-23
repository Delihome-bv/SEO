# Deli Home Marketing AI Benchmark — ROOT

Version: 3.0
Freeze date: 2026-09-15
Scope: CanDo Worktops Made to Measure
Markets: NL, BE-NL, BE-FR
Purpose: capability benchmark only. Never publish.

## Central operating rule
The user gives one normal marketing assignment. The user does not manually choose a specialist.

The central system must:
1. recognise task type and target markets;
2. load only relevant shared context;
3. route to the correct specialist workflow;
4. obey source ownership and conflict rules;
5. use web only for current/live information;
6. execute the work;
7. send the NL source through independent QA;
8. when another locale is requested, invoke the commercial-localization specialist;
9. validate locale-specific links against that locale's sitemap and live web;
10. return a review-ready result or explicitly stop.

## Functional routing
### Source-market page build
- use `skills/seo-page-build/SKILL.md`;
- then `skills/source-quality-qa/SKILL.md`.

### Localization / transcreation
For BE-NL or BE-FR:
- do not translate literally;
- invoke `skills/commercial-localization/SKILL.md`;
- localize from approved meaning, product truth, page job, audience, local search context and local sitemap;
- perform three internal refinement passes before producing localized output.

The user does not have to name any skill.

## Canonical houses
| Question | Canonical source |
|---|---|
| Brand / tone | `02-BRAND.md` |
| Audience | `03-AUDIENCE.md` |
| Product truth | `04-PRODUCT-TRUTH.md` |
| Claims | `05-CLAIMS-POLICY.md` |
| Page job | `06-CONTENT-WORKBOOK.md` |
| Journey / links / measurement | `07-CONTENT-ARCHITECTURE.md` |
| Locale URLs | `07-LINKS/sitemap-*.csv` |
| SEO/GEO | `08-SEO-GEO-RULES.md` |
| Locale writing | `08-LOCALE-RULES.md` |
| Form / layout | `05-STRAMIEN/stramien-landingspagina-v6.html` |
| Source QA | `09-QA-GATE.md` |

## Conflict rule
A source owns only its own type of truth.
Priority:
1. explicit benchmark freeze rules;
2. canonical file for that information type;
3. locale sitemap for URLs;
4. current live web for live status/search context;
5. old/live copy as diagnostic input only.

Never let a live page overwrite newer internal product truth.
Never let localization create a new product fact.
Never let an NL URL imply the BE equivalent exists.
Never let old template copy create a product claim.

## Status vocabulary
- CONFIRMED: may be used as fact.
- OPEN: unresolved; do not publish as fact.
- VERIFY_LIVE: must be checked on the public web.
- FORBIDDEN: never use in consumer output.

## Hard stop
Never publish, update CMS, send data externally or modify a business system during this benchmark.
