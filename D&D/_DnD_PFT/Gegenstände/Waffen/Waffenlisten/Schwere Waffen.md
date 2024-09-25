---
aliases: Schweren Waffen
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
FROM #Gegenstand/Waffe/Klasse/Nahkampfwaffe
WHERE contains(Eigenschaften, "Schwer")
```