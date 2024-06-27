---
aliases:
  - Speak with Animals
tags:
  - Zauber
Grad: 1
Schule: "[[Erkenntniszauber|Erkenntnismagie]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Selbst
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: 10 Minuten
Konzentration: false
Ritual: true
Skalierbar: false
Klassen:
- "[[Barde]]"
- "[[Druide]]"
- "[[Waldläufer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Für die Wirkungsdauer kannst du Tiere verstehen und verbal mit ihnen kommunizieren. 
Das Wissen und die Wahrnehmung vieler Tiere wird durch ihre Intelligenz eingeschränkt. 
Sie sind jedoch zumindest in der Lage, Informationen über nahe Orte und Monster mitzuteilen - sowie über Ereignisse, die sie wahrnehmen können oder innerhalb des letzten Tages erlebt haben. 
Nach Ermessen des SL kannst du ein Tier überreden, dir einen kleinen Gefallen zu erweisen.