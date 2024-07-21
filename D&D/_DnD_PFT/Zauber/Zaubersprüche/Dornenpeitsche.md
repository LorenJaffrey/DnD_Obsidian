---
aliases:
  - Thorn Whip
tags:
  - Zauber/Offensiv
Grad: 0
Schule: "[[Verwandlungszauber|Verwandlung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 9 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Schaden: 1W6
Schadensart: "[[Stichschaden]]"
Ziel: AoE
Klassen:
  - "[[Druide]]"
  - "[[Magieschmied]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du erschaffst eine lange, rankenartige Peitsche, die mit Dornen bedeckt ist und die auf deinen Befehl hin nach einer Kreatur in Reichweite schlägt. 
Führe einen [[Nahkampfangriff|Nahkampf]]-Zauberangriff gegen das Ziel durch. 
Wenn der Angriff trifft, erleidet die Kreatur 1W6 [[Stichschaden]] . 
Handelt es sich um eine Kreatur der [[Größenkategorie]] [[Groß]] oder kleiner, wird sie zusätzlich 3 m in deine Richtung gezogen.

### Auf höheren Graden
Der Schaden dieses Zaubers steigt jeweils um 1W6 bei Erreichen höherer Stufen:
- Stufe 5 (2W6)
- Stufe 11 (3W6) 
- Stufe 17 (4W6).