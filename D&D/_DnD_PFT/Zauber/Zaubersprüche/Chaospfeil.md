---
aliases:
  - Chaos Bolt
tags:
  - Zauber/Offensiv
Grad: 1
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 36 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Schaden: 2W8 + 1W6
Schadensart: "[[Zufallsschaden]]"
Ziel: Einzel
Klassen:
  - "[[Zauberer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du schleuderst eine wogende Masse chaotischer Energie auf eine Kreatur in Reichweite. 
Führe einen Fernkampf-Zauberangriff gegen das Ziel durch. 
Bei einem Treffer erleidet das Ziel 2W8 + 1W6 Schaden. 
Wähle einen der beiden W8 aus. Die gewürfelte Zahl bestimmt die Schadensart wie unten aufgeführt.

| W8  | Schadensart             |
|:---:| ----------------------- |
|  1  | [[Säureschaden]]        |
|  2  | [[Kälteschaden]]        |
|  3  | [[Feuerschaden]]        |
|  4  | [[Energieschaden]]      |
|  5  | [[Blitzschaden]]        |
|  6  | [[Giftschaden]]         |
|  7  | [[Psychischer Schaden]] |
|  8  | [[Schallschaden]]       |

Wenn du auf beiden Würfeln dieselbe Zahl erzielst, springt die chaotische Energie vom Ziel bis zu 9 m weit zu einer anderen Kreatur deiner Wahl. 
Führe gegen das neue Ziel einen neuen [[Angriffswurf]] durch, und führe auch einen neuen [[Schadenswurf]] durch. 
Dieser könnte die Energie erneut überspringen lassen. 
Eine Kreatur kann bei jedem Wirken dieses Zaubers nur einmal zu dessen Ziel werden.

### Auf höheren Graden
Wenn du diesen Zauber mit einem [[Zauberplätze|Zauberplatz]] des 2. Grades oder höher wirkst, nimmt jedes Ziel für jeden [[Zaubergrad]] über dem ersten 1W6 zusätzlichen Schaden vom erwürfelten Typ.

Quelle: Xanathars Ratgeber für alles, Seite: 152