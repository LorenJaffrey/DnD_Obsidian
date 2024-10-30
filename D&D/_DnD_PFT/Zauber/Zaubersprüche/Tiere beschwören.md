---
aliases:
tags:
  - Zauber/Offensiv
Grad: 3
Schule: "[[Beschwörungszauber|Beschwörung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 18 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: 1 Stunde
Konzentration: true
Ritual: false
Skalierbar: true
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
Du beschwörst Feengeister in Form von Tieren, die in freien Bereichen in Reichweite erscheinen, die du sehen kannst. Wähle eine der folgenden Optionen aus:

- Ein Tier mit Herausforderungsgrad 2 oder niedriger
- Zwei Tiere mit Herausforderungsgrad 1 oder niedriger
- Vier Tiere mit Herausforderungsgrad 1/2 oder niedriger
- Acht Tiere mit Herausforderungsgrad 1/4 oder niedriger
- Jedes Tier ist gleichzeitig ein Feenwesen und verschwindet, wenn der Zauber endet oder seine Trefferpunkte auf 0 sinken.

Die beschworenen Kreaturen sind dir und deinen Gefährten freundlich gesinnt. Würfle die Initiative für die beschworenen Kreaturen als Gruppe aus, die über ihren eigenen Zug verfügt. Sie gehorchen deinen mündlichen Befehlen (erfordert keine Aktion), Wenn du ihnen keine Befehle erteilst, verteidigen sie sich gegen feindlich gesinnte Kreaturen, führen aber anderenfalls keine Aktionen aus.

Der SL hat die Werte der Kreaturen.

## Auf höheren Graden
Wirkst du diesen Zauber mit bestimmten Zauberplätzen höheren Grades, erscheinen mehr Kreaturen, wenn du eine der oben genannten Optionen auswählst: doppelt so viele mit einem Zauberplatz des 5. Grades, dreimal so viele mit einem Zauberplatz des 7. Grades und viermal so viele mit einem Zauberplatz des 9. Grades.