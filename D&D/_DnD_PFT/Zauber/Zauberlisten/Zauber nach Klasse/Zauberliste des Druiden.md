---
aliases:
  - Druidenzauber
---

# `=this.file.name`

```dataview
TABLE WITHOUT ID

file.link AS "Zauber",
Grad,
Schule,
Zeitaufwand, 
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

WHERE contains(Klassen, [[Druide]])

SORT grad, file.name
```