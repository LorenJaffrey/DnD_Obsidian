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
> ![[Tiefling 1.png|350]]

|                              |                                                                            |
| ---------------------------- | -------------------------------------------------------------------------- |
| [[Kreaturtypen\|Kreaturtyp]] | `=this.Kreaturtyp`                                                         | 
| [[Größenkategorie\|Größe]]   | `=this.Größenkategorie`                                                    |
| [[Bewegungsrate]]            | `=this.Bewegungsrate*1.5 + " Meter (" + this.Bewegungsrate + " Kästchen)"` |

## Beschreibung
Verkörpert durch die Verbindung von Mensch und Dämon oder durch einen verfluchten Blutlinie, sind Tieflinge oft in der Gesellschaft ausgestoßen. 
Dennoch zeigen sie Durchhaltevermögen angesichts von Widrigkeiten. 
Ihre Vorfahren sind nicht aus den Tiefen des Ewigen Feuers hervorgekommen, um sich kleinen Rückschlägen zu ergeben!

## Merkmale
`$=dv.list(dv.current().Merkmale)`

### Celestisch
Du kennst [[Celestisch]], wenn deine [[Intelligenz|IN]] nicht negativ ist.

### Himmlische Einsicht
Du erhältst einen Bonus von +1 auf [[Motiv erkennen]].

### Feuergeboren
Du besitzt [[Schadensarten#Schadensresistenz]] gegen [[Gleißender Schaden|gleißenden Schaden]].





(Mittelgroß)

_Als Nachkommen göttlicher Wesen tragen Celestials eine Aura von Adel und Anmut. Ihre angeborene Verbindung zu den höheren Ebenen befähigt sie, den Auswirkungen von Unglück zu widerstehen und standhaft zu bleiben, wo andere schwächeln könnten._

**Hochgeboren**  
Dein benachteiligter Rettungswurf wird neutral. Du beherrschst Celestialisch, wenn dein INT nicht negativ ist.