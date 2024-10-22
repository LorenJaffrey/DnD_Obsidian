---
tags:
---
# `=this.file.name`

```dataview
TABLE WITHOUT ID
file.link AS "Feuerwaffe",
"`dice:" + SchadenFern + "\|none\|noform`"  AS "Schaden", 
SchadensartFern AS "Schadensart", 
Range1 AS "Minimalreichweite", 
Range2 AS "Grundreichweite", 
Range3 AS "Maximalreichweite", 
Hände, 
Gewicht, 
Kosten
FROM #Gegenstand/Waffe/Klasse/Feuerwaffe AND !#Gegenstand/Magischer_Gegenstand
```