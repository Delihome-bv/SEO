# Contentwerkboek Werkbladen — Clean Benchmark

Freeze: 2026-09-15
Scope: CanDo worktop content cluster.
Benchmark build target: W8, `Werkbladen op maat`.
Markets: NL source, then BE-NL and BE-FR localization where requested.

## What this is
The translation from knowledge to a buildable page.

Per page this workbook defines:
- visitor decision task;
- page/search role;
- block jobs;
- which source house owns the facts for that block;
- page-specific prohibitions;
- CTA role;
- measurement;
- dependencies and internal-link role.

## What this is not
No second product knowledge base, keyword map, claims list, sitemap, measurement framework or template.
One fact, one house.

## 0. Houses of truth
| What | House |
|---|---|
| Product facts | `04-PRODUCT-TRUTH.md` |
| Allowed / forbidden / open claims | `05-CLAIMS-POLICY.md` |
| Keyword/search-demand facts | `06A-KEYWORD-MAP-WERKBLADEN.md` |
| Journey, link and measurement logic | `07-CONTENT-ARCHITECTURE.md` |
| Locale URLs | `07-LINKS/sitemap-*.csv` + live validation |
| Brand | `02-BRAND.md` |
| Audience | `03-AUDIENCE.md` |
| SEO/GEO rules | `08-SEO-GEO-RULES.md` |
| Locale language rules | `08-LOCALE-RULES.md` |
| Form | `05-STRAMIEN/stramien-landingspagina-v6.html` |
| QA | `09-QA-GATE.md` |

If old/live/template copy conflicts with product truth, product truth wins.
If an URL differs across markets, that market's sitemap wins.

---

## 0b. Link structure
The decision/choice layer is the functional node, not automatically the broad hub.

Every page uses three link directions:
- UP: direct parent in that market's current tree;
- SIDEWAYS: direct alternatives that genuinely exist;
- FORWARD: next decision or retailer handoff.

Hard rules:
1. never link to something that does not exist;
2. a sample CTA only links to the sample service for that category and locale;
3. do not translate URLs;
4. locale link structures may differ;
5. primary/secondary actions follow the supplied stramien.

---

## 1. Worktop cluster logic
Four facts steer the cluster:

1. Renovation/replacement is a major entry problem.
2. Made to measure is a high-intent route, not the entire category.
3. The messy middle requires comparison, reassurance and physical validation.
4. Essential / Advance / Signature must be translated into decisions, not presented as a technical data dump.

The series names are labels for the choice. They are not the SEO architecture.

---

## 2. Page agenda around the benchmark page
The benchmark builds only W8. The surrounding pages exist as routing/cannibalisation context.

| ID | Page concept | Main decision task | Role |
|---|---|---|---|
| W1 | Keukenblad / aanrechtblad vervangen | Can I replace only the worktop? | renovation entry |
| W2 | Wrappen of vervangen | Which renovation route fits? | comparison |
| W3 | Welk werkblad past bij jouw keuken | Which series/build fits? | messy-middle choice |
| W4 | Marmerlook keukenblad | I want the look; what am I actually buying? | look family |
| W5 | Houtlook werkblad | Is it real wood and what does that mean? | expectation management |
| W6 | Betonlook / steenlook | I want the look without claiming real stone | look family |
| W7 | Producthub werkbladen | Show me the available routes | router/hub |
| W8 | Werkbladen op maat | I know I need made to measure; what now? | **benchmark build target** |
| W9 | Stalenservice werkbladen | I want to validate colour/finish physically | validation |
| W10 | BE/FR made-to-measure | Same decision problem in local market | localized route, not literal translation |

Dependency rule:
W8 may link to W3/W9 or another planned child only if that page actually exists in that locale's sitemap/live site.

---

# 3. W8 — Werkbladen op maat

