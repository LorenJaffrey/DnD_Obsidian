---
aliases:
tags:
  - Zauber/Offensiv
Grad: 1
Schule: "[[Beschwörungszauber|Beschwörung]]"
Zeitaufwand: "[[Bonusaktion]]"
Reichweite: Selbst
Verbal: true
Geste: false
Material: false
Materialkosten: 
Dauer: 1 Minute
Konzentration: true
Ritual: false
Skalierbar: true
Schaden: 1W10
Schadensart: "[[Stichschaden]]" 
Ziel: AoE
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Das nächste Mal, wenn du innerhalb der Wirkungsdauer des Zaubers eine Kreatur mit einer Fernkampfwaffe triffst, verwandelt sich das Geschoss oder die Waffe selbst (im Falle einer Wurfwaffe) in cinen Hagel aus Dornen. Neben dem normalen Effekt des Angriffs müssen das Ziel und alle Kreaturen innerhalb von 1,50 m um dieses einen Geschicklichkeitsrettungswurf ablegen. Bei einem Misserfolg erleidet eine Kreatur 1W10 Stichschaden oder halb so viel Schaden bei einem erfolgreichen Rettungswurf.

## Auf höheren Graden
Wenn du diesen Spruch mit einem Zauberplatz des 2. oder eines höheren Grades wirkst, steigt der Schaden für jeden Grad über den 1. hinaus um 1W10 (maximal 6W10).