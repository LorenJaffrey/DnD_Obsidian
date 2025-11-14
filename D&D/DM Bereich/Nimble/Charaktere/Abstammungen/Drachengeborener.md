---
tags:
  - Regeln/Nimble/Charakter/Abstammung
Kreaturtyp: "[[Humanoide]]"
Größenkategorie: "[[Mittelgroß]] (150 - 210 cm)"
Bewegungsrate: 6
Vorkommen: Ungewöhnlich
Merkmale:
  - "[[Drakonischer Odem]]"
---
# `=this.file.name`
> [!recite|right no-title fit] `=this.file.name`
> ![[dragonborn.png|350]]

|                              |                         |
| ---------------------------- | ----------------------- |
| [[Kreaturtypen\|Kreaturtyp]] | `=this.Kreaturtyp`      |
| [[Größenkategorie\|Größe]]   | `=this.Größenkategorie` |
| [[Bewegungsrate]]            | `=this.Bewegungsrate*1.5 + " Meter (" + this.Bewegungsrate + " Kästchen)"`   |

## Beschreibung
In dir lodert die Seele eines Drachen, deine schuppige Haut ist hart wie geschmiedeter Stahl. 
Du bist ein Glutofen, und dein Erbe sind die Kohlen, die deine Flammen nähren. 
Rufe deinen Zorn an, sprich in der Sprache deiner Ahnen und entfessele ungezügelte Wut in deinen Angriffen.

## Merkmale
`$=dv.list(dv.current().Merkmale)`

### Drakonisch
Du sprichst [[Drakonisch]], sofern deine [[Intelligenz|IN]] nicht negativ ist.

### Drachenerbe 
Deine Schuppenhaut verleiht dir einen zusätzlichen Punkt auf deine [[Rüstungsklasse]].
Wähle außerdem eine drakonische Abstammung:

| Abstammung | Schadensart      |
| ---------- | ---------------- |
| Rot        | [[Feuerschaden]] |
| Blau       | [[Blitzschaden]] |
| Grün       | [[Giftschaden]]  |
| Schwarz    | [[Säureschaden]] |
| Weiß       | [[Kälteschaden]] |
| Gold       | [[Feuerschaden]] |
| Bronze     | [[Blitzschaden]] |
| Silber     | [[Kälteschaden]] |
| Kupfer     | [[Säureschaden]] |
| Messing    | [[Giftschaden]]  |