## 3.1 Decision task, in visitor language
Source meaning:
`Ik weet dat mijn werkblad op maat moet. Hoe kies ik de juiste uitvoering, welke uitsparingen kunnen vooraf worden voorbereid, wat moet ik zelf nog doen en waar ga ik daarna verder?`

This sentence defines meaning. It is NOT a sentence template for translation.

Register:
help choose → confirm → retailer handoff.

Primary anxieties:
- measuring incorrectly;
- precision cutting/milling;
- choosing the wrong series;
- understanding the sink difference;
- not knowing what happens after leaving CanDo.

## 3.2 Search role
NL source owner:
`https://www.cando.eu/nl-nl/hout/hout-op-maat/werkbladen-op-maat/`

Primary NL benchmark term:
`werkblad op maat` — 720/month.

Secondary NL vocabulary:
- werkbladen op maat;
- keukenblad op maat;
- aanrechtblad op maat;
- werkblad;
- keukenblad;
- aanrechtblad.

Do not create separate owner pages for synonym intent in this benchmark.

For BE-NL and BE-FR, the localization specialist re-evaluates terminology from the local search context and does not mechanically carry over NL term weighting.

## 3.3 Page job
By the primary CTA, the visitor must understand:
1. why made to measure is useful in this situation;
2. what precision work is prepared before delivery;
3. the practical choice between Essential / Advance / Signature;
4. which sink route belongs to which series;
5. what the customer still needs to do;
6. what happens at retailer handoff;
7. the next action.

This page is not:
- a material encyclopedia;
- a generic price page;
- a delivery-promise page;
- a comparison against every worktop material on the market;
- a new parallel owner page.

## 3.4 Block sequence and source ownership
The supplied HTML stramien owns visual structure. Map the following content jobs into it without redesigning the template.

| # | Block job | What it must do | Fact/source house |
|---|---|---|---|
| 1 | Hero | Give the made-to-measure promise and set expectation for the route | Brand + audience + this workbook |
| 2 | Why made to measure | Explain dimensions + prepared precision work | Product truth + claims |
| 3 | Which series fits | Translate Essential/Advance/Signature into choice criteria | Product truth |
| 4 | Sink difference | Explain Essential top-mounted vs Advance/Signature flush-mounted route | Product truth + claims |
| 5 | Measuring / precision reassurance | Explain what is prepared without absolute promises | Product truth + claims |
| 6 | How it works | Concise choose → dimensions/options → retailer → receive/place flow | Content architecture |
| 7 | Retailer handoff | Explain the system switch before CTA | Content architecture + locale sitemap/live check |
| 8 | FAQ | Answer high-intent remaining questions; no filler duplication | Keyword map + SEO/GEO |
| 9 | Final CTA | Continue to retailer choice/configuration | Content architecture |

If the stramien contains obsolete example copy, keep the structural block and replace the copy. The stramien owns form, not facts.

## 3.5 Product-choice translation
### Essential
Decision framing:
- familiar 38 mm HPL route;
- 25 decor names;
- straight edge;
- top-mounted sink route.

Do not imply flush mounting and do not turn internal/current price data into a consumer price promise.

### Advance
Decision framing:
- HPL look with a lighter internal construction;
- 32 or 38 mm;
- flush-mounted sink option;
- especially relevant when lower weight matters for larger worktops/islands.

Consumer wording:
`een lichte kern met een dragend raster`

Do not use honeycomb, recycled-wood-fibre raw-material claims, unconfirmed maximum dimensions, price or delivery time.

### Signature
Decision framing:
- 12 mm solid glass-based composite route;
- slim appearance;
- polished/velvet finishes;
- flush-mounted sink;
- PITT cooking where relevant.

Do not say 100% recycled worktop/material, fully recyclable, price or delivery time.

## 3.6 Sink and tap rule
Freeze 15-09-2026:
- Essential: customer uses/buys a top-mounted sink separately;
- Advance/Signature: sink may be selected/ordered;
- taps are NOT supplied/ordered at launch;
- a tap hole/cut-out may still be prepared.

