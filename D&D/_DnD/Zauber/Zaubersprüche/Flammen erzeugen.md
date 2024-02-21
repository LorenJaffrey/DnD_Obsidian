---
aliases: 
- Produce Flame
tags: 
- Zauber/Art/Schaden/Feuer
- Zauber/Wirkungsbereich/Geschoss
Grad: 0
Schule: "[[Beschwörungszauber|Beschwörung]]"
Zeitaufwand: "[[Zug#Aktion]]"
Reichweite: 9 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: 10m
Konzentration: false
Ritual: false
Skalierbar: true
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
*Eine flackernde Flamme erscheint in deiner Hand.*

Diese bleibt für die Wirkungsdauer bestehen und beschädigt weder dich noch deine Ausrüstung. Sie strahlt innerhalb von 3 m [[Helles Licht]] und in einem Radius von weiteren 3 m [[Dämmriges Licht]] aus. Der Zauber endet, wenn du ihn als [[Zug#Aktion]] aufhebst oder noch einmal wirkst.

Du kannst mit der Flamme auch angreifen, dies beendet jedoch den Zauber. Beim Wirken des Zaubers oder als [[Zug#Aktion]] in einem späteren Zug kannst du die Flamme auf eine Kreatur innerhalb von 9 m werfen. Führe einen Fernkampf-Zauberangriff aus. Bei einem Treffer erleidet das Ziel 1W8 [[Feuerschaden]].

### Auf höheren Graden
Der Schaden dieses Zaubers steigt auf höheren Stufen:
- Stufe 5: 2W8
- Stufe 11: 3W8
- Stufe 17: 4W8