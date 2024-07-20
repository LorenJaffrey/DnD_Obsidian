---
aliases: 
  - Mage Hand
tags: 
  - Zauber
Grad: 0
Schule: "[[Beschwörungszauber|Beschwörung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 9 Meter
Verbal: true
Geste: true
Material: false
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
  - "[[Magieschmied]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Eine geisterhafte, schwebende Hand erscheint an einem Punkt deiner Wahl in Reichweite.*

Die Hand bleibt für die Wirkungsdauer bestehen oder bis du sie mit einer [[Aktion]] fortschickst. 
Sie verschwindet auch, wenn sie sich weiter als 9 m von dir entfernt oder du den Zauber erneut wirkst.
Als [[Aktion]] kannst du die Hand kontrollieren und sie verwenden, um mit Gegenständen zu interagieren, geschlossene Türen oder Behälter zu öffnen, einen Gegenstand aus einem geöffneten Behälter zu holen oder ihn darin zu verstauen oder den Inhalt einer Phiole auszugießen. 
Immer wenn du die Hand kontrollierst, darfst du sie bis zu 9 m bewegen.
Die Hand kann nicht [[Angriff|angreifen]], keine magischen Gegenstände aktivieren oder mehr als 10 Pfund tragen.