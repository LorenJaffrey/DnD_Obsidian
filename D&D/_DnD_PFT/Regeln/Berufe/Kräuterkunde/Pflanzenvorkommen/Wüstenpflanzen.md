---
tags:
  - Beruf/Kräuterkunde/Umgebung
aliases:
  - Wüste
---
# `=this.file.name`
```dataview
TABLE WITHOUT ID
file.name AS "W6",
file.link AS "Pflanze",
Art,
Effekt.Roh AS "Effekt Roh",
Effekt.Verarbeitet AS "Effekt Verarbeitet"
FROM #Beruf/Kräuterkunde/Zutat
WHERE file.name != "Vorlage Kräuterkunde-Zutat"
AND contains(Umgebungen, this.file.link)
SORT file.name
```