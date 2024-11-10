---
aliases:
  - Snilloc’s Snowball Swarm
tags:
  - Zauber
Grad: 2
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 27 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: ein Stück Eis, oder ein kleiner weißer Steinsplitter
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Schaden: 3d6
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
Ein Hagel magischer Schneebelle bricht von einem Punkt hervor, den du innerhalb der Reichweite wählst. Jede Kreatur in einer Kugel mit 1,50 Meter  (1 Kästchen) Radius, deren Zentrum an diesem Punkt liegt, muss einen [[Geschicklichkeit]]-[[Rettungswurf]] durchführen. Eine Kreatur erleidet 3W6 [[Kälteschaden]] bei einem Fehlschlag, die Hälfte davon bei einem Erfolg.

## Auf  höheren Graden
Wenn du diesen Zauber unter Verwendung eines [[Zauberplätze|Zauberplatz]] des 3. Grades oder höher verwendest, so erhöht sich der Schaden um 1W6 für jeden Zauberplatz-Grad über dem zweiten.

Quelle: Xanathars Ratgeber für alles, Seite: 165