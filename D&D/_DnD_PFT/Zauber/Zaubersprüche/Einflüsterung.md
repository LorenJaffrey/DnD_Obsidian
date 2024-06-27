---
aliases:
  - Suggestion
tags:
  - Zauber
Grad: 2
Schule: "[[Verzauberungen|Verzauberung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 9 m (6 Kästchen)
Verbal: true
Geste: false
Material: true
Materialkosten: 
Dauer: 8 Stunden
Konzentration: true
Ritual: false
Skalierbar: false
Klassen:
- "[[Barde]]"
- "[[Magier]]"
- "[[Hexenmeister]]"
- "[[Zauberer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du schlägst eine Vorgehensweise vor (auf einen oder zwei Sätze beschränkt) und beeinflusst auf magische Weise eine Kreatur in Reichweite, die du sehen kannst und die dich hören und verstehen kann. 
Kreaturen, die nicht [[Bezaubert]] werden können, sind gegen diesen Effekt immun. 
Die Einflüsterung muss so formuliert sein, dass die vorgeschlagene Vorgehensweise angemessen erscheint. 
Aufforderungen, sich selbst zu erstechen, sich in einen Speer zu stürzen, sich anzuzünden oder auf andere Weise zu verletzen, beenden den Zauber.

Das Ziel muss einen [[Rettungswurf]] auf [[Weisheit]] ausführen.
Scheitert der Wurf, führt es die von dir beschriebene Vorgehensweise nach Kräften aus. 
Die vorgeschlagene Vorgehensweise kann während der gesamten Wirkungsdauer fortgesetzt werden. 
Wenn die vorgeschlagene Aktivität in kürzerer Zeit abgeschlossen werden kann, endet der Zauber, sobald das Ziel die Aktivität beendet hat.

Du kannst auch Bedingungen festlegen, die während der Wirkungsdauer eine besondere Handlung auslösen. 
Du könntest zum Beispiel vorschlagen, dass ein Ritter dem ersten Bettler, den er trifft, sein Pferd schenk.
Wenn eine Bedingung vor Ablauf der Wirkungsdauer nicht erfüllt wird, so wird die Handlung nicht ausgeführt.

Wenn du oder einer deiner Begleiter das Ziel verletzt, endet der Zauber.


### Auf höheren Graden