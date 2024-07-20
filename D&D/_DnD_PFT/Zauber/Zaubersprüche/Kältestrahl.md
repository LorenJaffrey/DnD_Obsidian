---
aliases:
  - Ray of Frost
tags:
  - Zauber/Offensiv
Grad: 0
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
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
  - "[[Zauberer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Ein eisiger Strahl aus blau-weißem Licht schießt auf eine Kreatur in Reichweite zu.*

Führe einen [[Fernkampfangriff|Fernkampf]]-Zauberangriff gegen das Ziel aus. 
Bei einem Treffer erleidet die Kreatur 1W8 [[Kälteschaden]] und ihre [[Bewegungsrate]] wird bis zum Beginn deines nächsten Zuges um 3 m verringert 

### Auf höheren Graden
Der Schaden dieses Zaubers steigt jeweils um 1W8 bei Erreichen höherer Stufen:
- Stufe 5 (2W8)
- Stufe 11 (3W8) 
- Stufe 17 (4W8)

Quelle: Players Handbook, Seite: 243