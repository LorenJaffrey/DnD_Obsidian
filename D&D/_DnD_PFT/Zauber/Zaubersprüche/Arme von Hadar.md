---
aliases:
  - Arms of Hadar
tags:
  - Zauber/Offensiv
Grad: 1
Schule: "[[Beschwörungszauber|Beschwörung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Radius 3 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: 
Dauer: unmittelbar
Konzentration: true
Ritual: true
Skalierbar: true
Schaden: 2W6
Schadensart: "[[Nekrotischer Schaden]]"
Ziel: AoE
Klassen: 
  - "[[Hexenmeister]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`
Klassen: `=this.Klassen`
## Beschreibung
*Du berufst dich auf die Macht Hadars, des Dunklen Hungers.*

Tentakel aus finsterer Energie brechen aus dir hervor und schlagen auf alle Kreaturen innerhalb von 3 m ein. Jede Kreatur in diesem Bereich muss einen [[Rettungswurf]] auf [[Stärke]] ablegen. 
Bei einem Misserfolg erleidet ein Ziel 2W6 [[Nekrotischer Schaden]] und kann bis zu seinem nächsten [[Zug]] keine [[Reaktion]] verwenden. Bei einem erfolgreichen [[Rettungswurf]] nimmt die Kreatur halben Schaden, erleidet aber keine anderen Auswirkungen.

### Auf höheren Graden
Wenn du diesen Spruch mit einem [[Zauberplätze|Zauberplatz]] des 2. oder eines höheren [[Zaubergrad|Grades]] wirkst, steigt der Schaden für jeden [[Zaubergrad|Grad]] über den 1. hinaus um 1W6.