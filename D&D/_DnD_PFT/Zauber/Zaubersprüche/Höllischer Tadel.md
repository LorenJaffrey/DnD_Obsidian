---
aliases: 
- Hellish Rebuke
tags: 
- Zauber
Grad: 1
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Reaktion]]"
Reichweite: 18 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
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
*Du deutest mit einem Finger und die Kreatur, die dich verletzt hat, wird für einen kurzen Moment von höllischen Flammen eingehüllt.*

Die Kreatur muss einen [[Rettungswurf]] auf [[Geschicklichkeit]] ablegen.
Bei einem Misserfolg erleidet das Ziel 2W10 [[Feuerschaden]] oder halb so viel Schaden bei einem erfolgreichen [[Rettungswurf]].

### Auf höheren Graden
Wenn du diesen Spruch mit einem [[Zauberplätze|Zauberplatz]] des 2. oder eines höheren Grades wirkst, steigt der Schaden für jeden Grad über den 1. hinaus um 1W10.