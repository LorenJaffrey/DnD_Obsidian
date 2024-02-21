---
aliases: 
- Hervorrufung
---
# `=this.file.name`
Manipulieren magische Energiequellen mit einer Vielzahl von Effekten. Manche erzeugen Feuerblitze, andere kanalisieren positive Energie um Wunden zu heilen.

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

WHERE contains(Schule, [[Hervorrufungszauber]])

SORT grad, file.name
```