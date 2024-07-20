---
aliases: 
  - Bane
tags: 
  - Zauber
Grad: 1
Schule: "[[Verzauberungen|Verzauberung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 9 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: 
Dauer: 1m
Konzentration: true
Ritual: false
Skalierbar: true
Klassen:
  - "[[Barde]]"
  - "[[Kleriker]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Bis zu drei Kreaturen deiner Wahl in Reichweite, die du sehen kannst, müssen einen [[Rettungswurf]] auf [[Charisma]] ablegen. 
Immer wenn ein Ziel, dem sein [[Rettungswurf]] nicht gelungen ist, während der Wirkungsdauer des Zaubers einen [[Angriffswurf]] oder [[Rettungswurf]] ausführt, muss es mit einem W4 würfeln und das Ergebnis vom entsprechenden Wurf abziehen.

### Auf höheren Graden
Wenn du diesen Spruch mit einem [[Zauberplätze|Zauberplatz]] des 2. oder eines höheren [[Zaubergrad|Grades]] wirkst, kannst du für jeden [[Zaubergrad|Grad]] über den 1. hinaus eine zusätzliche Kreatur als Ziel wählen.