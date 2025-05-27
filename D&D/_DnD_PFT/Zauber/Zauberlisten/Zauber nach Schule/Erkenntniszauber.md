---
tags:
  - Schule_der_Magie
aliases:
  - Erkenntnis
  - Erkenntnismagie
Typische_Effekte: "Enthüllt Informationen."
---
# `=this.file.name`
`=this.Typische_Effekte`

```dataview
TABLE WITHOUT ID

file.link AS "Zauber",
Grad,
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

WHERE contains(Schule, [[Erkenntniszauber]])

SORT grad, file.name
```