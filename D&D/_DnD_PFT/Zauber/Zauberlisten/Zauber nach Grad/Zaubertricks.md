---
aliases: Zaubertrick
---
# `=this.file.name`
Ein Zaubertrick kann jederzeit und ohne einen [[Zauberplätze|Zauberplatz]] gewirkt werden. 
Außerdem muss er nicht vorbereitet werden.
Der [[Zaubergrad]] von Zaubertricks ist 0.

```dataview
TABLE WITHOUT ID

file.link AS "Zauber",
Schule, 
Zeitaufwand,
Schaden AS "Schaden ab Lv. 1",
SchadenLv5 AS "Schaden ab Lv. 5",
SchadenLv11 AS "Schaden ab Lv. 11",
SchadenLv17 AS "Schaden ab Lv. 17",
Reichweite, 
choice(Verbal,"X","") AS "Verbal", 
choice(Geste,"X","") AS "Geste", 
choice(Material,"X","") AS "Material", 
choice(Materialkosten, "X", "") AS "Materialkosten", 
Dauer, 
choice(Konzentration,"X","") AS "Konzentration", 
choice(Ritual,"X","") AS "Ritual", 
choice(Skalierbar,"X","") AS "Skalierbar" 

FROM #Zauber

WHERE Grad = 0

SORT grad, file.name
```