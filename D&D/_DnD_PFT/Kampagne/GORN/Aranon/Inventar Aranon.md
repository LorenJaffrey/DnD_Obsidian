---
tags: 
Charakter: "[[Aranon]]"
Geld:
  PM: 0
  GM: 234
  EM: 0
  SM: 449
  KM: 900
---
# `=this.file.name`
> [!infobox]
> ###### Geld
> | Währung | Anzahl |
> | ---- | ---- |
> | PM (10 GM)| `INPUT[number():Geld.PM]` |
> | GM  (10 SM)| `INPUT[number():Geld.GM]` |
> | EM  (5 SM) | `INPUT[number():Geld.EM]` |
> | SM (10 KM) | `INPUT[number():Geld.SM]` |
> | KM | `INPUT[number():Geld.KM]` |
> 
> ##### Last
> | Type | Stat |
> | ---- | ---- |
> | Belastet | `=(this.Charakter.Attribute.Stärke*5)+1` - `=(this.Charakter.Attribute.Stärke*10)` Pfund |
> | Stark Belastet | `=(this.Charakter.Attribute.Stärke*10)+1` - `=(this.Charakter.Attribute.Stärke*15)` Pfund |
> | Maximale Traglast | `=(this.Charakter.Attribute.Stärke*15)` Pfund |
> | Maximalbelastung | `=(this.Charakter.Attribute.Stärke*30)` Pfund |

## Am Körper
| Gegenstand                                | Anzahl | Gewicht | Gesamt |
| ----------------------------------------- |:------:|:-------:|:------:|
| [[Kampfstab]]                             |   1    |    7    |   7    |
| [[Krummsäbel]]                            |   1    |    3    |   3    |
| Gewöhnliche Kleidung                      |   1    |    3    |   3    |
| [[Druidischer Fokus]] (Horn des Einhorns) |   1    |    0    |   0    |
| [[Rucksack]]                              |   1    |    5    |   5    |
| GESAMT                                    |        |         |   18   |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->

## Rucksack
| Gegenstand                  | Anzahl | Gewicht | Gesamt |
| --------------------------- |:------:|:-------:|:------:|
| [[Schlafsack]]              |   1    |    7    |   7    |
| [[Zunderkästchen]]          |   1    |    1    |   1    |
| [[Reisegeschirr]]           |   1    |    1    |   1    |
| [[Schleuder]]               |   1    |    1    |   1    |
| [[Holzschild]]              |   1    |    6    |   6    |
| [[Fackel]]                  |   2    |    1    |   2    |
| [[Ration]]                  |   7    |    1    |   9    |
| [[Trinkschlauch]]           |   1    |    4    |   4    |
| [[Seil aus Hanf]] in Metern |   13   |   0.6   |  7.8   |
| [[Einfacher Rum (Flasche)]] |   0    |    1    |   0    |
| [[Schriftrollenbehälter]]   |   1    |    1    |   1    |
| [[Lederrüstung]]            |   2    |   10    |   20   |
| Flüssigkeit (silbrig)       |   1    |    0    |   0    |
| Pulver (schwarz)            |   1    |    0    |   0    |
| Flüssigkeit (zäh, braun)    |   1    |    0    |   0    |
| [[Kurzschwert]]             |   1    |    2    |   2    |
| [[Gildenabzeichen]]         |   1    |    0    |   0    |
| GESAMT                      |        |         |  61.8  |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->

2x Lederrüstung, 1x Kurzschwert, 1x Leichte Armbrust, 1x Köcher mit Bolzen, 1x Heiltrank, Fellrüstung voller Orkblut, 1x Wirselkraut