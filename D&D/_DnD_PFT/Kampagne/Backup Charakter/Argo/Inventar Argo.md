---
Charakter: "[[Argo]]"
Geld:
  PM: 10
  GM: 100
  EM: 3
  SM: 5
  KM: 9
---
# `=this.file.name`
> [!infobox]
> ###### Geld
> | Währung | Anzahl |
> | ---- | ---- |
> | PM (10 GM)| `=this.Geld.PM` |
> | GM  (10 SM)| `=this.Geld.GM` |
> | EM  (5 SM) | `=this.Geld.EM` |
> | SM (10 KM) | `=this.Geld.SM` |
> | KM | `=this.Geld.KM` |
> 
> ##### Last
> | Type | Stat |
> | ---- | ---- |
> | Belastet | `=(this.Charakter.Attribute.Stärke*5)+1` - `=(this.Charakter.Attribute.Stärke*10)` Pfund |
> | Stark Belastet | `=(this.Charakter.Attribute.Stärke*10)+1` - `=(this.Charakter.Attribute.Stärke*15)` Pfund |
> | Maximale Traglast | `=(this.Charakter.Attribute.Stärke*15)` Pfund |
> | Maximalbelastung | `=(this.Charakter.Attribute.Stärke*30)` Pfund |

## Am Körper
| Gegenstand                   | Anzahl | Gewicht | Gesamt |
| ---------------------------- |:------:|:-------:|:------:| 
| [[Dolch]]                    |   2    |    1    |   2    |
| [[Kampfstab]]                |   1    |    4    |   1    | 
| [[Arkaner Fokus]] - Kristall |   1    |    1    |   1    |
|                              |        |         |        |
| GESAMT                       |        |         |   4    |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->

## Rucksack
| Gegenstand         | Anzahl | Gewicht | Gesamt |
| ------------------ |:------:|:-------:|:------:|
| [[Brechstange]]    |   1    |    5    |   5    |
| [[Hammer]]         |   1    |    3    |   3    |
| [[Kletterhaken]]   |   10   |  0.25   |  2.5   |
| [[Fackel]]         |   10   |    1    |   10   |
| [[Zunderkästchen]] |   1    |    1    |   1    |
| [[Ration]]         |   10   |    1    |   10   |
| [[Trinkschlauch]]  |   1    |    -    |   -    |
| [[Seil aus Hanf]]  | 15 (m) |   0.6   |   9    |
| GESAMT             |        |         |  40.5  | 
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->