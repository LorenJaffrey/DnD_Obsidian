---
aliases:
tags:
  - Zauber
Grad: 3
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Bonusaktion]]"
Reichweite: Selbst
Verbal: true
Geste: false
Material: false
Materialkosten: 
Dauer: 1 Minute
Konzentration: true
Ritual: false
Skalierbar: false
Schaden: 3W8
Schadensart: [[Gleißender Schaden]]
Ziel: 
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Das nächste Mal, wenn du innerhalb der Wirkungsdauer des Zaubers eine Kreatur mit einer Nahkampfwaffe triffst, lodert deine Waffe in hellem Licht auf und verursacht beim Ziel zusätzlich 3W8 gleißenden Schaden. Außerdem muss ihm ein Konstitutionsrettungswurf gelingen, um nicht für die Wirkungsdauer zu erblinden. Eine Kreatur, die durch diesen Zauber geblendet wurde, darf am Ende jedes ihrer Züge einen weiteren Konstitutionsrettungswurf ablegen. Bei einem Erfolg verliert sie den Zustand blind.