---
aliases:
  - 
tags:
  - Zauber
Grad: 2
Schule: "[[Bannzauber|Bannmagie]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: true
Materialkosten: Goldstaub im Wert von mindestens 25 GM, derbeim Wirken des Zaubers verbraucht wird
Dauer: bis der Zauber gebannt wird
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
Du berührst eine geschlossene Tür, ein Fenster, Tor, eine Kiste oder einen anderen Eingang, der für die Wirkungsdauer versiegelt wird. Du und andere Kreaturen, die du beim Wirken des Zaubers festlegst, können den Gegenstand normal öffnen. Du kannst auch ein Passwort festlegen, dass den Zauber für
1 Minute unterdrückt, wenn es innerhalb von 1,5 m um den Gegenstand ausgesprochen wird. Ansonsten ist der Durchgang nicht zu passieren, bis er zerstört oder der Zauber gebannt wird. Klopfen auf den Gegenstand zu wirken, unterdrückt Arkanes Schloss für 10 Minuten.
Solange der Gegenstand von diesem Zauber betroffen wird, ist er schwieriger zu zerstören oder aufzubrechen: Der SG eines Wurfes, um den Gegenstand zu zerbrechen oder zu knacken, steigt um 10.