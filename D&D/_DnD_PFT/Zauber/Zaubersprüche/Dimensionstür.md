---
aliases: 
  - Dimension Door
tags: 
  - Zauber
Grad: 4
Schule: "[[Beschwörungszauber|Beschwörung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 150 Meter
Verbal: true
Geste: false
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: false
Schaden: 
Schadensart: 
Ziel: 
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du teleportierst dich von deiner aktuellen Position zu einem beliebigen anderen Punkt in Reichweite. Du triffst genau an dem gewünschten Punkt ein. Dies kann ein Ort sein, den du sehen oder aus der Erinnerung abrufen kannst oder den du beschreibst, indem du Reichweite und Richtung angibst, wie „60 Meter direkt nach unten“ oder „nordöstlich in einem Winkel von 45 Grad nach oben, und zwar 90 Meter“. Du darfst Gegenstände mitnehmen, solange ihr Gewicht deine Traglast nicht übersteigt, sowie eine bereitwillige Kreatur deiner Größe oder kleiner, die ebenfalls Ausrüstung bis zu ihrer Traglast mit sich führen kann. Die Kreatur muss sich innerhalb von 1,50 m befinden, wenn du den Zauber wirkst. Würdest du an einem Ort ankommen, an dem sich bereits ein Gegenstand oder eine Kreatur befindet, erleiden du und dein Mitreisender 4W6 Energieschaden und ihr werdet nicht teleportiert.