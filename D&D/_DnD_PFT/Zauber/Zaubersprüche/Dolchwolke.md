---
aliases:
tags:
  - Zauber/Offensiv
Grad: 2
Schule: "[[Beschwörungszauber|Beschwörung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Selbst
Verbal: true
Geste: true
Material: true
Materialkosten: eine Glasscherbe
Dauer: 1 Minute
Konzentration: true
Ritual: false
Skalierbar: true
Schaden: 4d4
Schadensart: "[[Hiebschaden]]" 
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
Du füllst die Luft in einem Würfel mit 1,50 m Kantenlänge, der um einen Punkt deiner Wahl in Reichweite zentriert ist, mit wirbelnden Dolchen. Eine Kreatur erleidet 4W4 Hiebschaden, wenn sie den Bereich das erste Mal in einem Zug betritt oder ihren Zug dort beginnt.

## Auf höheren Graden
Wenn du diesen Spruch mit einem Zauberplatz des 3. oder eines höheren Grades wirkst, steigt der Schaden für jeden Grad über den 2. hinaus um 2W4.