# Locale link inputs

The workflow expects these normalized runtime files:
- `sitemap-nl.csv`
- `sitemap-be-nl.csv`
- `sitemap-be-fr.csv`

The repository currently contains the original RTF sitemap exports, but these are source material, not the normalized runtime link universe.

If a requested locale CSV is absent, return `NOT READY` for that locale. Never invent or translate URL slugs.
