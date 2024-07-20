---
aliases: 
  - Healing Word
tags: 
  - Zauber
Grad: 1
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Bonusaktion]]"
Reichweite: 18 Meter
Verbal: true
Geste: false
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Klassen:
  - "[[Barde]]"
  - "[[Druide]]"
  - "[[Kleriker]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Eine Kreatur deiner Wahl, die sich in Reichweite befindet und die du sehen kannst, erhält [[Trefferpunkte]] zurück in Höhe von 1W4 + den Modifikator deines zum Zaubern relevanten Attributs. 
Der Zauber hat keine Auswirkungen auf [[Untote]] oder [[Konstrukte]].

### Auf höheren Graden
Wenn du diesen Spruch mit einem [[Zauberplätze|Zauberplatz]] des 2. oder eines höheren [[Zaubergrad|Grades]] wirkst, steigt die Anzahl der geheilten [[Trefferpunkte]] für jeden [[Zaubergrad|Grad]] über den 1. hinaus um 1W4.