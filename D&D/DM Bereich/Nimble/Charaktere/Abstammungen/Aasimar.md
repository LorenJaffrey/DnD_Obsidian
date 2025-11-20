---
tags:
  - Regeln/Nimble/Charakter/Abstammung
Kreaturtyp: "[[Humanoide]]"
Größenkategorie: "[[Mittelgroß]] (120 - 210 cm) oder [[Klein]] (60 - 120 cm)" 
Bewegungsrate: 6
Vorkommen: Ungewöhnlich
Merkmale:
  - "[[Heilende Hände]]"
---
# `=this.file.name`
> [!recite|right no-title fit] `=this.file.name`
> ![[Aasimar.png|400]]

|                              |                                                                            |
| ---------------------------- | -------------------------------------------------------------------------- |
| [[Kreaturtypen\|Kreaturtyp]] | `=this.Kreaturtyp`                                                         | 
| [[Größenkategorie\|Größe]]   | `=this.Größenkategorie`                                                    |
| [[Bewegungsrate]]            | `=this.Bewegungsrate*1.5 + " Meter (" + this.Bewegungsrate + " Kästchen)"` |

## Beschreibung
Als Nachkommen göttlicher Wesen tragen Celestials eine Aura von Adel und Anmut. 
Ihre angeborene Verbindung zu den höheren Ebenen befähigt sie, den Auswirkungen von Unglück zu widerstehen und standhaft zu bleiben, wo andere schwächeln könnten.

## Merkmale
`$=dv.list(dv.current().Merkmale)`

### Celestisch
Du kennst [[Celestisch]], wenn deine [[Intelligenz|IN]] nicht negativ ist.

### Himmlische Einsicht
Du erhältst einen Bonus von +1 auf [[Motiv erkennen]].

### Feuergeboren
Du besitzt [[Schadensarten#Schadensresistenz]] gegen [[Gleißender Schaden|gleißenden Schaden]].