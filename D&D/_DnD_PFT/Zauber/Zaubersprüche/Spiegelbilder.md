---
aliases:
  - Mirror Image
tags:
  - Zauber
Grad: 2
Schule: "[[Illusionszauber|Illusion]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: selbst
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: false
Klassen:
- "[[Barde]]"
- "[[Hexenmeister]]"
- "[[Zauberer]]"
- "[[Magier]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Drei illusionäre Duplikate von dir erscheinen in deinem Bereich.
Bis der Zauber endet, bewegen sie sich mit dir und ahmen deine Aktionen nach. 
Dabei verändern sie ständig ihre Position, sodass du und deine Abbilder unmöglich zu unterscheiden seid. 
Als [[Aktion]] kannst du die illusionären Duplikate jederzeit fortschicken.

Immer wenn du während der Wirkungsdauer Ziel eines [[Angriff|Angriffs]] wirst, würfle mit einem W20, um zu bestimmen, ob der Angriff dir gilt oder einem deiner Duplikate.

Verfügst du über alle drei Duplikate, wird ein Angriff auf eines von ihnen übertragen, wenn du eine 6 oder höher würfelst. 
Beizwei Duplikaten musst du eine 8 oder höher würfeln, bei einem Duplikat eine 11 oder höher.

Die [[Rüstungsklasse]] eines Duplikats ist 10 + den [[Geschicklichkeit#Geschicklichkeitsmodifikator]]. 
Wenn ein Angriff ein Duplikat trifft, wird es zerstört.

Ein Duplikat kann einzig und allein von einem Angriff zerstört werden, der trifft, es ignoriert alle anderen Arten von Schaden und Effekten. 
Der Zauber endet, wenn alle drei Duplikate zerstört sind.
Eine Kreatur ist nicht vom Effekt der Spiegelbilder betroffen, wenn sie nicht sehen kann, wenn sie sich auf andere Sinne als die Sicht verlässt oder wenn sie [[Illusionszauber|Illusionen]] durchschauen kann (etwa mit [[Wahre Sicht]]).