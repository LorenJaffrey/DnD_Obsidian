---
tags:
  - Regeln/Nimble/Charakter/Abstammung
Kreaturtyp: "[[Humanoide]]"
Größenkategorie: "[[Mittelgroß]] (210 - 240 cm)"
Bewegungsrate: 6
Vorkommen: Ungewöhnlich
Merkmale:
  - "[[Stärke des Steins]]"
---
# `=this.file.name`
> [!recite|right no-title fit] `=this.file.name`
> ![[Half-Giant.png|350]]

|                              |                                                                            |
| ---------------------------- | -------------------------------------------------------------------------- |
| [[Kreaturtypen\|Kreaturtyp]] | `=this.Kreaturtyp`                                                         |
| [[Größenkategorie\|Größe]]   | `=this.Größenkategorie`                                                    |
| [[Bewegungsrate]]            | `=this.Bewegungsrate*1.5 + " Meter (" + this.Bewegungsrate + " Kästchen)"` |

## Beschreibung
Turmhohe Wesen, deren Stärke so unbeweglich ist wie die Berge, die sie ihr Zuhause nennen. 
Ihre schiere Größe und Widerstandskraft machen sie zu furchterregenden Gegnern, die selbst verheerende Treffer überleben können.

## Merkmale
`$=dv.list(dv.current().Merkmale)`

### Halblingisch
Du sprichst [[Riesisch]], sofern deine [[Intelligenz|IN]] nicht negativ ist.

### Verstohlen  
Du erhältst einen Bonus von +1 auf [[Athletik]]. 
Du erhältst außerdem +2 [[Inventar#Inventarplätze]].