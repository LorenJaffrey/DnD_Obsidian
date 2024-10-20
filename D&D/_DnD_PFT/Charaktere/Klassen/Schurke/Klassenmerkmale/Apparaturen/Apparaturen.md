---
aliases:
  - Apparatur
---
# `=this.file.name`

```dataview
TABLE WITHOUT ID

file.link AS "Apparaturen", 
SG,
Stufe,
Einsatz

FROM #Merkmal/Klasse/Schurke/Meistertüftler/Apparatur 

SORT SG, file.name
```