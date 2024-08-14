---
aliases:
tags:
  - Zauber/Offensiv
Grad: 3
Schule: "[[Beschwörungszauber|Beschwörung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 36 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: 10 Minuten
Konzentration: true
Ritual: false
Skalierbar: true
Schaden: 3W10
Schadensart: "[[Blitzschaden]]" 
Ziel: AoE
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du erschaffst eine Sturmwolke in Form eines Zylinders, der 3 m hoch ist und einen Radius von 18 m besitzt, zentriert um einen Punkt in Reichweite. Der Zauber misslingt, wenn du keinen Punkt in der Luft sehen kannst, an dem die Sturmwolke erscheinen könnte (wenn du beispielsweise in einem Raum bist, der die Wolke nicht aufnehmen kann). Wirkst du den Zauber, wähle einen Punkt unterhalb der Wolke, den du sehen kannst. Ein Blitz fährt von der Wolke herab und schlägt in diesen ein. Jede Kreatur im Umkreis von 1,50 m um den Punkt muss einen Geschicklichkeitsrettungswurf ablegen. Bei einem Misserfolg erleidet das Ziel 3W10 Blitzschaden oder halb so viel Schaden bei einem erfolgreichen Rettungswurf. In jedem deiner Züge, bis der Zauber endet, kannst du deine Aktion verwenden, um auf diese Weise einen weiteren Blitz zu beschwören, der entweder in denselben oder einen anderen Punkt einschlägt. Wenn du dich draußen aufhältst und ein Sturm herrscht, während du den Zauber wirkst, verleiht dieser dir die Kontrolle über den bestehenden Sturm und erschafft keinen eigenen. In diesem Fall steigt der Schaden des Zaubers um 1W10.

## Auf höheren Graden
Wenn du diesen Spruch mit einem Zauberplatz des 4. oder eines höheren Grades wirkst, steigt der Schaden für jeden Grad über den 3. hinaus um 1W10.