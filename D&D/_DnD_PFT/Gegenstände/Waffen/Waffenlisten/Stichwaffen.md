---
tags:
---
# `=this.file.name`

```dataview
TABLE WITHOUT ID
file.link AS "Waffe",
"`dice:" + Schaden + "\|none\|noform`"  AS "Schaden",
Schadensart, 
Hände, 
Größe, 
Eigenschaften
FROM #Gegenstand/Waffe/Art/Stichwaffe AND #Gegenstand/Waffe/Klasse/Nahkampfwaffe 
SORT größe, file.name
```