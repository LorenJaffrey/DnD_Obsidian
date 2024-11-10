---
aliases:
tags:
  - Zauber/Offensiv
Grad: 3
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Selbst (Linie von 30 m)
Verbal: true
Geste: true
Material: true
Materialkosten: ein Stück Fell und ein Stab aus Bernstein, Kristall oder Glas
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Schaden: 8d6
Schadensart: [[Blitzschaden]]
Ziel: Linie
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Ein Blitz in Gestalt einer Linie mit 30 m Länge und 1,50 m Breite bricht in eine Richtung deiner Wahl aus dir hervor. Jede Kreatur innerhalb der Linie muss einen Geschicklichkeitsrettungswurf ablegen. Bei einem Misserfolg erleidet das Ziel 8W6 Blitzschaden oder halb so viel Schaden bei einem erfolgreichen Rettungswurf.
Der Blitz entzündet alle brennbaren Gegenstände im Wirkungsbereich, die nicht getragen oder in der Hand gehalten werden.

## Auf höheren Graden
Wenn du diesen Spruch mit einem Zauberplatz des 4. oder eines höheren Grades wirkst, steigt der Schaden für jeden Grad über den 3. hinaus um 1W6.