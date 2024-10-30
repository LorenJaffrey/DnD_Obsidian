---
aliases:
  - Lesser Restoration
tags:
  - Zauber
Grad: 3
Schule: "[[Bannzauber|Bannmagie]]"
Zeitaufwand: 1 Reaktion
Reichweite: 18 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: G
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Schaden: 
Schadensart: 
Ziel: Einzel
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du versuchst, eine Kreatur beim Wirken eines Zaubers zu unterbrechen. Wirkt die Kreatur einen Zauber des 3. Grades oder niedriger, scheitert ihr Zauber und hat keinen Effekt. Wirkt sie einen Zauber des 4. Grades oder höher, führe einen Attributswurf mit deinem Attribut zum Zauberwirken aus. Der SG ist 10 + der Grad des Zaubers. Bei einem Erfolg schlägt der Zauber der Kreatur fehl und hat keinen Effekt

## Auf höheren Graden
Wirkst du diesen Zauber, indem du einen Zauberplatz des 4. Grades oder höher nutzt, hat der unterbrochene Zauber keinen Effekt, wenn sein Grad niedriger als er Zauberplatz ist, den du zum Wirken verwendet hast, oder ihm entspricht.