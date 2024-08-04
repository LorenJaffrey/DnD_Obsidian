---
aliases:
  - Ablenkung
tags:
  - Zauber
Grad: 5
Schule: "[[Illusionszauber|Illusion]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Selbst
Verbal: false
Geste: true
Material: false
Materialkosten: 
Dauer: 1 Stunde
Konzentration: true
Ritual: false
Skalierbar: false
Schaden: 
Schadensart: 
Ziel: Einzel
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du wirst unsichtbar, gleichzeitig erscheint ein illusionäres Abbild von dir selbst dort, wo du stehst. Dieses Abbild bleibt für die Wirkungsdauer bestehen, aber die Unsichtbarkeit endet, wenn du angreifst oder einen Zauber wirkst.
Als Aktion kannst du dein illusionäres Abbild bis zu deiner doppelten Bewegungsrate bewegen und es gestikulieren, sprechen und auf jede Art handeln lassen, die du möchtest. Du kannst durch seine Augen sehen und durch seine Ohren hören, als würdest du dort stehen, wo es sich aufhält.
In jedem deiner Züge kannst du als Bonusaktion von deinen Sinnen zu den Sinnen des Abbilds wechseln und andersherum. Solange du seine Sinne nutzt, bist du blind und taub für deine eigene Umgebung.
