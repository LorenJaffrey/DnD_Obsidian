# `=this.file.name`
Erhalte Metamagie-Optionen, während du aufsteigst. 
Du kannst einmal pro [[Runde]] eine davon einsetzen.

> [!tip]- Studium! 
> Wann immer du während einer [[Sichere Rast|Sicheren Rast]] arkane Bücher studierst oder von einem höherstufigen Magier unterrichtet wirst, kannst du andere verfügbare Arkanisten-Optionen wählen.﻿

```dataview
TABLE WITHOUT ID

file.link AS "Title",
Einsatz

FROM #Regeln/Nimble/Merkmal/Klasse/Arkanist/Metamagie 

SORT file.name
```