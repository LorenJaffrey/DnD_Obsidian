---
aliases:
  - Shocking Grasp
tags:
  - Zauber
Grad: 0
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Klassen:
- "[[Zauberer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Blitze springen aus deinen Händen und versetzen einer Kreatur. die du berührst, einen Schock. Führe einen Nahkampf-Zauberangriff gegen das Ziel durch. Du bist im Vorteil bei diesem Angriffswurf, wenn das Ziel eine Rüstung tragt, die aus Metall besteht. Bei einem Treffer erleidet die Kreatur 1W8 Blitzschaden und kann bis zum Beginn deines nächsten Zuges keine Reaktionen durchführen

### Auf höheren Graden
Der Schaden dieses Zaubers steigt jeweils um 1W8 bei Erreichen höherer Stufen:
- Stufe 5 (2W8)
- Stufe 11 (3W8) 
- Stufe 17 (4W8)

Quelle: Players Handbook, Seite: 261