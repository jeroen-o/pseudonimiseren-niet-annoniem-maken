# Versiegeschiedenis

## v6.2
- Naamvarianten: een ingevoerde naam dekt automatisch voornaam, achternaam met tussenvoegsels, samengestelde en koppelteken-varianten
- Voornamenlijst uitgebreid naar 2.300+ Nederlandse voornamen (suggesties)
- Ingebouwde detectie van polis-, dossier-, klant-, contract- en offertenummers (met context) en IP-adressen
- Automatische roundtrip-controle na elke verwerking, zichtbaar in het stoplicht
- Sleutel-documentmatch bij terugzetten: waarschuwing wanneer een sleutel vermoedelijk niet bij het document hoort
- Extra Word-risicodekking: verplaatste tekst (moveFrom/moveTo), people.xml-auteursgegevens en de documentthumbnail worden opgeschoond; thumbnail telt mee in de mediadetectie

## v6.1
- In-page dialoogvensters in plaats van browser-pop-ups: alle functies (incl. sleutelwachtwoorden) werken nu ook in een Google Sites-iframe
- Knop "Tool downloaden" om het HTML-bestand op de eigen pc te zetten

## v6.0
- Word-bestand terugzetten met behoud van opmaak
- Documentvergelijker (regel- en woordniveau)
- PDF blurren via rasteren (veilige redactie)
- Ingebouwde zelftest (9 tests)
- Dossierlabel in sleutel, bestandsnamen en verslag
- Hyperlinks (mailto/URL) in Word gepseudonimiseerd; Excel-tabbladnamen vervangen; Postbus-detectie
- Signalering van afbeeldingen in Word en e-mailbijlagen (stoplicht)

## v4.0
- Gepseudonimiseerde bestandsnamen (ook in ZIP en verslag)
- Word-metadata-stripper en tracked-changes-opschoning (met detectie bij laden)
- Deelbaar-stoplicht (groen/oranje/rood eindcheck)
- Excel/CSV kolomgestuurd pseudonimiseren

## v3.x
- Vervolgdossiers: bestaande sleutel aanvullen met consistente tokens
- E-mail (.eml) als invoer, incl. kopregels
- Achternaam- en straatnaamsuggesties; huisnummer-referenties ("nr 15")
- Context-scanner incl. bijzondere persoonsgegevens (art. 9 AVG), woonduur, leeftijd, plaatsnamen
- Verwerkingsverslag; ingebouwd praktijkvoorbeeld met uitleg

## v2.0
- Aanhef- en initiaaldetectie; genitief; KvK met context; datums voluit
- Vals-positieven uitsluiten met één klik; batchverwerking; ZIP
- Word-uitvoer met behoud van opmaak; OCR voor gescande PDF's
- Sleutelversleuteling (AES-256-GCM) en sleutelbeheer
- Foto's blurren met EXIF-verwijdering; handleiding in de tool

## v1.0
- Basisdetectie (BSN met elfproef, IBAN met mod-97, e-mail, telefoon, adres, postcode, kenteken)
- Tokens met sleutel; visuele controle; voornamensuggesties; terugzetten
