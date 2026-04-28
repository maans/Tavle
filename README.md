# Interaktiv Tavle

Browserbaseret tavleværktøj til undervisning.

## Funktioner

- Flere tavler
- Tekst, video, tegning, timer, billeder, links og PDF
- Lokale PDF-filer og billeder kan indlejres i backup
- Indlejrede PDF’er og billeder kan downloades igen
- Lykkehjul til tilfældige valg
- Gruppeværktøj med tilfældig gruppedannelse
- Gemte lister til både hjul og grupper
- Præsentationstilstand
- JSON-backup og selvstændig HTML-kopi

## PDF og medier

Lokale billeder og lokale PDF-filer kan indlejres i tavledata som data-URL. Det betyder, at de følger med i **Gem som fil** og i JSON-backup, så tavlen kan åbnes på en anden maskine.

Indlejrede medier kan hentes ud igen:

- PDF-widget: **Download PDF**
- Billed-widget: **Download billede**
- Backup-dialog: **Download indlejrede medier**

Baggrundsbilleder indgår også i “Download indlejrede medier”, hvis de er indlejret.

Bemærk: store PDF’er og store billeder kan gøre backupfilen meget stor og kan fylde browserens lokale lager. Til meget store PDF’er kan et eksternt link være bedre.

## Backup

Brug **Gem som fil** til en selvstændig HTML-kopi.

Brug **Eksportér projektfil JSON** til backup og **Importér JSON** til at hente den ind igen. JSON-backup indeholder tavledata, gemte hjul-/gruppelister og indlejrede lokale medier.

## GitHub Pages

Hovedfilen skal hedde `index.html`.

Live-version:

https://maans.github.io/Tavle/
