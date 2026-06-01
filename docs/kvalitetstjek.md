# Kvalitetstjek - v48a bedre PDF-skabeloner

De første generiske PDF-skabeloner var teknisk korrekte, men for lidt brugervenlige. I v48a er skabelonerne derfor lavet om til menneskelige lærerark med tabel-layout.

## Ændringer i PDF-skabeloner

* KaPardy-skabeloner bruger liggende A4 og en samlet række pr. spørgsmål.
* Kolonnerne er: Nr., Kategori, Point, Spørgsmål, Rigtigt svar, Forkert 1, Forkert 2 og Forkert 3.
* KaPardy 15, 20, 25 og 30 fordeles over flere sider med samme tabel-layout.
* Afstemning, lykkehjul, ordsky, timer og linkliste bruger også tabeller med korte, læsbare kolonneoverskrifter.
* Grupper-skabeloner bruger navnelister i to kolonner.
* Feltnavnene er stadig stabile og systematiske, men de dominerer ikke længere layoutet.

## Kontrol udført

* `kapardy_05`, `kapardy_10`, `kapardy_15`, `kapardy_20`, `kapardy_25` og `kapardy_30` er kontrolleret med pypdf: de har henholdsvis 35, 70, 105, 140, 175 og 210 KaPardy-felter, svarende til 7 felter pr. spørgsmål.
* `kapardy_10.pdf` er render-testet til PNG og kontrolleret visuelt: layoutet er tabelbaseret, uden klipning eller overlap.
* `linkliste_10_links.pdf` er render-testet som repræsentant for øvrige widgetskabeloner: layoutet er tabelbaseret og læsbart.
* Alle PDF'er er programmatisk genereret som rigtige AcroForm-PDF'er med udfyldelige felter.

## Kendte begrænsninger

PDF-formfelterne er tomme, ikke udfyldt med tekniske placeholder-navne. Det er bevidst, fordi skabelonerne nu skal fungere som lærerark. De tekniske feltnavne findes stadig i formularstrukturen.

KaPardy-spillene uden for temaet Nordisk mytologi er stadig placeholders fra den tidligere pakke og bør ikke betragtes som færdig faglig quizbank.

## v48b – online spilvælger

v48b ændrer spilflowet, så de færdige KaPardy-spil ikke behøver at blive uploadet/importeret som 90 lokale DataWidgets. I stedet læses `docs/manifest_spil.json`, og brugeren vælger først antal spørgsmål og derefter tema/genre. Selve CSV-filen hentes først, når brugeren klikker på et spil.

Nye adgangsveje:

- Fra **KaPardy**: knappen `🌐 Spil` åbner onlinebiblioteket.
- Fra **PDFWidget**: knappen `🏆 Spil` åbner samme bibliotek og kan åbne spillet i PDFWidget, KaPardy eller begge dele.
- Fra **AI-generatoren**: ekstra faneblad/genvej `Færdige spil` åbner samme vælger.
- Fra en lokal KaPardy-kompatibel DataWidget: knappen `📄 PDFWidget` kan åbne data i en passende KaPardy-PDF-skabelon.

Testpunkter for v48b:

1. Onlinebiblioteket viser antal: 5, 10, 15, 20, 25 og 30.
2. Temaer vises først efter valgt antal spørgsmål.
3. CSV-filer hentes først ved klik på tema.
4. Spil kan åbnes i KaPardy uden at importere alle 90 spil.
5. Spil kan åbnes i PDFWidget som udfyldt KaPardy-skabelon.
6. Spil kan åbnes i både KaPardy og PDFWidget.
7. AI-generatorens nye fane/genvej åbner samme spilvælger.
8. Lokale uploadede KaPardy-datawidgets kan stadig vælges og åbnes i PDFWidget.

Kendt begrænsning: Den nye AI-generatoradgang er implementeret som et ekstra faneblad/genvej i den eksisterende AI-modal. Den erstatter ikke hele AI-generatorens interne firetrins-logik, men åbner samme spilbibliotek uden at kopiere eller importere spillene først.


## v48c literal-template-fix

Retter v48b-fejl hvor JavaScript-templateudtryk som `${kahoopardyModeName(currentMode)}` og `${esc(t.ico)}` kunne blive vist direkte i brugerfladen. Fixet er bevidst lille og defensivt: det ændrer ikke PDF-, CSV- eller DataWidget-struktur, men overskriver kun de berørte UI-renderfunktioner og rydder synlige literal-placeholders efter render.
