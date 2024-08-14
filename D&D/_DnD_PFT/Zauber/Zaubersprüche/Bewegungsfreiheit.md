---
aliases:
  - 
tags:
  - Zauber
Grad: 4
Schule: "[[Bannzauber|Bannmagie]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: true
Materialkosten: ein Lederriemen, gebunden um einen Arm oder eine ähnliche Gliedmaße
Dauer: 1 Stunde
Konzentration: false
Ritual: false
Skalierbar: false
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
Wirkungsdauer:  `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du berührst eine bereitwillige Kreatur. Für die Wirkungsdauer ist die Bewegung des Ziels nicht durch schwieriges Gelände eingeschränkt, außerdem können Zauber und andere magische Effekte weder die Bewegungsrate der Kreatur verringern noch dafür sorgen, dass sie gelähmt oder festgesetzt wird. Zusätzlich kann das Ziel 1,50 m Bewegungsrate aufwenden, um automatisch aus nicht-magischen Behinderungen zu entkommen, wie Handschellen oder einer Kreatur, die sie festhält. Zu guter Letzt erleiden Bewegung und Angriffe des Ziels keine Abzüge, wenn es
sich unter Wasser aufhält.