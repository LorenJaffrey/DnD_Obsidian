---
aliases: 
tags:
  - Zauber/Offensiv
Grad: 1
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 27 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: ein Diamant im Wert von mindestens 50 GM
Dauer: unmitttelbar
Konzentration: false
Ritual: false
Skalierbar: true
Schaden: 3d8
Schadensart:
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
Du schleuderst eine Sphäre aus Energie mit 10 cm Durchmesser auf eine Kreatur in Reichweite, die du sehen kannst. Beim Wirken des Zaubers wählst du Blitz, Feuer, Gift, Kälte, Säure oder Schall aus, um die Art der Kugel zu bestimmen, und führst dann einen Fernkampf-Zauberangriff gegen das Ziel aus. Trifft der Angriff, erleidet das Ziel 3W8 Schaden des gewählten Typs.

## Auf höheren Graden
Wenn du diesen Spruch mit einem Zauberplatz des 2. oder eines höheren Grades wirkst, steigt der Schaden für jeden Grad über den 1. hinaus um 1W8.