---
aliases:
tags:
  - Zauber/Offensiv
Grad: 3
Schule: "[[Verwandlungszauber|Verwandlung]]"
Zeitaufwand: "[[Bonusaktion]]"
Reichweite: selbst
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: 1 Minute
Konzentration: true
Ritual: false
Skalierbar: true
Schaden: 4W8
Schadensart: "[[Blitzschaden]]"
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
Das nächste Mal, wenn du innerhalb der Wirkungsdauer des Zaubers eine Kreatur mit einer Fernkampfwaffe angreifst, verwandelt sich das Geschoss oder die Waffe selbst (im Falle einer Wurfwaffe) in einen Blitz. Führe einen normalen Angriffswurf aus. Das Ziel erleidet bei einem Treffer 4W8 Blitzschaden oder halb so viel Schaden, wenn du verfehlst. Dies ersetzt den Waffenschaden. Gleichgültig ob du triffst oder verfehlst, muss jede Kreatur innerhalb von 3 m um das Ziel einen Geschicklichkeitsrettungswurf ablegen. Bei einem Misserfolg erleidet die entsprechende Kreatur 2W8 Blitzschaden oder halb so viel Schaden bei einem erfolgreichen Rettungswurf. Das Geschoss oder die Waffe nimmt anschließend wieder seine ursprüngliche Form an.

## Auf höheren Graden
Wenn du diesen Spruch mit einem Zauberplatz des 4. oder eines höheren Grades wirkst, steigt der Schaden beider Zaubereffekte für jeden Grad über den 3. hinaus um 1W8.