---
aliases:
  - 
tags:
  - Zauber
Grad: 7
Schule: "[[Nekromantiezauber|Nekromantie]]"
Zeitaufwand: 1 Stunde
Reichweite: Berührung
Verbal: true
Geste: true
Material: true
Materialkosten: ein Diamant im Wert von mindestens 1.000 GM, der beim Wirken des Zaubers verbraucht wird)
Dauer: Unmittelbar
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
Wirkungsdauer:  `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du berührst eine verstorbene Kreatur, die nicht länger als 100 Jahre tot ist, nicht an Altersschwäche starb und nicht untot war. Wenn die Seele des Ziels frei und willig ist, kehrt die Kreatur mit allen Trefferpunkten ins Leben zurück. Der Zauber neutralisiert alle Gifte und heilt alle natürlichen Krankheiten, welche die Kreatur bei ihrem Tod plagten. Magische Krankheiten, Flüche oder ähnliche Effekte kann er nicht aufheben. Wenn diese nicht vor Wirken des Zaubers entfernt werden, treten sie wieder in Kraft, sobald die Kreatur zu neuem Leben erweckt ist. Der Zauber schließt alle tödlichen Wunden und stellt alle fehlenden Gliedmaßen wieder her. Von den Toten zurückzukehren, ist eine wahre Prüfung für das Ziel. Es erleidet einen Malus von -4 auf alle Angriffs-, Rettungs- und Attributswürfe. Immer wenn es eine lange Rast beendet, reduziert sich der Malus um 1, bis er aufgehoben ist. Wirkst du den Zauber, um eine Kreatur zum Leben zu erwecken, die länger als 1 Jahr tot ist, bedeutet das eine große Anstrengung für dich. Bis du eine lange Rast beendet hast, kannst du keine weiteren Zauber wirken und bist im Nachteil bei allen Attributs-, Angriffs- und Rettungswürfen. 