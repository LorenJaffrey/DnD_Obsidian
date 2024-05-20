---
aliases: 
  - Mittelschwerer Rüstung
tags:
  - Gegenstand/Rüstung
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
FROM #Gegenstand/Rüstung/Mittel
SORT RP, SR
```