---
aliases:
  - Rüstung
---
# `=this.file.name`

```dataview
TABLE  WITHOUT ID 
file.link AS "Title",
Klasse, 
RP, 
SR, 
Stärke, 
Dex_cap AS "GES Cap", 
Eigenschaften, 
Gewicht, 
Kosten
FROM #Gegenstand/Rüstung
SORT Klasse, RP, SR
WHERE file.name != "Vorlage Rüstung"
AND Klasse
```