---
tags:
  - Regeln/Nimble/Charakter/Abstammung
Kreaturtyp: "[[Humanoide]]"
Größenkategorie: "[[Mittelgroß]] (150 - 180 cm)"
Bewegungsrate: 7
Vorkommen: Häufig
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
Elfen verkörpern Schnelligkeit und Anmut. 
Ihre hohen, schlanken Gestalten täuschen ihre angeborene Geschwindigkeit, Grazie und Klugheit. 
Sowohl in der Diplomatie als auch im Kampf sind sie beeindruckend und schlagen oft schnell zu, um das Schlimmste durch ein frühzeitiges Handeln zu verhindern.

## Merkmale
`$=dv.list(dv.current().Merkmale)`

### Elfisch
Du kennst [[Elfisch]], wenn deine [[Intelligenz|IN]] nicht negativ ist.