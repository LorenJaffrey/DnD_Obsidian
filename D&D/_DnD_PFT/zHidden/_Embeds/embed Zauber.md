# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbal (V)]], [[Geste (G)]], [[Material (M)]]", "[[Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbal (V)]], [[Material (M)]]", "[[Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Geste (G)]], [[Material (M)]]", "[[Geste (G)]]"),	choice(this.Material, "[[Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`
Klassen: `=this.Klassen`