---
aliases:
  - Cure Wounds
tags:
  - Zauber
Grad: 1
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Klassen:
  - "[[Druide]]"
  - "[[Barde]]"
  - "[[Kleriker]]"
  - "[[Paladin]]"
  - "[[Magieschmied]]"
  - "[[Waldläufer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Eine Kreatur, die du berührst, gewinnt [[Trefferpunkte]] in Höhe von 1W8 + deinem [[Zauberattribut]]-Modifikator zurück. 
Dieser Zauber wirkt nicht auf [[Untote]] oder [[Konstrukte]].

### Auf höheren Graden
Wirkst du diesen Zauber, indem du einen [[Zauberplätze|Zauberplatz]] des 2. [[Zaubergrad|Grades]] oder höher nutzt, steigt die Heilung für jeden [[Zaubergrad|Grad]] über dem 1. um 1W8.