---
aliases:
tags:
Grad: 3
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: unbegrenzt
Verbal: true
Geste: true
Material: true
Materialkosten: ein kurzes Stück feinen Kupferdrahtes
Dauer: 1 Runde
Konzentration: false
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
Du schickst eine kurze Botschaft von 25 Wörtern oder weniger an eine Kreatur, mit der du vertraut bist. 
Die Kreatur hört die Nachricht in ihren Gedanken, erfasst dich als den Sender, sofern sie dich kennt, und kann sofort auf die gleiche Weise antworten. 
Der Zauber erlaubt es Kreaturen mit einem Intelligenzwert von mindestens 1, die Bedeutung der Nachricht zu verstehen. 
Du kannst die Nachricht über jede Entfernung und sogar auf andere Existenzebenen schicken. 
Befindet sich dein Ziel allerdings auf einer anderen Ebene, besteht eine Chance von 5%, dass die  Botschaft nicht ankommt.