---
aliases: 
  - Message
tags: 
  - Zauber
Grad: 0
Schule: "[[Verwandlungszauber|Verwandlung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 36 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: ein kurzes Stück Kupferdraht
Dauer: 1 Runde
Konzentration: false
Ritual: false
Skalierbar: false
Klassen:
  - "[[Zauberer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du deutest mit dem Finger auf eine Kreatur in Reichweite und flüsterst eine Botschaft. 
Das Ziel (und nur dieses) hört die Botschaft und kann in einem Flüstern antworten, das nur du zu hören vermagst.

 Du darfst diesen Zauber durch feste Gegenstände wirken wenn du mit dem Ziel vertraut bist und weißt, dass es sich hinter der Barriere befindet. 
 Magische Stille, 30 cm Stein, 2,5 cm gewöhnliches Metall, eine dünne Schicht Blei oder 90 cm Holz blockieren den Zauber. 
 Der Effekt muss keiner geraden Linie folgen und kann sich frei um Ecken oder durch Öffnungen bewegen.