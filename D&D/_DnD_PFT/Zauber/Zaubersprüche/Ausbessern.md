---
aliases: 
  - 
tags: 
  - Zauber
Grad: 0
Schule: "[[Verwandlungszauber|Verwandlung]]"
Zeitaufwand: 1 Minute
Reichweite: Berührung
Verbal: true
Geste: true
Material: true
Materialkosten: zwei Magnetsteine
Dauer: unmittelbar
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
Dieser Zauber repariert eine Bruchstelle oder einen Riss in einem Gegenstand, den du berührst, beispielsweise ein zerbrochenes Kettenglied, die beiden Hälften eines zerbrochenen Schlüssels, einen zerrissenen Umhang oder einen leckenden Weinschlauch. Solange der Riss oder die Bruchstelle in keiner
Ausdehnung größer als 30 cm ist, kannst du sie flicken, sodass keine Spur des vorherigen Schadens übrig bleibt. Der Zauber kann einen magischen Gegenstand oder ein Konstrukt auf physische Weise reparieren, einem solchen Gegenstand jedoch nicht seine Magie wiedergeben.