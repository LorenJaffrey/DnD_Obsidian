---
aliases:
  - Entangle
tags:
  - Zauber
Grad: 1
Schule: "[[Beschwörungszauber|Beschwörung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 27 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: 1 Minute
Konzentration: true
Ritual: false
Skalierbar: false
Schaden: 
Schadensart: 
Ziel: AoE
Klassen:
  - "[[Druide]]"
  - "[[Waldläufer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Umschlingende Gräser und Ranken wachsen in einem quadratischen Bereich mit 6 m Seitenlänge in Reichweite aus dem Boden. 
Für die Wirkungsdauer verwandeln diese Pflanzen den Boden in [[Schwieriges Gelände]].
Jede Kreatur, die sich in dem Bereich aufhält, wenn du den Zauber wirkst, muss einen erfolgreichen [[Rettungswurf]] auf [[Stärke]] ablegen, um nicht für die Wirkungsdauer von den umschlingenden Pflanzen [[Festgesetzt]] zu werden. 
Eine Kreatur, die von den Pflanzen [[Festgesetzt]] ist, kann als [[Aktion]] einen [[Attribute|Attributswurf]] auf [[Stärke]] gegen deinen [[Zauberrettungswurf-Schwierigkeitsgrad]] ablegen. Bei einem Erfolg kann sie sich befreien.
Wenn der Zauber endet, verdorren die beschworenen Pflanzen.