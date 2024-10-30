---
aliases:
  - Lesser Restoration
tags:
  - Zauber
Grad: 3
Schule: "[[Bannzauber|Bannmagie]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 36 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Schaden: 
Schadensart: 
Ziel: Einzel
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Wähle eine Kreatur, ein Objekt oder einen magischen Effekt in Reichweite. Jeder Zauber des 3. Grades oder niedriger, der auf dem Ziel liegt, endet. Führe für jeden Zauber des 4. Grades oder höher, der auf dem Ziel liegt, einen Attributswurf mit deinem Attribut zum Zauberwirken aus. Der SG ist gleich 10 + der Grad des Zaubers. Bei einem erfolgreichen Wurf endet der Zauber.

## Auf höheren Graden
Wenn du diesen Zauber wirkst, indem du einen Zauberplatz des 4. Grades oder höher nutzt, beendest du automatisch die Effekte von Zaubern, die auf dem Ziel liegen und deren Grad gleich oder niedriger als der Grad des Zauberplatzes ist, den du gerade nutzt.