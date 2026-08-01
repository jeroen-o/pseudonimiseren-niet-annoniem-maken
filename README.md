# Pseudonimisator v6.1

Vervang persoonsgegevens in teksten, Word-bestanden, PDF's, e-mails en spreadsheets door tokens vóórdat je een dossier gebruikt in een AI-tool — volledig lokaal in de browser, zonder dataverzending. Inclusief foto's/PDF's blurren, documentvergelijker, Word-herstel en een ingebouwd deelbaar-stoplicht.

## Functies in het kort

- **Pseudonimiseren**: automatische herkenning van BSN (elfproef), IBAN (mod-97), e-mail, telefoon, adres/postcode/Postbus, kenteken, KvK, datums en namen (aanhef, initialen, eigen lijst, suggesties); eigen regex-patronen voor polis-/dossiernummers
- **Invoer**: plakken, .txt, Word (.docx), PDF (met OCR-optie voor scans), e-mail (.eml, incl. kop en bijlage-signalering), Excel/CSV (kolomgestuurd)
- **Uitvoer**: .txt, Word met behoud van opmaak (incl. kop-/voetteksten, voetnoten, hyperlinks; metadata-stripper en tracked-changes-opschoning), Excel/CSV, ZIP-batch — alle met gepseudonimiseerde bestandsnamen
- **Sleutel**: per dossier (met dossierlabel), optioneel AES-256-versleuteld met wachtwoord; vervolgdossiers hergebruiken bestaande tokens
- **Controle**: visuele tokenweergave, vals-positieven uitsluiten, context-scanner (incl. bijzondere persoonsgegevens art. 9 AVG), deelbaar-stoplicht, verwerkingsverslag, ingebouwde zelftest en praktijkvoorbeeld
- **Terugzetten**: tekst én Word-bestanden, met sleutelbeheer (wachtwoord wijzigen/toevoegen/verwijderen)
- **Vergelijken**: origineel naast AI-versie met verschillen op regel- en woordniveau
- **Foto's & PDF blurren**: pixeleren/blur/zwart balkje, EXIF-verwijdering, PDF-redactie via rasteren (afgedekte tekst bestaat écht niet meer)

## Installatie op GitHub Pages

1. Maak een nieuw repository (bijv. `pseudonimisator`) en upload `index.html`
2. Ga naar **Settings → Pages**, kies **Deploy from a branch**, selecteer `main` / root en sla op
3. Na ± 1 minuut staat de tool op `https://<gebruikersnaam>.github.io/pseudonimisator/`

## Insluiten in Google Sites

Invoegen → **Insluiten** → **Via URL** → plak de GitHub Pages-URL. Kies volledige breedte en een ruime hoogte (1400–1800 px). Gebruik de URL-variant, niet "Code insluiten". Alle functies — inclusief de wachtwoorddialogen — werken in het iframe (v6.1 gebruikt eigen dialoogvensters in plaats van browser-pop-ups).

## Lokaal gebruiken

Klik rechtsboven in de tool op **⬇ Tool downloaden** en sla het bestand op; dubbelklikken opent het in elke moderne browser. Plakken en .txt werken volledig offline. Voor Word/PDF/Excel/OCR/PDF-uitvoer worden bij eerste gebruik opensourcebibliotheken (mammoth, pdf.js, JSZip, SheetJS, jsPDF, Tesseract) van cdnjs geladen — dat vereist eenmalig internet, maar er wordt nooit documentinhoud verzonden.

## Belangrijk (AVG)

Gepseudonimiseerde gegevens blijven **persoonsgegevens** zolang de sleutel bestaat; de AVG is onverkort van toepassing (standpunt Autoriteit Persoonsgegevens). De detectie is patroongebaseerd en indicatief: context kan iemand herleidbaar houden — zie het ingebouwde praktijkvoorbeeld in de tab "Uitleg & AVG". De eindcontrole en de verantwoordelijkheid voor het delen liggen altijd bij de gebruiker. Deze tool is een hulpmiddel, geen juridisch advies.

## Feedback

Opmerkingen, suggesties of een document waar de tool op vastloopt? Mail jeroen.oversteegen@blinqx.tech

## Zelftest

Open de tab **Uitleg & AVG** en klik op **Zelftest uitvoeren** — de tool controleert zichzelf (elfproef, IBAN, detectie, roundtrip, versleuteling) en rapporteert groen/rood.
