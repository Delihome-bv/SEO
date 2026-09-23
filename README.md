# Deli Home SEO AI workspace

Shared repository for CanDo SEO/content work with Claude Code and GitHub Copilot.

## Start here
- `CLAUDE.md`: shared always-on instructions.
- `00-ROOT.md`: source governance and routing.
- `.github/agents/seo-orchestrator.agent.md`: Copilot end-to-end orchestrator.
- `.claude/agents/`: specialist agents reusable by Claude Code and VS Code Copilot.
- `.claude/skills/`: portable workflows.

## Canonical knowledge
The numbered Markdown/CSV files in the repository root are controlled sources. Example HTML files are working artifacts, not product truth.

## Runtime dependencies
- Page structure: `05-STRAMIEN/stramien-landingspagina-v6.html`
- Locale URLs: `07-LINKS/sitemap-nl.csv`, `sitemap-be-nl.csv`, `sitemap-be-fr.csv`
- Retailer eligibility: `07-RETAILER-ROUTES.csv`

The normalized sitemap CSVs are currently still missing. That is a deliberate hard stop: do not invent locale URLs from the RTF exports.
