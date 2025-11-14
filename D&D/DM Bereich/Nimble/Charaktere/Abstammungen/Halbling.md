---
tags:
  - Regeln/Nimble/Charakter/Abstammung
Kreaturtyp: "[[Humanoide]]"
Größenkategorie: "[[Klein]] (80 - 110 cm)"
Bewegungsrate: 6
Vorkommen: Häufig
Merkmale:
  - "[[Glückspilz]]"
---
# `=this.file.name`
> [!recite|right no-title fit] `=this.file.name`
> ![[Halbling.png|350]]

|                              |                                                                            |
| ---------------------------- | -------------------------------------------------------------------------- |
| [[Kreaturtypen\|Kreaturtyp]] | `=this.Kreaturtyp`                                                         |
| [[Größenkategorie\|Größe]]   | `=this.Größenkategorie`                                                    |
| [[Bewegungsrate]]            | `=this.Bewegungsrate*1.5 + " Meter (" + this.Bewegungsrate + " Kästchen)"` |

## Beschreibung
So ähnlich wie ein Mensch, aber kleiner (außer den Füßen). 
Woher kommt eigentlich unser Glück? 
Nun… du kennst doch den Spruch mit den Hasenfüßen? 
Wir haben im Vergleich dazu Füße ohne Ende. 
Stell dir mal vor, wie viel Glück du in diesen kleinen Dingern stecken hast!

## Merkmale
`$=dv.list(dv.current().Merkmale)`

### Halblingisch
Du sprichst [[Halblingisch]], sofern deine [[Intelligenz|IN]] nicht negativ ist.

### Verstohlen  
Du erhältst einen Bonus von +1 auf [[Heimlichkeit]]. 