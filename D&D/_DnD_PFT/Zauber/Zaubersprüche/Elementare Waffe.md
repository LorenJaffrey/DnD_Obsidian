---
aliases: 
tags: 
  - Zauber
Grad: 3
Schule: "[[Verwandlungszauber|Verwandlung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: false
Materialkosten:
Dauer: 1 Stunde
Konzentration: true
Ritual: false
Skalierbar: true
Schaden: + 1W4
Schadensart: 
Ziel:
Klassen:
  - "[[Zauberer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Eine nicht-magische Waffe, die du berührst, wird zu einer magischen Waffe. Wähle eine der folgenden Schadensarten: Blitz, Feuer, Kälte, Säure oder Schall. Für die Wirkungsdauer erhält die Waffe einen Bonus von +1 auf Angriffswürfe und fügt bei einem Treffer zusätzlich 1W4 Punkte Schaden des gewählten Typs zu.


## Auf höheren Graden
Wenn du diesen Spruch mit einem Zauberplatz eines höheren Grades wirkst, steigen der Angriffsbonus und der Zusatzschaden: bei einem Zauberplatz des 5. oder 6. Grades auf +2 und 2W4, bei einem des 7. oder eines höheren Grades auf +3 und 3W4.