# Interaktiv Tavle

Et enkelt, browserbaseret tavleværktøj til undervisning. Appen er lavet som én HTML-fil og kan bruges direkte fra GitHub Pages eller downloades til lokal/offline brug.

Live-version:

https://maans.github.io/Tavle/

## Hvad kan appen?

Appen giver en digital undervisningstavle med flere tavler og flytbare widgets.

### Widgets

- **Tekst** – skriv noter, spørgsmål og instruktioner
- **Video** – indsæt video/YouTube-link
- **Tegn** – tegn og annotér på tavlen
- **Hjul** – lykkehjul til tilfældige valg
- **Grupper** – lav tilfældige grupper fra en liste
- **Timer** – nedtælling med alarm
- **Billede** – indsæt billeder fra fil eller URL
- **Link** – klikbare links
- **PDF** – vis eller link til PDF-materiale
- **Baggrund** – vælg farve eller billede
- **Grid** – vis/skjul hjælpelinjer
- **Linje** – geometriske linjer/markeringer
- **Backup** – gem, hent og eksportér

## Tavler

- Opret nye tavler med **+ tavle**
- Skift tavle med pile, tastatur eller swipe
- Brug **Tavler**-oversigten, når der er flere tavler
- Omarrangér og slet tavler i tavleoversigten

## Hjul

Lykkehjulet kan bruges til meget andet end elevnavne:

- elever
- emner
- spørgsmål
- grupper
- fordybelsesområder
- opgaver

Du kan gemme og hente lister, så de kan genbruges.

## Grupper

Gruppeværktøjet bruger samme type lister som lykkehjulet.

Arbejdsgang:

1. Indsæt eller hent en liste
2. Vælg antal personer pr. gruppe
3. Tryk **Dan grupper**
4. Listen skjules automatisk, så grupperne får mest mulig plads
5. Grupperne vises i kolonner, og hjulet forbliver synligt i præsentationstilstand
6. Tryk **Vis/rediger liste**, hvis listen skal ændres

Formålet er, at eleverne tydeligt kan se, at grupperne dannes tilfældigt og fair.

## Præsentationstilstand

Præsentationstilstand giver en renere visning til eleverne:

- færre værktøjsknapper
- tekstfelter kan ikke redigeres
- tavletitlen er stadig synlig
- fokus på indholdet
- gruppehjulet og gruppeoversigten kan stadig vises

## Værktøjslinje og pin

Pinknappen nederst bruges som hurtigkontakt:

- klik én gang: værktøjslinjen holdes synlig
- klik igen: automatisk skjul slås til igen

Kontrolpanelet kan stadig bruges til finere indstillinger, fx hvor længe værktøjslinjen skal være synlig før automatisk skjul.

## Gem og backup

Appen gemmer automatisk i browserens `localStorage`.

Det betyder, at data ligger lokalt i den browser/enhed, du bruger. Lav derfor backup, hvis du vil være sikker.

### Gem som fil

Laver en selvstændig HTML-fil med tavler, widgets, lister og indlejrede billeder.

Det er den praktiske “alt i én”-kopi.

### JSON

JSON er teknisk backup/import.

Brug:

- **Eksportér projektfil JSON**
- **Importér JSON**

`Åbn fil` er fjernet, fordi JSON-import er den mest stabile måde at hente tavledata ind igen.

### Hent tom app

Downloader nyeste ZIP fra GitHub:

https://github.com/maans/Tavle/archive/refs/heads/main.zip

## Lokal brug

Download `index.html` og åbn filen i en browser.

På iPad fungerer appen bedst i Safari eller Chrome. Appen kan også bruges via GitHub Pages.

## GitHub Pages

For at udgive appen:

1. Upload `index.html` til repository
2. Gå til **Settings → Pages**
3. Vælg branch `main`
4. Vælg mappe `/root`
5. Åbn GitHub Pages-linket

GitHub Pages forventer normalt, at hovedfilen hedder:

```text
index.html
```

## Status

Appen er i løbende udvikling og tilpasses praktisk undervisningsbrug.
