# Orchestrator — Worktop Page Benchmark

## Phase 1 — PREPARE
Classify brand, task, source market and requested target markets.

Gate 0 requires:
- owner page and page role;
- product truth;
- claims policy;
- target-locale sitemap for each requested locale;
- stramien.

If a requested locale sitemap is missing, that locale is NOT READY.

## Phase 2 — RESEARCH / RESOLVE — NL SOURCE
Required:
1. open the current NL owner page;
2. run exact search `werkbladen op maat`;
3. inspect at least three relevant organic results if technically possible;
4. validate NL links against `07-LINKS/sitemap-nl.csv` and live web;
5. log date and URLs.

## Phase 3 — BUILD NL
Use `skills/seo-page-build/SKILL.md`.
The stramien owns structure/layout. The content workbook owns page job. Product truth and claims own facts.

## Phase 4 — VALIDATE NL
Use `skills/source-quality-qa/SKILL.md`.
If QA returns NEEDS_FIX: correct once and run QA once more.
Only an approved NL source version may be localized.

## Phase 5 — LOCALIZE
For BE-NL and/or BE-FR invoke `skills/commercial-localization/SKILL.md`.
The specialist uses approved meaning, not sentence-by-sentence translation, researches local search wording where needed, uses the local sitemap and performs three internal refinement passes.

## Phase 6 — LOCALE HANDOFF CHECK
Per locale verify:
- all internal links against locale sitemap;
- no product fact changed;
- natural commercial language;
- local search terminology;
- no NL-only URL or wording leaked through.

## Phase 7 — HANDOFF
Return NL source package, requested localized packages, decision log, source QA, localization QA summaries, unresolved items and READY FOR HUMAN REVIEW / NOT READY by locale.

No publish step exists.
