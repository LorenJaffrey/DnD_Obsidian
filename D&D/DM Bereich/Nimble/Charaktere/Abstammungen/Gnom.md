---
tags:
  - Regeln/Nimble/Charakter/Abstammung
Kreaturtyp: "[[Humanoide]]"
Größenkategorie: "[[Klein]] (80 - 100 cm)"
Bewegungsrate: 5
Vorkommen: Häufig
Merkmale:
  - "[[Optimistisch]]"
---
# `=this.file.name`
> [!recite|right no-title fit] `=this.file.name`
> ![[Gnom.png|350]]

|                              |                         |
| ---------------------------- | ----------------------- |
| [[Kreaturtypen\|Kreaturtyp]] | `=this.Kreaturtyp`      |
| [[Größenkategorie\|Größe]]   | `=this.Größenkategorie` |
| [[Bewegungsrate]]            | `=this.Bewegungsrate*1.5 + " Meter (" + this.Bewegungsrate + " Kästchen)"`   |

## Beschreibung
Exzentrisch, neugierig und stets optimistisch, sind Gnome fröhlich – besonders im Vergleich zu ihren meist mürrischeren und größeren Verwandten, den Zwergen. 
Bekannt für ihr Tüfteln, das Verbreiten von Heiterkeit und verspielte Streiche, verfolgen Gnome ihre Leidenschaften mit zerstreuter Begeisterung.

## Merkmale
`$=dv.list(dv.current().Merkmale)`

### Gnomisch
Du sprichst [[Gnomisch]], sofern deine [[Intelligenz|IN]] nicht negativ ist.