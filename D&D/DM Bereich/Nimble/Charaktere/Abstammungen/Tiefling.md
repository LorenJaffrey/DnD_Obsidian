---
tags:
  - Regeln/Nimble/Charakter/Abstammung
Kreaturtyp: "[[Humanoide]]"
Größenkategorie: "[[Mittelgroß]] (120 - 210 cm) oder [[Klein]] (90 - 120 cm)" 
Bewegungsrate: 6
Vorkommen: Ungewöhnlich
Merkmale:
  - "[[Aufmerksam]]"
---
# `=this.file.name`
> [!recite|right no-title fit] `=this.file.name`
> ![[elf_highelf.png|350]]

|                              |                         |
| ---------------------------- | ----------------------- |
| [[Kreaturtypen\|Kreaturtyp]] | `=this.Kreaturtyp`      |
| [[Größenkategorie\|Größe]]   | `=this.Größenkategorie` |
| [[Bewegungsrate]]            | `=this.Bewegungsrate*1.5 + " Meter (" + this.Bewegungsrate + " Kästchen)"`   |

## Beschreibung
Verkörpert durch die Verbindung von Mensch und Dämon oder durch einen verfluchten Blutlinie, sind Tieflinge oft in der Gesellschaft ausgestoßen. 
Dennoch zeigen sie Durchhaltevermögen angesichts von Widrigkeiten. 
Ihre Vorfahren sind nicht aus den Tiefen des Ewigen Feuers hervorgekommen, um sich kleinen Rückschlägen zu ergeben!

## Merkmale
`$=dv.list(dv.current().Merkmale)`

### Infernalisch
Du kennst [[Infernalisch]], wenn deine [[Intelligenz|IN]] nicht negativ ist.

### Feuergeboren  
Einer deiner neutralen [[Rettungswurf|Rettungswürfe]] ist im [[Vorteil und Nachteil|Vorteil]].