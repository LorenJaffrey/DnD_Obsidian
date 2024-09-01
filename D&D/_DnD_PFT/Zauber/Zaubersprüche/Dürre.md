---
aliases:
tags:
  - Zauber
Grad: 4
Schule: "[[Nekromantiezauber|Nekromantie]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 9 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: true
Ritual: false
Skalierbar: true
Schaden: 8W8
Schadensart: "[[Nekrotischer Schaden]]"
Ziel: 
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer:  `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Nekromantische Energie ergießt sich über eine Kreatur deiner Wahl in Reichweite, die du sehen kannst, und entzieht ihr jegliche Feuchtigkeit und Vitalität. Das Ziel muss einen Konstitutionsrettungswurf ablegen. Bei einem Misserfolg erleidet die Kreatur 8W8 nekrotischen Schaden oder halb so viel Schaden bei einem erfolgreichen Rettungswurf. Der Zauber hat keine Auswirkungen auf Untote oder Konstrukte. Wenn du den Zauber auf eine Pflanzenkreatur oder eine magische Pflanze wirkst, ist diese bei ihrem Rettungswurf im Nachteil und der Zauber verursacht den maximal möglichen Schaden. Du kannst als Ziel auch eine nicht-magische Pflanze auswählen, die keine Kreatur ist (etwa einen gewöhnlichen Baum oder einen Busch). Die Pflanze legt keinen Rettungswurf ab: Sie verdorrt einfach und stirbt.

## Auf höheren Graden
Wenn du diesen Spruch mit einem Zauberplatz des 5. oder eines höheren Grades wirkst, steigt der Schaden für jeden Grad über den 4. hinaus um 1W8.