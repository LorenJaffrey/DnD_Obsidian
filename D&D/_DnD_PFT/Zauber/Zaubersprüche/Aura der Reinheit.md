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
Reinigende Energie strahlt von dir aus und erschafft eine Aura mit 9 m Radius. Bis der Zauber endet, bewegt sich die Aura mit dir als Mittelpunkt fort. Alle nicht feindlichen Kreaturen innerhalb der Aura (inklusive dir selbst) können nicht krank werden, erhalten eine Resistenz gegen Giftschaden und sind im
Vorteil bei Rettungswürfen gegen Effekte, die folgende Zustände auslösen: betäubt, bezaubert, blind, gelähmt, taub, verängstigt und vergiftet.