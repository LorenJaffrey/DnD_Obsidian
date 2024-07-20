---
aliases:
  - Shield
tags:
  - Zauber
Grad: 1
Schule: "[[Bannzauber|Bannmagie]]"
Zeitaufwand: "[[Reaktion]]"
Reichweite: Selbst
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: 1 Runde
Konzentration: false
Ritual: false
Skalierbar: false
Schaden: 
Schadensart: 
Ziel: Einzel
Klassen:
  - "[[Zauberer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer:  1 Runde

## Beschreibung
*Eine unsichtbare Barriere aus magischer Energie erscheint und schützt dich.*

Bis zum Beginn deines nächsten Zuges hast du einen Bonus von +5 auf deine [[Rüstungsklasse]], auch gegen den auslösenden Angriff, und erleidest keinen Schaden durch den Zauber [[Magisches Geschoss]].

Quelle: Players Handbook, Seite: 260