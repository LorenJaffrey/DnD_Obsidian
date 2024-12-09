---
cssclass: dnd
tags: 
Charakter: "[[Aranon]]"
Geld:
  PM: 0
  GM: 324
  EM: 0
  SM: 384
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
| [[Stab des Sommerwalds]]                  |   1    |    3    |   3    |
| [[Krummsäbel]]                            |   1    |    3    |   3    |
| Gewöhnliche Kleidung                      |   1    |    3    |   3    |
| [[Druidischer Fokus]] (Horn des Einhorns) |   1    |    0    |   0    |
| [[Rucksack]]                              |   1    |    5    |   5    |
| [[Fellrüstung]]  (voller Orkblut)         |   1    |   20    |   20   |
| GESAMT                                    |        |         |   34   |
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
| [[Ration]]                  |   12   |    1    |   12   |
| [[Trinkschlauch]]           |   1    |    4    |   4    |
| [[Seil aus Hanf]] in Metern |   13   |   0.6   |  7.8   |
| [[Einfacher Rum (Flasche)]] |   5    |   0.5   |  2.5   |
| [[Schriftrollenbehälter]]   |   1    |    1    |   1    |
| Flüssigkeit (silbrig)       |   1    |    0    |   0    |
| Pulver (schwarz)            |   1    |    0    |   0    |
| Flüssigkeit (zäh, braun)    |   1    |    0    |   0    |
| [[Gildenabzeichen]]         |   1    |    0    |   0    |
| [[Bergsilberkraut]]         |   1    |    0    |   0    |
| Wein (Flasche)              |   2    |    1    |   2    |
| [[Ring des Schutzes]]       |   1    |    0    |   0    |
| [[Aurelisbeeren]]           |   2    |    0    |   0    |
| [[Nachtlichtkelch]]         |   2    |    0    |   0    |
| Unsichtbare Karte           |        |         |  47.3  |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->