---
aliases: 
tags:
  - Zauber/Offensiv
Grad: 7
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 30 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: Rubinstaub im Wert von 1.500 GM
Dauer: 1 Stunde
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
Ein unbewegliches, unsichtbares würfelförmiges Gefängnis aus magischer Energie bildet sich um einen Bereich deiner Wahl in Reichweite. Das Gefängnis kann ein Käfig oder eine geschlossene Kiste sein, wie du möchtest.

Ein Gefängnis in Form einer Kiste hat eine Kantenlänge von bis zu 3 m und erschafft eine feste Barriere, durch die keinerlei Materie dringen kann und die Zauber blockiert, die in den oder aus dem Bereich gewirkt werden.

Ein Gefängnis in Form eines Käfigs besitzt eine Kantenlänge von 6 m und besteht aus 1,25 cm dicken Stäben, die jeweils 1,25 cm voneinander entfernt sind. Wenn du den Zauber wirkst, wird jede Kreatur in dem Energiekäfig gefangen, die vollständig von ihm umschlossen ist. Kreaturen, die sich nur zum Teil in dem Bereich aufhalten oder die zu groß für den Käfig sind, werden von der Mitte des Bereichs weggestoßen, bis sie sich vollständig außerhalb befinden. 
Eine Kreatur im Energiekäfig kann diesen nur auf magische Art verlassen. Wenn der Gefangene versucht, mittels Teleportation oder Ebenenreisen zu entfliehen, muss er zunächst einen Charismarettungswurf ablegen. Bei einem Erfolg kann die Kreatur diese Art von Magie verwenden, um den Energiekäfig zu verlassen. Bei einem  Misserfolg kann sie dies nicht und der gewirkte Zauber ist vergeudet. Der Energiekäfig erstreckt sich auch in die Atherebene, was eine Flucht über diese Ebene verhindert.

Der Zauber kann nicht durch Magie bannen aufgehoben werden.