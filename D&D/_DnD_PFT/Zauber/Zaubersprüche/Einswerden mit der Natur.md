---
aliases: 
tags: 
  - Zauber
Grad: 5
Schule: "[[Erkenntniszauber|Erkenntnis]]"
Zeitaufwand: 1 Minute
Reichweite: selbst
Verbal: true
Geste: true
Material: false
Materialkosten:
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
Du wirst für einen Augenblick eins mit der Natur und erlangst Wissen über die Umgebung. Im Freien wirkt der Zauber auf das Land, das dich innerhalb von 4,5 km umgibt. In Höhlen und an anderen unterirdischen Plätzen sinkt der Radius auf 90 m. Der Zauber funktioniert nur an natürlichen Orten, nicht in Gebieten, die vollständig durch Bebauung entstanden sind, wie Kerker oder Städte.

Du erlangst sofort Wissen über bis zu drei Fakten deiner Wahl zu einem der folgenden Themen bezüglich der Umgebung:

- Gelände und Gewässer,
- vorherrschende Pflanzen, Mineralien, Tiere oder Bewohner,
- mächtige celestische Wesen, Feen, Unholde, Elementare oder Untote, · Einflussnahmen von anderen Existenzebenen,
- Bauwerke.

Beispielsweise könntest du herausfinden, wo sich in dieser Gegend ein mächtiger Untoter aufhält, sich wichtige Quellen von Trinkwasser befinden und nahe Städte liegen.