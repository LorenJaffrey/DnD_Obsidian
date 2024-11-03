---
aliases: Schweren Waffen
tags:
  - Liste/Waffen
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
FROM #Gegenstand/Waffe/Klasse/Nahkampfwaffe AND !#Gegenstand/Magischer_Gegenstand
WHERE contains(Eigenschaften, "Schwer")
```