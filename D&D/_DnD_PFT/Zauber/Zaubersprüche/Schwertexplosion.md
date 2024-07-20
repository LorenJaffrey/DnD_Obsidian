---
aliases:
  - Sword Burst
tags:
  - Zauber
Grad: 0
Schule: "[[Beschwörungszauber|Beschwörung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Selbst
Verbal: true
Geste: false
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Klassen:
  - "[[Magieschmied]]"
  - "[[Zauberer]]"
  - "[[Magier]]"
  - "[[Hexenmeister]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Für einen Moment fegt eine Schar spektraler Klingen in Kreisform um dich herum.*

Alle Kreaturen innerhalb von 1,5 Metern müssen einen [[Rettungswurf]] auf [[Geschicklichkeit]] ausführen, ansonsten erleiden sie 1W6 [[Energieschaden]].

### Auf höheren Graden
Der Schaden dieses Zaubers steigt jeweils um 1W6 bei Erreichen höherer Stufen:
- Stufe 5 (2W6)
- Stufe 11 (3W6) 
- Stufe 17 (4W6)