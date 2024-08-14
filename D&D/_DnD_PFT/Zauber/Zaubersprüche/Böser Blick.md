---
aliases:
tags:
  - Zauber
Grad: 6
Schule: "[[Nekromantiezauber|Nekromantie]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: selbst
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
Für die Wirkungsdauer des Zaubers werden deine Augen zu einer tintenschwarzen Leere, die von grauenhafter Macht erfüllt ist. Eine Kreatur deiner Wahl innerhalb von 18 m, die du sehen kannst, muss einen erfolgreichen Weisheitsrettungswurf ablegen, um nicht für die Wirkungsdauer einen der folgenden Effekte deiner Wahl zu erleiden. In jedem deiner Züge, bis der Zauber endet, kannst du deine Aktion verwenden, um eine weitere Kreatur als Ziel zu wählen. Dabei kannst du jedoch keine Kreatur bestimmen, deren Rettungswurf gegen diese Verwendung von Böser Blick bereits erfolgreich war.

**Schlaf:** Das Ziel wird bewusstlos. Es wacht auf, wenn es Schaden erleidet oder eine andere Kreatur ihre Aktion verwendet, um den Schlafenden wachzurütteln.

**Panik:** Das Ziel wird von dir verängstigt. In jedem ihrer Züge muss die verängstigte Kreatur die Spurtaktion verwenden und sich auf dem sichersten sowie kürzesten verfügbaren Weg von dir wegbewegen, bis dies nicht mehr möglich ist. Der Effekt endet, wenn sich das Ziel an einem Ort mindestens 18 m von dir entfernt befindet, an dem sie dich nicht mehr sehen kann.

**Übelkeit:** Das Ziel ist im Nachteil bei Angriffs- und Attributswürfen. Am Ende eines jeden seiner Züge darf es einen weiteren Weisheitsrettungswurf ablegen. Bei einem Erfolg endet der Effekt.
