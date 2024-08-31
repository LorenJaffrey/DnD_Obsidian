---
tags:
  - Beruf/Kräuterkunde
aliases:
  - Kraut
---
# `=this.file.name`
```dataview
TABLE WITHOUT ID
file.link AS "Kraut",
Art,
Effekt.Roh AS "Effekt Roh",
Effekt.Verarbeitet AS "Effekt Verarbeitet"
FROM #Beruf/Kräuterkunde/Zutat
WHERE file.name != "Vorlage Kräuterkunde-Zutat"
SORT Art, file.name
```