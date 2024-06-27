---
aliases: 
- Thunderwave
tags: 
- Zauber
Grad: 1
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Würfel 4,5 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Klassen:
- "[[Barde]]"
- "[[Druide]]"
- "[[Magier]]"
- "[[Zauberer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Eine Woge aus donnernder Kraft geht von dir aus.* 

Jede Kreatur in einem Würfel mit 4,50 m Kantenlänge muss einen [[Rettungswurf]] auf [[Konstitution]] ablegen. Bei einem Misserfolg erleidet eine Kreatur 2W8 [[Schallschaden]] und wird 3 m von dir weggestoßen.

Bei einem erfolgreichen [[Rettungswurf]] erleidet die Kreatur nur den halben Schaden und wird nicht weggestoßen.

Nicht gesicherte oder befestigte Gegenstände, die sich vollständig innerhalb des Wirkungsbereichs befinden, werden automatisch 3 m von dir weggestoßen. Der Zauber erzeugt ein donnerndes Dröhnen, das bis in 90 m Entfernung hörbar ist.

### Auf höheren Graden
Wenn du diesen Spruch mit einem [[Zauberplätze|Zauberplatz]] des 2. oder eines höheren Grades wirkst, steigt der Schaden für jeden Grad über den 1. hinaus um 1W8.