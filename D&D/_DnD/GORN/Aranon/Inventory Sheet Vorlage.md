---
Charakter: "[[Character Sheet Vorlage]]"
Geld:
  PM: 0
  GM: 203
  EM: 0
  SM: 329
  KM: 900
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
| Gegenstand                | Anzahl | Gewicht | Gesamt |
| ------------------------- |:------:|:-------:|:------:|
| [[Kampfstab]]             |   1    |    7    |   7    |
| [[Krummsäbel]]            |   1    |    3    |   3    |
| [[Gewöhnliche Kleidung]]  |   1    |    3    |   3    |
| Druidischer Fokus / Totem |   1    |    0    |   0    |
| [[Gildenabzeichen]]       |   1    |    0    |   0    |
| GESAMT                    |        |         |   13   |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->

## Rucksack
| Gegenstand                | Anzahl | Gewicht | Gesamt |
| ------------------------- |:------:|:-------:|:------:|
| [[Schlafsack]]            |   1    |    5    |   5    |
| [[Zunderkästchen]]        |   1    |    1    |   1    |
| [[Reisegeschirr]]         |   1    |    1    |   1    |
| [[Schleuder]]             |   1    |    1    |   1    |
| [[Holzschild]]            |   1    |    6    |   6    |
| [[Fackel]]                |   2    |    1    |   2    |
| [[Tagesration]]           |   12   |    1    |   12   |
| [[Trinkschlauch]]         |   1    |    4    |   4    |
| [[Hanfseil]] 12m          |   1    |   10    |   10   |
| [[Schnaps]]               |   0    |    1    |   0    |
| [[Schriftrollenbehälter]] |   1    |    1    |   1    |
| GESAMT                    |        |         |   43   |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->