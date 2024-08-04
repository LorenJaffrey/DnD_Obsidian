---
aliases:
  - Blade Ward
tags:
  - Zauber
Grad: 0
Schule: "[[Bannzauber|Bannmagie]]"
Zeitaufwand: "[[Aktion]]"
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
*Ein Sigille des Schutzes aus magischer Energie schützt dich.*

Du streckst die Hand aus und zeichnest ein Sigille des Schutzes in die Luft. Bis zum Ende deines nächsten Zuges besitzt du eine [[Schadensarten#Schadensresistenz|Resistenz]] gegen Wucht-, Hieb- und Stichschaden, der von Waffenangriffen verursacht wird.

Quelle: Players Handbook, Seite: 243