---
aliases:
  - Mage Armor
tags:
  - Zauber
Grad: 1
Schule: "[[Bannzauber|Bannmagie]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: true
Materialkosten: ein Stück gehörtetes Leder
Dauer: 8 Stunden
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
*Eine unsichtbare Rüstung aus magischer Energie schützt dich.*

Du berührst eine bereitwillige Kreatur, die keine Rüstung trägt. Schützende magische Energie umgibt sie, bis der Zauber endet. Die Basis-[[Rüstungsklasse]] des Ziels entspricht nun 13 + seinen [[Geschicklichkeit]]-Modifikator. Der Zauber endet, wenn das Ziel eine Rüstung anlegt oder du den Zauber mit einer Aktion aufhebst.

Quelle: Players Handbook, Seite: 247