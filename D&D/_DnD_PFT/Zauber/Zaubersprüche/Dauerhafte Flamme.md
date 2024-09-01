---
aliases: 
tags:
  - Zauber/Offensiv
Grad: 2
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: true
Materialkosten: Rubinstaub im Wert von mindestens 50 GM, der beim Wirken des Zaubers verbraucht wird
Dauer: bis der Zauber gebannt wird
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
Eine Flamme mit der Helligkeit einer Fackel springt aus einem Gegenstand hervor, den du berührst. Der Effekt sieht wie eine gewöhnliche Flamme aus, erzeugt aber keine Hitze und verbraucht keinen Sauerstoff. Eine Dauerhafte Flamme kann verdeckt oder verborgen werden, aber nicht erstickt oder gelöscht.