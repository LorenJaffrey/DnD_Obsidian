---
aliases:
  - Warding Wind
tags:
  - Zauber
Grad: 2
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Selbst
Verbal: true
Geste: false
Material: false
Materialkosten: 
Dauer: 10 Minuten
Konzentration: true
Ritual: false
Skalierbar: false
Schaden: 
Schadensart: 
Ziel: AoE
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
Ein starker Wind (30 km/h) weht in einem Radius von 3 m um dich herum und bewegt sich mit dir, wobei er auf dir zentriert bleibt. 
Der Wind verbleibt für die Wirkungsdauer des Zaubers.

Der Wind hat folgende Effekte: 
- Er macht dich und andere Kreaturen in seinem Bereich [[taub]]. 
- Er löscht ungeschützte Feuer in seinem Bereich die so groß sind wie Fackeln oder kleiner. 
- Er hält Dampfe, Gase und Nebel ab, die von starken Winden verweht werden 
- Der Bereich ist [[Schwieriges Gelände]]für jede Kreatur außer dir. 
- Die [[Angriffswurf|Angriffswürfe]] von [[Fernkampfwaffen]] haben [[Vorteil und Nachteil|Nachteil]], wenn der Angriff in den Wind hinein oder aus ihm hinaus führt.

Quelle: Xanathars Ratgeber für alles, Seite: 164