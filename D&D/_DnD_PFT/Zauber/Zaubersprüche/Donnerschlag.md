---
aliases:
  - Thunderclap
tags:
  - Zauber
Grad: 0
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 1,50 Meter
Verbal: false
Geste: true
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Klassen:
  - "[[Zauberer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du erzeugst einen Ausbruch donnernden Klangs, den man bis zu 30 m weit hören kann. 
Jede andere Kreatur innerhalb der Reichweite außer dir muss einen [[Rettungswurf]] auf [[Konstitution]] bestehen oder 1W6 [[Schallschaden]] erleiden. 

### Auf höheren Graden
Der Schaden dieses Zaubers steigt jeweils um 1W6 bei Erreichen höherer Stufen:
- Stufe 5 (2W6)
- Stufe 11 (3W6) 
- Stufe 17 (4W6)

Quelle: Xanathars Ratgeber für alles, Seite: 152