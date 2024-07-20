---
aliases: 
  - Eldritch Blast
tags:
  - Zauber/Offensiv
Grad: 0
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 36 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Schaden: 1W10
Schadensart: "[[Energieschaden]]"
Ziel: Einzel
Klassen:
  - "[[Hexenmeister]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Ein Strahl aus knisternder Energie schießt auf eine Kreatur in Reichweite zu.*

Führe einen Fernkampf-Zauberangriff gegen das Ziel aus. Bei einem Treffer erleidet es 1W10 [[Energieschaden]].

### Auf höheren Stufen
Der Zauber erschafft mehr als einen Strahl, wenn du höhere Stufen erreichst: 
- zwei Strahlen auf der 5. Stufe
- drei Strahlen auf der 11. Stufe
- vier Strahlen auf der 17. Stufe
Du kannst die Strahlen auf dasselbe oder unterschiedliche Ziele lenken.
Mache einen eigenständigen [[Zauberangriffswürfe|Zauberangriffswurf]] für jeden Strahl.