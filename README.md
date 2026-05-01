# Interaktiv Tavle


## v141 REN

Bygget fra v141-basen med minimal patch: backup er tilføjet direkte til den faktiske Mere-menu (`data-more-tool`) og hjælp lytter nu både på `data-tool` og `data-more-tool`. Hovedtoolbar er kompakt og backup skjules derfra.


## v141

`?`-knappen kalder nu den eksisterende `showQuickHelp()` direkte via appens egen `handleTool(t)`. Tidligere eksterne hjælp-overlay/listeners er fjernet.
