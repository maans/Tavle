# Interaktiv tavle

En enkel, lokal og iPad-venlig interaktiv tavle til planlægning og præsentation af undervisning.

Appen er lavet som én HTML-fil og kan bruges direkte i browseren via GitHub Pages eller downloades til lokal/offline brug. Den er inspireret af værktøjer som Classroomscreen, men med fokus på et enkelt workflow til undervisning, fordybelsesområder, lodtrækning, tekst, billeder, links, timer og hurtige tavleskift.

## Prøv appen

Live-version:

https://maans.github.io/Tavle/

## Hvad kan appen?

- Opret flere tavler i samme forløb
- Skift mellem tavler med pile, tastatur eller tavleoversigt
- Omdøb, omarrangér og slet tavler i tavleoversigten
- Tilføj widgets:
  - tekst
  - video/link til video
  - tegning/annotering
  - lykkehjul
  - timer
  - billede
  - link
  - PDF-link
- Brug præsentationstilstand med renere visning
- Tegn oven på tavlen i annoteringstilstand
- Gem og hent lister til lykkehjulet
- Flyt widgets mellem tavler
- Gem hele tavlen som en selvstændig HTML-fil
- Lav JSON-backup og importér igen
- Download nyeste tomme app direkte fra GitHub

## Lokal brug

Appen kan bruges på to måder:

### 1. Via GitHub Pages

Åbn:

https://maans.github.io/Tavle/

### 2. Som lokal HTML-fil

Download `index.html` eller den nyeste ZIP-fil fra GitHub, og åbn filen i en browser.

På iPad kan appen bruges i Safari/Chrome. Hvis man arbejder i Quine 2 eller lignende, kan man åbne HTML-filen lokalt og gemme kopier.

## Gem og backup

Appen gemmer automatisk data i browserens `localStorage`.

Det betyder:

- dine tavler ligger lokalt i den browser, du bruger
- data følger ikke automatisk med til en anden browser eller enhed
- hvis browserdata slettes, kan tavlerne forsvinde

Brug derfor backup-funktionerne:

### Gem som fil

Gemmer en selvstændig HTML-fil med tavler, widgets, lister og indlejrede billeder.

Det er den mest praktiske “alt-i-en”-backup.

### Åbn fil

Indlæser en tidligere gemt tavlefil.

### JSON-backup

Teknisk backupformat. Kan være nyttigt, hvis man kun vil gemme projektdata.

## Billeder

Billeder kan indsættes fra:

- lokal fil
- URL

Lokale billeder kan gemmes indlejret i tavlefilen, men store billeder kan gøre filen tung.

Billeder fra URL kræver internetforbindelse og kan blive blokeret af den hjemmeside, billedet ligger på.

## Lykkehjulet

Lykkehjulet kan bruges til andet end elever, fx:

- fordybelsesområder
- spørgsmål
- grupper
- opgaver
- rækkefølger

Man kan gemme og hente lister, og valgte elementer kan flyttes til en valgt-pulje, så de ikke trækkes igen.

## Præsentationstilstand

Præsentationstilstand skjuler redigeringsværktøjer og gør tavlen roligere at vise på projektor/skærm.

Tekstfelter kan ikke redigeres i præsentationstilstand.

## Teknisk

Appen er en statisk HTML-app uden server.

Den bruger:

- HTML
- CSS
- JavaScript
- `localStorage`
- data-URL til indlejrede billeder

Der er ingen login, database eller ekstern backend.

## Installation på GitHub Pages

1. Opret et GitHub-repository
2. Upload `index.html`
3. Gå til **Settings → Pages**
4. Vælg branch `main` og mappe `/root`
5. Åbn den adresse GitHub Pages viser

## Filnavne

GitHub Pages forventer normalt, at hovedfilen hedder:

```text
index.html
```

Hvis filen fx hedder `index.html.html`, vil siden typisk ikke åbne korrekt.

## Bemærkninger

Appen er udviklet iterativt til konkret undervisningsbrug. Den er især optimeret til iPad/touch, men kan også bruges på computer.

Hvis noget opfører sig mærkeligt efter upload af ny version, kan det skyldes gammel browsercache eller gamle data i `localStorage`.
