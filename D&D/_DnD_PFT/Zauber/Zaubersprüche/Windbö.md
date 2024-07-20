---
aliases:
  - Gust
tags:
  - Zauber
Grad: 0
Schule: "[[Verwandlungszauber|Verwandlung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 9 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: false
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
Du ermächtigst dich der Luft und zwingst sie, einen der folgen- den Effekte an einem Punkt zu erzeugen, den du innerhalb der Reichweite sehen kannst: 
- Eine mittelgroße oder kleinere Kreatur muss einen [[Rettungswurf]] auf [[Stärke]] bestehen oder wird bis zu 1,50 m von dir weggedrückt. 
- Du erzeugst einen kleinen Windstoß, der fähig ist, ein Objekt, das weder in der Hand gehalten noch getragen wird und das nicht mehr als 5 Pfund wiegt, zu bewegen. 
   Das Objekt wird bis zu 3 m von dir weggedrückt. 
   Es wird nicht mit genug Kraft weggedrückt, um Schaden zu verursachen 
- Du erzeugst einen harmlosen wahrnehmbaren Effekt unter Verwendung von Luft, wie zum Beispiel das Rascheln von Blättern, Wind, der Fensterläden zuschlägt, oder Kleidung die sich in einer Brise bewegt

Quelle: Xanathars Ratgeber für alles, Seite: 170