---
aliases:
  - Invisibility
tags:
  - Zauber
Grad: 2
Schule: "[[Illusionszauber|Illusion]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: true
Materialkosten: 
Dauer: 1 Stunde
Konzentration: true
Ritual: false
Skalierbar: false
Klassen:
  - "[[Barde]]"
  - "[[Magieschmied]]"
  - "[[Hexenmeister]]"
  - "[[Zauberer]]"
  - "[[Magier]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Eine Kreatur, die du berührst, wird [[Unsichtbar]], bis der Zauber endet. 
Alles, was das Ziel trägt oder in der Hand hält, wird ebenfalls [[Unsichtbar]], solange es sich am Körper der Kreatur befindet.
Der Zauber endet für das betroffene Ziel, wenn dieses angreift oder einen Zauber wirkt.

### Auf höheren Graden
Wenn du diesen Spruch mit einem [[Zauberplätze|Zauberplatz]] des 3. oder eines höheren [[Zaubergrad|Grades]] wirkst, kannst du für jeden [[Zaubergrad|Grad]] über den 2. hinaus eine zusätzliche Kreatur als Ziel wählen.