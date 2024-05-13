---
tags:
- Beruf/Kräuterkunde/Umgebung
---

# `=this.file.name`

```dataview
TABLE WITHOUT ID
file.link AS "Pflanze",
aliases,
Art,
Effekt.Roh AS "Effekt Roh",
Effekt.Verarbeitet AS "Effekt Verarbeitet",
AnzahlDosenFürVerarbeitung AS "Dosen",
VerarbeitungsSG AS "SG"
FROM #Beruf/Kräuterkunde/Zutat
WHERE file.name != "Vorlage Kräuterkunde-Zutat"
AND contains(Umgebungen, "Grasland")
SORT Art, file.name
```