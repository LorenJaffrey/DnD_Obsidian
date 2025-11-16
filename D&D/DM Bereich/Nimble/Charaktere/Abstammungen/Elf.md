---
tags:
  - Regeln/Nimble/Charakter/Abstammung
Kreaturtyp: "[[Humanoide]]"
Größenkategorie: "[[Mittelgroß]] (150 - 180 cm)"
Bewegungsrate: 6
Vorkommen: Häufig
Merkmale:
---
# `=this.file.name`
> [!recite|right no-title fit] `=this.file.name`
> ![[elf_highelf.png|350]]

|                              |                                                                            |
| ---------------------------- | -------------------------------------------------------------------------- |
| [[Kreaturtypen\|Kreaturtyp]] | `=this.Kreaturtyp`                                                         | 
| [[Größenkategorie\|Größe]]   | `=this.Größenkategorie`                                                    |
| [[Bewegungsrate]]            | `=this.Bewegungsrate*1.5 + " Meter (" + this.Bewegungsrate + " Kästchen)"` |

## Beschreibung
Elfen verkörpern Schnelligkeit und Anmut. 
Ihre hohen, schlanken Gestalten täuschen ihre angeborene Geschwindigkeit, Grazie und Klugheit. 
Sowohl in der Diplomatie als auch im Kampf sind sie beeindruckend und schlagen oft schnell zu, um das Schlimmste durch ein frühzeitiges Handeln zu verhindern.

## Merkmale
`$=dv.list(dv.current().Merkmale)`

### Elfisch
Du kennst [[Elfisch]], wenn deine [[Intelligenz|IN]] nicht negativ ist.

### Scharfe Sinne
Du erhältst einen Bonus von +1 auf [[Wahrnehmung]], [[Motiv erkennen]] und [[Überlebenskunst]].
Du erhältst außerdem [[Vorteil und Nachteil|Vorteil]] auf [[Initiative]].