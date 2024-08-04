---
aliases:
  - Ansteckung
tags:
  - Zauber
Grad: 5
Schule: "[[Nekromantiezauber|Nekromantie]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: 7 Tage
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
Deine Berührung löst Krankheiten aus. Führe einen Nahkampf-Zauberangriff gegen eine Kreatur innerhalb deiner Reichweite aus. Bei einem Treffer wird das Ziel vergiftet. Am Ende eines jeden seiner Züge muss das Ziel einen Konstitutionsrettungswurf ablegen. Gelingen drei dieser Rettungswürfe, ist das Ziel nicht länger vergiftet und der Zauber endet. Misslingen drei Würfe, ist das Ziel nicht länger vergiftet, du kannst aber eine der unten beschriebenen Krankheiten wählen. 
Wenn die Kreatur dies getan hat, kann sie sich nicht willentlich vom Ziel entfernen. Wenn das Ziel eine beeinflusste Kreatur verletzt oder ihr anderweitig schadet, darf diese einen Weisheitsrettungswurf ablegen, um den Effekt zu beenden, wie es unten beschrieben ist. Den Effekt beenden: Wenn sich eine beeinflusste Kreatur am Ende ihres Zuges außerhalb von 18 m um das Ziel befindet und es nicht sehen kann, legt sie einen Weisheitsrettungswurf ab. Bei einem Erfolg ist die Kreatur nicht länger vom Effekt des Zaubers betroffen und begreift, dass das Gefühl der Abstoßung oder Anziehung magischer Natur ist. Außerdem darf eine Kreatur, die unter dem Einfluss dieses Zaubers steht (solange dieser wirkt), alle 24 Stunden einen weiteren Rettungswurf ablegen. Eine Kreatur, der ein Rettungswurf gegen den Effekt gelingt, ist für eine 1 Minute gegen seine Auswirkungen immun. Danach kann er wieder in Kraft treten.