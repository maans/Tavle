# Interaktiv Tavle

Et enkelt, browserbaseret tavleværktøj til undervisning.

## Funktioner

- Flere tavler
- Tekst, video, tegning, timer, billeder, links og PDF
- Lykkehjul til tilfældige valg
- Gruppeværktøj med tilfældig gruppedannelse
- Gemte lister til både hjul og grupper
- Præsentationstilstand
- JSON-backup og selvstændig HTML-kopi

## Hjul og lister

Gemte lister bruges både af lykkehjulet og gruppeværktøjet. JSON-backup indeholder nu også gemte lister, så de kan hentes igen efter import.

## Grupper

1. Hent eller skriv en liste
2. Vælg antal personer pr. gruppe
3. Tryk **Dan grupper**
4. Listen skjules automatisk, så grupperne får plads
5. Hjulet forbliver synligt i præsentationstilstand

## Timer

Timeren tæller ned uden at gemme hele projektet hvert sekund. Det forhindrer gentagne fejlbeskeder, hvis projektet er stort.

## Gem og backup

Appen gemmer automatisk i browserens `localStorage`, men browserens lagerplads kan blive fyldt af store billeder.

Brug derfor:

- **Gem som fil** til en selvstændig HTML-kopi
- **Eksportér projektfil JSON** til backup
- **Importér JSON** til at hente backup ind igen

## GitHub Pages

Hovedfilen skal hedde:

```text
index.html
```

Live-version:

https://maans.github.io/Tavle/
