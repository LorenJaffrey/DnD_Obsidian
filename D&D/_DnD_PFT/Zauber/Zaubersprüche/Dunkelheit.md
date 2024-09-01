---
aliases: 
tags:
  - Zauber/Offensiv
Grad: 2
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 18 Meter
Verbal: true
Geste: false
Material: true
Materialkosten: Fledermausfell und ein Tropfen Pech oder ein Stück Kohle
Dauer: 10 Minuten
Konzentration: true
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
Magische Dunkelheit breitet sich von einem Punkt deiner Wahl in Reichweite aus (auch um Ecken) und füllt für die Wirkungsdauer eine Sphäre mit einem Radius von 4,50 m. Selbst Kreaturen mit Dunkelsicht vermögen den Bereich mit Blicken nicht zu durchdringen und nicht-magisches Licht kann ihn nicht erhellen. Ist der gewählte Punkt ein Gegenstand, breitet sich die Dunkelheit von dem Gegenstand aus und bewegt sich mit ihm, falls eine Kreatur ihn trägt oder in der Hand hält. Wird die Quelle der Dunkelheit vollständig mit einem blickdichten Gegenstand bedeckt, wie einer Schüssel oder einem Helm, blockiert das die Dunkelheit. Überschneidet sich die Sphäre mit einem Bereich magischen Lichts, der mit einem Spruch des 2. oder eines niedrigeren Grades erschaffen wurde, wird der Zauber aufgehoben, der das Licht verursacht.