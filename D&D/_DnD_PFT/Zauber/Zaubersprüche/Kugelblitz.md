---
aliases:
tags:
  - Zauber/Offensiv
Grad: 6
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 45 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: ein Stück Fell, ein Stück Bernstein, Glas oder eine Kristallstange und drei Silbernadeln
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Schaden: 10W8
Schadensart: [[Blitzschaden]]
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
Du erschaffst einen Blitz, der in einem Bogen auf ein Ziel deiner Wahl zusteuert, das du in Reichweite sehen kannst. Drei Blitze springen dann von diesem Ziel zu bis zu drei anderen Zielen, die sich jeweils innerhalb von 9 Metern um das erste Ziel befinden müssen. Ein Ziel kann eine Kreatur oder ein Gegenstand sein und kann nur von einem der Blitze getroffen werden.

Ein Ziel muss einen Rettungswurf auf Geschicklichkeit machen. Bei einem misslungenen Rettungswurf erleidet das Ziel 10W8 Blitzschaden, bei einem erfolgreichen Rettungswurf die Hälfte des Schadens.

## Auf höheren Graden
Wenn du diesen Zauberspruch mit einem Zauberplatz des 7. Grades oder höher wirkst, springt für jeden Zauberplatz-Grad über dem 6. Grad ein zusätzlicher Bolzen vom ersten Ziel zu einem anderen Ziel.