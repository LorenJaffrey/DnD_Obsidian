---
alias: Minor Illusion
tags: 
- Zauber/Art/Utility
Grad: 0
Schule: "[[Illusionszauber|Illusion]]"
Zeitaufwand: "[[Zug#Aktion]]"
Reichweite: 9 Meter
Verbal: false
Geste: true
Material: true
Materialkosten: 
Dauer: 1m
Konzentration: false
Ritual: false
Skalierbar: false
Klassen:
- "[[Barde]]"
- "[[Hexenmeister]]"
- "[[Magier]]"
- "[[Zauberer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Du erschaffst ein Geräusch oder das Abbild eines Gegenstands, das für die Wirkungsdauer bestehen bleibt.*

Die Illusion endet auch, wenn du sie als [[Zug#Aktion]] aufhebst oder den Zauber erneut wirkst.

Erschaffst du ein Geräusch, kann die Lautstärke von einem Flüstern bis zu einem Schrei reichen. Es kann sich um deine eigene Stimme handeln, die Stimme eines anderen, das Brüllen eines Löwen, schlagende Trommeln oder ein beliebiges anderes Geräusch. Du darfst einen einzigen Laut hervorrufen, der für die gesamte Wirkungsdauer anhält, oder mehrere einzelne Laute zu verschiedenen Zeitpunkten innerhalb der Wirkungsdauer.

Erschaffst du das Abbild eines Gegenstands - wie das eines Stuhles, schlammiger Fußabdrücke oder einer kleinen Truhe -, darf dieses nicht größer als ein Würfel mit einer Kantenlänge von 1,50 m sein. Das Abbild kann weder Geräusche, Licht, Gerüche noch andere sensorische Effekte erzeugen.

Körperliche Interaktion mit dem Trugbild offenbart, dass es sich um eine Illusion handelt, da Dinge es einfach durchdringen.
Eine Kreatur kann ihre [[Zug#Aktion]] verwenden, um das Bildnis oder das Geräusch zu untersuchen. Gelingt ihr ein Wurf auf [[Nachforschungen]] gegen den [[Schwierigkeitsgrad|SG]] zum Widerstehen deiner Zauber, kann sie erkennen, dass es sich um eine Illusion handelt.

Durchschaut eine Kreatur die Illusion, verblasst diese für sie.