---
name: commercial-localization
description: Localizes an approved CanDo NL source page for BE-NL or BE-FR using native commercial language, local search terminology, target-locale sitemap links and valid retailer routes while keeping product truth invariant. Use only after source QA passes.
---
# Commercial Localization

## Required inputs
Read:
- ../../../00-ROOT.md
- ../../../02-BRAND.md
- ../../../03-AUDIENCE.md
- ../../../04-PRODUCT-TRUTH.md
- ../../../05-CLAIMS-POLICY.md
- ../../../06-CONTENT-WORKBOOK.md
- ../../../07-CONTENT-ARCHITECTURE.md
- ../../../07-RETAILER-ROUTES.csv
- ../../../08-LOCALE-RULES.md
- ../../../08-SEO-GEO-RULES.md
- the approved NL source;
- the target locale sitemap in ../../../07-LINKS/.

## Procedure
1. Do not localize an NL source that has not passed source QA.
2. Select only retailer routes valid for the target locale and proposition, then validate URLs against that locale's sitemap/live state.
3. Rebuild from approved meaning, never line by line.
4. Re-evaluate local search wording, headings, metadata and CTA language.
5. Preserve every product fact, claim status and series distinction.
6. Perform three silent refinement passes: meaning/claims, native commercial fluency, then local SEO/CTA/routes.
7. Return the final localized version plus a concise localization QA summary and unresolved items.

Never replace a missing Belgian route with a French retailer. Never translate URL slugs. Never invent a local route.
