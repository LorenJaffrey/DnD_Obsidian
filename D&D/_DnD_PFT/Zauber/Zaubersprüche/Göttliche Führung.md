---
aliases:
  - Guidance
tags:
  - Zauber
Grad: 0
Schule: "[[Erkenntniszauber|Erkenntnismagie]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: 1 Minute
Konzentration: true
Ritual: false
Skalierbar: false
Schaden: 
Schadensart: 
Ziel: Einzel
Klassen:
  - "[[Magieschmied]]"
  - "[[Kleriker]]"
  - "[[Druide]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du berührst eine bereitwillige Kreatur. 
Einmal während der Wirkungsdauer kann das Ziel mit einem W4 würfeln und das Ergebnis auf einen [[Attribute|Attributswurf]] seiner Wahl addieren. 
Es darf sich vor oder nach dem [[Attribute|Attributswurf]] dazu entscheiden, den Würfel einzusetzen. 
Anschließend endet der Zauber.