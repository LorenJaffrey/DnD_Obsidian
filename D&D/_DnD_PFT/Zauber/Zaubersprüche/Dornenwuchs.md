---
aliases:
  - 
tags:
  - Zauber/Offensiv
Grad: 2
Schule: "[[Verwandlungszauber|Verwandlung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 45 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: sieben scharfe Dornen oder sieben angespitze kleine Zweige
Dauer: 10 Minuten
Konzentration: true
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
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Der Boden in einem Radius von 6 m, zentriert um einen Punkt in Reichweite, wird von harten Stacheln und Dornen überwuchert. Für die Wirkungsdauer gilt der Bereich als schwieriges Gelände. Bewegt sich eine Kreatur in das Gebiet hinein oder innerhalb dessen, erleidet sie 2W4 Stichschaden für jeweils 1,50 m, die sie zurücklegt. Die Verwandlung des Bodens ist so getarnt, dass dieser nicht gefährlich wirkt. Jede Kreatur, die den Bereich nicht sehen kann, wenn der Zauber gewirkt wird, muss bei dessen Betreten einen Wurf auf Weisheit (Wahrnehmung) gegen den SG zum Widerstehen deiner Zauber ablegen. Misslingt er, erkennt sie nicht, welche Gefahr von dem Gelände ausgeht.