This distinction must survive comparison, process copy, FAQ, CTA copy and every localized version.

## 3.7 Precision-work wording
Safe:
`Het precieze zaag- en freeswerk wordt vooraf gedaan op basis van de opgegeven maten en gekozen uitsparingen.`

Safe:
- measurement choices matter;
- the customer still places/connects the worktop;
- working with two people may be advised.

Do not claim:
- every imaginable cut-out;
- that no drilling/adjustment can ever be needed;
- fixed installation duration;
- an installation service.

## 3.8 Price and delivery
### Price
Allowed:
- explain that price becomes visible in the retailer configuration/order flow.

Forbidden:
- generic consumer price;
- `vanaf` price;
- compare series by price;
- transfer Essential's price to Advance/Signature.

### Delivery
Forbidden:
- one generic delivery promise;
- any delivery time for Advance/Signature.

Live retailer lead-time information remains retailer/live-state information and does not become a CanDo-wide product promise.

## 3.9 Link decisions
All destinations come from the target locale sitemap plus live verification.

Preferred functional relationships:
- UP: Hout op Maat parent/equivalent, if valid;
- SIDEWAYS: W3-style comparison/choice content, only if it actually exists;
- FORWARD: retailer selection/configuration;
- SECONDARY: worktop sample service, only if exact local destination is valid.

Forbidden:
- fabricated choice-help URL;
- fabricated sample URL;
- known redirect URL as final link;
- NL URL copied into BE;
- FAB/no-name route presented as the CanDo three-series proposition.

## 3.10 Page-specific prohibitions
In addition to `05-CLAIMS-POLICY.md`:
- no new parallel owner page;
- no reviews/stars/Trustpilot product proof;
- no full 25-decor tile grid;
- no massief-hout claim for these series;
- no broad comparison with ceramic, Dekton, granite etc.;
- no assortmentsbrede FSC claim;
- no unconfirmed norm numbers;
- no unsupported maximum dimensions for Advance/Signature;
- no direct configurator/retailer URL unless locale-verified.

## 3.11 CTA
Primary:
`retailer choice / configuration` in locally natural wording.

NL working label:
`Stel je werkblad samen`

The localized specialist is allowed to choose a different locally stronger commercial CTA if meaning and route stay the same.

Secondary:
sample CTA only when the worktop sample service is valid in that locale.

## 3.12 Measurement
Primary:
outgoing retailer click, split by retailer/route where possible.

Secondary:
- retailer configuration click;
- sample request;
- comparison/decision interaction.

Never call pageviews, rankings or impressions the final business result.
A click-out is also not a sale.

---

## 4. Cross-market localization rules for this page

### NL
Build source version first and pass source QA.

### BE-NL
Do not translate NL copy line by line.
Rebuild from decision task + product truth + Belgian search vocabulary + BE-NL sitemap.
The internal-link set may differ from NL.

### BE-FR
Do not translate Dutch syntax into French.
Rebuild commercially in natural Belgian French from the same decision task and product truth.
Search language, headings, CTA and links are market decisions.
`plan de travail` is a category anchor, not a command to translate every Dutch term literally.

The localization specialist performs three silent refinement passes before output.

---

## 5. Benchmark blockers / open items
These do not block the NL build unless the page requires the fact, but they must not be guessed:
- Advance maximum dimensions;
- Advance delivery time;
- Signature delivery time;
- final sample-service URL per locale;
- final launch date;
- any separate Karwei page decision.

Locale build blocker:
- missing locale sitemap.

---

## 6. Build order
1. Root + orchestrator.
2. Product truth / claims.
3. Brand + audience.
4. Keyword map + this workbook.
5. Target locale sitemap(s).
6. Stramien.
7. NL BUILD.
8. NL source QA.
9. Commercial localization.
10. Locale QA summary.
11. Human review.
