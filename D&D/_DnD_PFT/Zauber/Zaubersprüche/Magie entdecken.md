---
aliases: 
- Detect Magic
tags: 
- Zauber
Grad: 1
Schule: "[[Erkenntniszauber|Erkenntnis]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 36 Meter
Verbal: true
Geste: true
Material: false
Materialkosten:
Dauer: 10m
Konzentration: true
Ritual: true
Skalierbar: false
Klassen:
- "[[Barde]]"
- "[[Druide]]"
- "[[Kleriker]]"
- "[[Magier]]"
- "[[Paladin]]"
- "[[Waldläufer]]"
- "[[Zauberer]]"
- "[[Magieschmied]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Für die Wirkungsdauer fühlst du die Anwesenheit von Magie im Umkreis von 9 m. Verwendest du deine [[Aktion]], wenn du Magie auf diese Weise spürst, nimmst du eine schwache Aura um jede sichtbare Kreatur und jeden Gegenstand im Wirkungsbereich wahr, der von Magie erfüllt ist. Außerdem ist dir auch die Schule der Magie bekannt, sofern es eine gibt.
Der Zauber kann die meisten Hindernisse durchdringen, wird aber blockiert von 30 cm Stein, 2,5 cm gewöhnlichem Metall, einer dünnen Schicht Blei oder 90 cm Holz oder Erde.