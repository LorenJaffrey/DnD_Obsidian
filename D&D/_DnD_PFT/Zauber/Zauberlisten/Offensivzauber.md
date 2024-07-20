# `=this.file.name`

```dataview
TABLE WITHOUT ID

file.link AS "Zauber",
Grad, 
Schule, 
Zeitaufwand, 
Reichweite,
Schaden,
Schadensart,
Ziel,
choice(Verbal,"X","") AS "Verbal", 
choice(Geste,"X","") AS "Geste", 
choice(Material,"X","") AS "Material", 
choice(Materialkosten, "X", "") AS "Materialkosten", 
Dauer, 
choice(Konzentration,"X","") AS "Konzentration", 
choice(Ritual,"X","") AS "Ritual", 
choice(Skalierbar,"X","") AS "Skalierbar" 

FROM #Zauber/Offensiv

SORT grad, file.name
```