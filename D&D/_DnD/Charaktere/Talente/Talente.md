---
aliases:
  - Talent
---
# `=this.file.name`

Solltest du jemals die Voraussetzungen für ein Talent nicht mehr erfüllen, kannst du es so lange nicht nutzen, bis du diese wieder erfüllst.

## Übersicht

```dataview
TABLE WITHOUT ID 
file.link AS "Talent", Stufe, Voraussetzungen, choice(Wiederholbar,"X","") AS "Wiederholbar", aliases AS "Alias"
FROM #Talent
SORT Stufe, file.name ASC
```