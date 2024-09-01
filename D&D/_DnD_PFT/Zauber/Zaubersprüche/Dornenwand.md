---
aliases:
tags:
  - Zauber/Offensiv
Grad: 6
Schule: "[[Beschwörungszauber|Beschwörung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 36 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: eine Handvoll Dornen
Dauer: 10 Minuten
Konzentration: true
Ritual: false
Skalierbar: true
Schaden: 7W8
Schadensart: "[[Hiebschaden]]" 
Ziel: AoE
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du erschaffst eine Barriere aus zähen, biegsamen und verworrenen Büschen, die vor nadelspitzen Dornen starren. Sie erscheint innerhalb der Reichweite auf einem festen Untergrund und bleibt für die Wirkungsdauer bestehen. Die Barriere kann gerade sein (bis zu 18 m lang, 3 m hoch und 1,50 m dick) oder ringförmig (bis zu 6 m Durchmesser, 3 m Höhe und 1,50 m Dicke). Sie blockiert die Sichtlinie. Erschaffst du die Barriere, müssen alle Kreaturen in ihrem Bereich einen Geschicklichkeitsrettungswurf ablegen. Bei einem Misserfolg erleidet eine Kreatur 7W8 Stichschaden oder
halb so viel Schaden bei einem gelungenen Rettungswurf. Eine Kreatur kann sich durch die Barriere bewegen, allerdings nur langsam und unter großen Schmerzen. Für jeweils 30 cm, die sich die Kreatur durch die Dornenbüsche bewegt, muss sie 1,20 m Bewegungsrate aufwenden. Betritt eine Kreatur die Barriere das erste Mal in einem Zug oder beendet sie ihren Zug dort, muss sie außerdem einen Geschicklichkeitsrettungswurf ablegen. Bei einem Misserfolg erleidet sie 7W8 Hiebschaden oder halb so viel Schaden bei einem erfolgreichen Rettungswurf.

## Auf höheren Graden
Wenn du diesen Spruch mit einem Zauberplatz des 7. oder eines höheren Grades wirkst, steigen beide Schadensarten für jeden Grad über den 6. hinaus um 1W8.