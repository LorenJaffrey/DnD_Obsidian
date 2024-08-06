---
aliases:
tags:
  - Zauber
Grad: 1
Schule: "[[Bannzauber|Bannmagie]]"
Zeitaufwand: 1 Minute
Reichweite: 9 m
Verbal: true
Geste: true
Material: true
Materialkosten: eine winzige Glocke und ein Stück feinen Silberdrahts
Dauer: 8 Stunden
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
Wirkungsdauer:   `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Du erschaffst einen Alarm gegen unerwünschtes Eindringen.*
Wähle eine Tür, ein Fenster oder einen Bereich in Reichweite, der nicht größer als ein Würfel mit 6 m Kantenlänge sein darf. 
Bis der Zauberspruch endet, macht dich ein Alarm darauf aufmerksam, wenn eine Kreatur der [[Größenkategorie]] [[Winzig]]  oder größer in den geschützten Bereich eindringt. 
Beim Wirken des Zaubers kannst du Kreaturen festlegen, die den Alarm nicht auslösen. 
Lege außerdem fest, ob der Alarm geistig oder hörbar ist. 
Ein geistiger Alarm macht sich als Klingeln in deinem Kopf bemerkbar, wenn du dich innerhalb von 1,5 km um den geschützten Bereich aufhältst. 
Das Klingeln weckt dich, falls du schlafen solltest. 
Ein hörbarer Alarm erzeugt im Umkreis von 18 m für 10 Sekunden das Geräusch einer Handglocke.