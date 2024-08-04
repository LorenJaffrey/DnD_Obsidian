---
aliases:
  - Arkanes Auge
tags:
  - Zauber
Grad: 4
Schule: "[[Erkenntniszauber|Erkenntnismagie]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 9 m
Verbal: true
Geste: true
Material: true
Materialkosten: etwas aus Fledermausfell
Dauer: 1 Stunde
Konzentration: true
Ritual: false
Skalierbar: false
Schaden: 
Schadensart: 
Ziel: 
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du erschaffst ein unsichtbares, magisches Auge in Reichweite, das für die Wirkungsdauer in der Luft schwebt. Du erhältst auf geistige Weise visuelle Informationen von dem Auge, das über normale Sicht sowie eine Dunkelsicht von 9 m verfügt. Das Auge kann in alle Richtungen blicken. Als Aktion kannst du das Auge 9 m beliebig bewegen. Es darf sich von dir entfernen, aber nicht eine andere Ebene der Existenz betreten. Eine feste Barriere blockiert die Bewegung des Auges, es ist aber in der Lage, sich durch Öffnungen mit 2,5 cm Durchmesser zu zwängen.