---
aliases:
  - 
tags:
  - Zauber
Grad: 4
Schule: "[[Bannzauber|Bannmagie]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Selbst (9 Meter)
Verbal: true
Geste: false
Material: false
Materialkosten: 
Dauer: 10 Minuten
Konzentration: true
Ritual: false
Skalierbar: false
Schaden: 
Schadensart: 
Ziel: 
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer:  1 Runde

## Beschreibung
Lebenserhaltende Energie entströmt dir und erschafft eine Aura mit 9 m Radius. Bis der Zauber endet, bewegt sich die Aura mit dir als Mittelpunkt fort. Alle nicht feindlichen Kreaturen innerhalb der Aura (inklusive dir selbst) erhalten eine Resistenz gegen nekrotischen Schaden, außerdem können ihre maximalen Trefferpunkte nicht verringert werden. Zusätzlich erlangen nicht feindliche, lebende Kreaturen 1 Trefferpunkt zurück, wenn sie ihren Zug in der Aura beginnen und 0 Trefferpunkte besitzen.