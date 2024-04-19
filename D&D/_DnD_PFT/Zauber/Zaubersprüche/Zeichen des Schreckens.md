---
aliases:
  - Sign of Terror
tags:
  - Zauber
Grad: 1
Schule: "[[Verzauberungen|Verzauberung]]"
Zeitaufwand: "[[Zug#Aktion]]"
Reichweite: 12 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: 
Dauer: 1m
Konzentration: true
Ritual: false
Skalierbar: true
Klassen:
- "[[Hexenmeister]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Du erschaffst vor den Augen einer Kreatur kurzzeitig eine schreckliche, glühende Rune , die mit einer schreckenerregenden Aura pulsiert.*

Die Kreatur muss einen [[Rettungswurf]] auf [[Weisheit]] bestehen oder wird [[Verängstigt]] bis der Zauber endet.
Das Ziel kann den [[Rettungswurf]] am Ende jedes [[Zug|Zuges]] wiederholen. Bei [[Erfolg]] endet der Effekt des Spruchs sofort.
[[Konstrukte]] und [[Untote]] sind immun gegen diesen Effekt.

### Auf höheren Graden
Wenn du diesen Spruch mit einem [[Zauberplätze|Zauberplatz]] des 2. oder eines höheren [[Zaubergrad|Grades]] wirkst, kannst du für jeden [[Zaubergrad|Grad]] über den 1. hinaus eine zusätzliche Kreatur als Ziel wählen.
Jede weitere Kreatur muss sich innerhalb von 3m (2 Kästchen) um das ursprüngliche Ziel befinden.