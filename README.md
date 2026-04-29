# Interaktiv Tavle

En fleksibel, browserbaseret undervisningstavle – samlet i én HTML-fil.

Appen er lavet til hurtig brug i undervisning, hvor man kan samle præsentation, aktiviteter, spørgsmål, medier og små interaktive værktøjer på én tavle.

---

## Hvad kan appen?

Du kan opbygge tavler med forskellige interaktive elementer:

- 📝 Tekst og noter
- 🎥 Video
- ✏️ Tegning
- 🎲 Lykkehjulet
- 👥 Gruppegenerator
- ☁️ Ordsky
- 🙂 Afstemning med emojis og resultatvisning
- ⏱️ Timer
- 🖼️ Billeder og baggrunde
- 🔗 Links
- 📄 PDF-visning

Widgets kan flyttes, skaleres, roteres, låses og placeres frit på tavlen.

---

## Lykkehjulet

Lykkehjulet kan både bruges til klassisk udtrækning, hvor valgte navne/emner fjernes fra puljen, og til opsamling, hvor valg bliver stående i puljen.  
Det gør det muligt at bruge hjulet som input til en ordsky, hvor hyppige valg vises større.

---

## Typiske anvendelser

- elevaktivering
- hurtige afstemninger
- brainstorm og begrebsarbejde
- gruppedannelse
- emneudvælgelse med lykkehjul
- præsentationer i klassen
- undervisningsskabeloner, der kan genbruges

---

## Gem og åbn

Appen bruger tavlefiler til backup og genbrug.

**Fuld tavle** gemmer tavler, widgets, indhold, medier og lister.  
**Kun skabelon** gemmer layout og åbne widgets, men rydder eksempelindhold.

---

## Online version

https://maans.github.io/Tavle/


## Lister fra lykkehjulet

Valgte resultater fra lykkehjulet kan gemmes som en liste og derefter hentes i fx ordsky, grupper eller andre lykkehjul.


## Ordsky / tagcloud

Ordskyvisninger bruger størrelse og vægt til at vise gentagelser. Visningen er designet til at fungere på tavle/projektor, så de vigtigste ord eller valg hurtigt kan aflæses.


## Lykkehjulet og ordskyvisning

I lykkehjulet kan man skifte mellem hjulvisning og ordskyvisning ved at klikke på widgettens titel. I ordskyvisning vises kun selve ordskyen, så den egner sig bedre til præsentation.


## Lykkehjulets visninger

Klik på højre panel med valgte resultater for at skifte til ordskyvisning. Klik på ordskyen for at skifte tilbage til hjulet.


## Lykkehjulets tagcloud

I hjulvisning bruges den lille **tagcloud >**-knap nederst i listen til at skifte visning. I tagcloudvisning bruges **< hjul** til at komme tilbage.


## Tagcloud

Tagcloud-visningen fordeler ordene mere frit i fladen, så den ikke opfører sig som en almindelig liste.


Tagcloud-layoutet er justeret, så ordene fordeles korrekt i fladen.


## Stabilitet

Baggrundsværktøjet og widget-knapper oven på indlejrede medier er strammet op, så videoer og PDF’er ikke blokerer for luk/slet-knapper.


## Billeder

Billed-preview i billedwidgets skaleres til widgettens størrelse, så lokale billeder ikke vises som små thumbnails.


## Baggrundsbilleder

Preview af baggrundsbilleder skaleres nu korrekt i baggrundsdialogen, så billedet fylder preview-ruden i stedet for at blive vist som en lille thumbnail.


## Preview

Billed- og baggrunds-preview bruger nu egentlige billedrammer, så billeder skaleres korrekt på både iPad og computer.


## Preview-fri arbejdsgang

Billeder indsættes direkte i billedwidgetten efter valg. Baggrundsbilleder går direkte til baggrundsindstillinger uden et stort previewfelt i appens dialog.


## Globalt ur

Appen har et globalt ur, der kan vises på alle tavler. Uret kan skifte mellem glas, minimal, scene og analog visning samt vise dato og sekunder.


## Ur

Urmodalen er ryddet op med tydelige rækker, designvalg og preview. Scene-uret er rettet, så det placeres korrekt på tavlen.


## Værktøjslinjen

Skjul og linje er samlet i én synlig pin-knap på hovedværktøjslinjen. Herfra indstilles fastgjort værktøjslinje, automatisk skjul og hvor mange sekunder linjen skal blive stående. Når linjen er skjult, hentes den frem med en særskilt “værktøjer ▲”-knap, så man ikke rammer et værktøj ved et uheld.


## v110

Automatisk skjul af værktøjslinjen er gjort mere stabilt med pointer-, mus- og touch-events. Den særskilte “værktøjer ▲”-knap viser linjen uden at aktivere et værktøj.


## Fokus-mode

Fokus-mode skjuler navigation og værktøjslinje, dæmper tavlen og lader dig fremhæve én widget. Funktionen er touch-first: tap vælger fokus, træk ignoreres, og på iPad afsluttes fokus med den synlige “✕ fokus”-knap.


## Værktøjslinje-fallback

Hvis værktøjslinjen er skjult, kan den hentes frem med knappen “værktøjer ▲”. Som ekstra fallback kan man holde fingeren/musen nede i nederste kant i ca. ét sekund. På computer virker Ctrl/Cmd + punktum også.
