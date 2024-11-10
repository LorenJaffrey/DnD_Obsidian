---
aliases: 
tags:
  - Zauber/Offensiv
Grad: 2
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Bonusaktion]]"
Reichweite: selbst
Verbal: true
Geste: false
Material: false
Materialkosten: 
Dauer: 1 Minute
Konzentration: true
Ritual: false
Skalierbar: true
Schaden: 2d6
Schadensart: "[[Gleißender Schaden]]"
Ziel: Einzel
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Das nächste Mal, wenn du innerhalb der Wirkungsdauer des Zaubers eine Kreatur mit einer Nahkampfwaffe triffst, leuchtet deine Waffe mit astralem Schein auf und verursacht beim Ziel zusätzlich 2W6 gleißenden Schaden. Das Ziel wird sichtbar, wenn es zuvor unsichtbar war, und
gibt in einem Radius von 1,50 m dämmriges Licht ab. Es kann nicht unsichtbar werden, bis der Zauber endet.

## Auf höheren Graden
Wenn du diesen Spruch mit einem Zauberplatz des 3. oder eines höheren Grades wirkst, steigt der Schaden für jeden Grad über den 2. hinaus um 1W6.