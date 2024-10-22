---
aliases: Einfache Waffe, Einfachen Waffe, Einfachen Waffen
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
FROM #Gegenstand/Waffe/Kategorie/Einfache_Waffe AND #Gegenstand/Waffe/Klasse/Nahkampfwaffe AND !#Gegenstand/Magischer_Gegenstand
```