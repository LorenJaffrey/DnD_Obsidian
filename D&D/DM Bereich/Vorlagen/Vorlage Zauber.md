---
aliases:
  - Englischer Name
tags:
  - Zauber/Art
  - Zauber/Wirkungsbereich
Grad: 1
Schule: Schule
Zeitaufwand: "[[Aktion]]"
Reichweite: Kegel 4,5 Meter
Verbal: false
Geste: false
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: false
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbal (V)]], [[Geste (G)]], [[Material (M)]]", "[[Verbal (V)]], [[Geste (G)]]"), choice(this.Material, "[[Verbale Verbal (V)]], [[Material (M)]]", "[[Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Geste (G)]], [[Material (M)]]", "[[Geste (G)]]"),	choice(this.Material, "[[Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung

### Auf höheren Graden