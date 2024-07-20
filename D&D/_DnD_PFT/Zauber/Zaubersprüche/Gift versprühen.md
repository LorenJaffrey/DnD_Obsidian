---
aliases: 
  - Poison Spray
tags: 
  - Zauber/Offensiv
Grad: 0
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 3 Meter
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
  - "[[Hexenmeister]]"
  - "[[Magier]]"
  - "[[Magieschmied]]"
  - "[[Zauberer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Du streckst deine Hand in Richtung einer Kreatur aus, die sich in Reichweite befindet und die du sehen kannst, und erzeugst eine Wolke ekelhaften Gases aus deiner Handfläche.*

Die Kreatur muss einen erfolgreichen [[Rettungswurf]] auf [[Konstitution]] ablegen, sonst erleidet sie 1W12 [[Giftschaden]] .

### Auf höheren Stufen
Der Schaden dieses Zaubers steigt wenn du höhere Stufen erreichst 
- 2W12 auf der 5. Stufe
- 3W12 auf der 11. Stufe
- 4W12 auf der 17. Stufe