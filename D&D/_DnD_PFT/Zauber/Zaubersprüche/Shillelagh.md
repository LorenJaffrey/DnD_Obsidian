---
tags: 
  - Zauber
Grad: 0
Schule: "[[Verwandlungszauber|Verwandlung]]"
Zeitaufwand: "[[Bonusaktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: 1m
Konzentration: false
Ritual: false
Skalierbar: false
Klassen:
  - "[[Druide]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Das Holz einer Keule oder eines Kampfstabs, den du in der Hand hältst, wird von der Macht der Natur erfüllt.*

Für die Wirkungsdauer kannst du dein Attribut zum Zauberwirken anstelle von [[Stärke]] verwenden, wenn du [[Angriffswurf]] und [[Schadenswurf]] für [[Nahkampfangriff|Nahkampfangriffe]] mit dieser Waffe durchführst. 
Außerdem wird der Schadenswürfel der Waffe zu einem W10 und die Waffe magisch, falls sie es nicht bereits ist. 
Der Zauber endet, wenn du ihn erneut wirkst oder die Waffe loslässt.