# Bynder: van asset id naar een werkende beeld-URL

**Opgeschreven 11-09-2026.** Dit stond nergens in de SEO-map. Een agent leidde het af door het kopcommentaar van stramien 32 naast zijn eigen `<img src>` te leggen. Dat is reverse-engineering, geen documentatie.

## De bron

`Desktop/Marketingplan/Strategie mijn Scope/Beeld/Meta_data_beeld_cando_*.csv`, **1.612 assets**. Let op: dat is **niet** Desktop-niveau, dat pad stond tot 11-09 fout in `CLAUDE.md`.

## Het recept

De CSV levert een asset id in het formaat **8-4-4-16** zonder het laatste streepje:

```
BEBDCC45-695A-4E6F-A793F7430414A8C7
```

De site wil **kleine letters** en het **volledige 8-4-4-4-12-patroon**:

```
bebdcc45-695a-4e6f-a793-f7430414a8c7
```

Dus: alles naar kleine letters, en zet een streepje na de vierde tekengroep van het laatste blok.

**De volledige URL:**

```
https://delihome.getbynder.com/asset/<uuid>/medium-JPG/<Title-met-streepjes>.jpg
```

De `Title` uit de CSV, met spaties vervangen door streepjes.

## Twee regels die erbij horen

1. **Test elke URL op HTTP 200 voordat hij de pagina in gaat.** Een asset id in de CSV garandeert niet dat de afgeleide URL resolvet.
2. **De bestandsnaam is geen beschrijving.** Open het beeld en kijk ernaar voordat je een alt-tekst schrijft. Een agent schreef op 11-09 bijna een alt-tekst over "een strakke naad tussen twee delen" voor een foto die hij niet had bekeken.

## Het beeldregister, en waarom het nu niet werkt

De regel is: gebruikte asset-id's registreer je in tab `06` van `CanDo-hout-redirects-en-inventaris.xlsx`, zodat dubbelgebruik onmogelijk wordt.

⛔ **Maar die tab is vanuit de bouw niet leesbaar.** Een agent die wil weten welk beeld al gebruikt is, moet dit doen:

```bash
grep -rho 'getbynder.com/asset/[0-9a-f-]*' "CanDo SEO/cando-stramienen/" | sort -u
```

Dat werkt, maar het is toeval dat het werkt. **Openstaand: een leesbaar beeldregister** (asset id naar stramien) naast de Excel, zodat de bouw niet hoeft te grep'en.
