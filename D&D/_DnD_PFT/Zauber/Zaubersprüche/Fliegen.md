---
aliases:
  - 
tags:
  - Zauber/Offensiv
Grad: 3
Schule: "[[Verwandlungszauber|Verwandlung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: true
Materialkosten: eine Flügelfeder von einem beliebigen Vogel
Dauer: 10 Minuten
Konzentration: true
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
Du berührst eine bereitwillige Kreatur. Für die Wirkungsdauer erhält das Ziel eine Flugbewegungsrate von 18 Metern. Wenn der Zauber endet und das Ziel noch fliegt, fällt es herunter, sofern es den Sturz nicht verhindern kann.

## Auf höheren Graden
Wenn du diesen Zauber wirkst, indem du einen Zauberplatz des 4. Grades oder höher nutzt, kannst du für jeden Grad über dem 3. eine zusätzliche Kreatur als Ziel wählen.