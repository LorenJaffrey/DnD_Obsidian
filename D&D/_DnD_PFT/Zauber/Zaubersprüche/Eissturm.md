---
aliases:
tags:
  - Zauber/Offensiv
Grad: 4
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 90 mr
Verbal: true
Geste: true
Material: true
Materialkosten: einige Tropfen Wasser und eine Prise Staub
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Schaden: 4d6 + 2d8
Schadensart: "[[Kälteschaden]]"
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
Ein Hagel aus felsharten Eisbrocken regnet in einem Zylinder mit 6 m Radius und 12 m Höhe auf die Erde. Der Zylinder ist um einen Punkt in Reichweite zentriert. Jede Kreatur innerhalb des Zylinders muss einen Geschicklichkeitsrettungswurf ablegen. Bei einem Misserfolg erleidet das Ziel 2W8 [[Wuchtschaden]] und 4W6 [[Kälteschaden]] oder halb so viel Schaden bei einem erfolgreichen Rettungswurf. Durch den Sturm gilt der Bereich des Zaubers bis zum Ende deines nächsten Zuges als schwieriges Gelände.

## Auf höheren Graden
Wenn du diesen Spruch mit einem Zauberplatz des 5. oder eines höheren Grades wirkst, steigt der Wuchtschaden für jeden Grad über den 4. hinaus um 1W8.