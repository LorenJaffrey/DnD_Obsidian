---
aliases:
  - 
tags:
  - Zauber/Offensiv
Grad: 3
Schule: "[[Verwandlungszauber|Verwandlung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 9 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: ein Stück Kork
Dauer: 1 Stunde
Konzentration: false
Ritual: false
Skalierbar: true
Schaden: 
Schadensart: 
Ziel: 
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Dieser Zauber verleiht die Fähigkeit, sich über flüssige Oberflāchen zu bewegen - wie Wasser, Säure, Schlamm, Schnee, Treibsand oder Lava -, als wären sie ungefährlicher, fester Boden (Wesen, die sich über geschmolzene Lava bewegen, erleiden allerdings aufgrund der Hitze Schaden). Bestimme bis zu zehn
bereitwillige Kreaturen in Reichweite, die du sehen kannst, welche die Fähigkeit für die Wirkungsdauer erhalten. Wenn du eine Kreatur als Ziel wählst, die sich in einer Flüssigkeit befindet oder untergetaucht ist, trägt der Zauber sie mit einer Geschwindigkeit von 18 m pro Runde an die Oberfläche.