---
aliases:
  - Fire Bolt
tags:
  - Zauber/Offensiv
Grad: 0
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 36 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Schaden: 1W10
SchadenLv5: 2W10
SchadenLv11: 3W10
SchadenLv17: 4W10
Schadensart: "[[Feuerschaden]]"
Ziel: AoE
Klassen:
  - "[[Magier]]"
  - "[[Zauberer]]"
  - "[[Magieschmied]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du schleuderst einen Splitter aus Feuer auf eine Kreatur in Reichweite. 
Führe einen [[Fernkampfangriff|Fernkampf]]-Zauberangriff gegen das Ziel aus. 
Bei einem Treffer erleidet es 1W10 [[Feuerschaden]].
Ein brennbarer Gegenstand, der von diesem Zauber getroffen wird, geht in Flammen auf, falls er nicht getragen oder in der Hand gehalten wird.

### Auf höheren Graden
Der Schaden dieses Zaubers steigt jeweils um 1W10 bei Erreichen höherer Stufen:
- Stufe 5 (2W10)
- Stufe 11 (3W10) 
- Stufe 17 (4W10)