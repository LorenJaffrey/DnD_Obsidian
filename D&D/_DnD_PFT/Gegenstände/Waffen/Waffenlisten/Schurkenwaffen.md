---
aliases: Schurkenwaffe
tags:
  - Liste/Waffen
---
# `=this.file.name`

## Nahkampfwaffen
```dataview
TABLE WITHOUT ID
file.link AS "Nahkampfwaffe",
"`dice:" + Schaden + "\|none\|noform`"  AS "Schaden",
Schadensart, 
Kategorie,
Hände, 
Größe, 
Eigenschaften
FROM (#Gegenstand/Waffe/Kategorie/Einfache_Waffe OR (#Gegenstand/Waffe/Kategorie/Kriegswaffe AND ([[Finesse]] OR [[Leicht]]))) AND !#Gegenstand/Magischer_Gegenstand AND #Gegenstand/Waffe/Klasse/Nahkampfwaffe 
SORT Kategorie
```

## Fernkampfwaffen
```dataview
TABLE WITHOUT ID
file.link AS "Fernkampfwaffe",
"`dice:" + SchadenFern + "\|none\|noform`"  AS "Schaden",
SchadensartFern AS "Schadensart", 
Range1 AS "Minimalreichweite", 
Range2 AS "Grundreichweite", 
Range3 AS "Maximalreichweite", 
Kategorie,
Hände,
Gewicht, 
EigenschaftenFern
FROM (#Gegenstand/Waffe/Kategorie/Einfache_Waffe OR (#Gegenstand/Waffe/Kategorie/Kriegswaffe AND ([[Finesse]] OR [[Leicht]]))) AND !#Gegenstand/Magischer_Gegenstand AND #Gegenstand/Waffe/Klasse/Fernkampfwaffe 
SORT Kategorie
```