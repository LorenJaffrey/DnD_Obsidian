---
tags: 
Charakter: "[[Niptac]]"
Geld:
  PM: 0
  GM: 301
  EM: 0
  SM: 342
  KM: 95
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
| Gegenstand                           | Anzahl | Gewicht | Gesamt |
| ------------------------------------ |:------:|:-------:|:------:|
| [[Kurzschwert]]                      |   1    |    2    |   2    |
| [[Dolch]]                            |   1    |    1    |   1    |
| [[Schleuder]]                        |   1    |    0    |   0    |
| [[Leichte Armbrust]]                 |   1    |    5    |   5    |
| [[Stiefel der Elfen]]                |   1    |    1    |   1    |
| [[Rucksack]]                         |   1    |    5    |   5    |
| [[Diebeswerkzeug]]                   |   1    |    1    |   1    |
| Freundschaftsarmband                 |   1    |  0.25   |  0.25  |
| [[Beschlagene Lederrüstung]]         |   1    |   13    |   13   |
| GESAMT                               |        |         | 28.25  |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->

## Rucksack
| Gegenstand                                                      | Anzahl | Gewicht | Gesamt |
| --------------------------------------------------------------- |:------:|:-------:|:------:|
| [[Schlafsack]]                                                  |   1    |    7    |   7    |
| [[Zunderkästchen]]                                              |   1    |    1    |   1    |
| [[Fackel]]                                                      |   8    |    1    |   8    |
| [[Ration]]                                                      |   7    |    1    |   9    |
| [[Trinkschlauch]]                                               |   1    |    4    |   4    |
| [[Reisegeschirr]]                                               |   1    |    1    |   1    |
| [[Dolch]]                                                       |   5    |    1    |   5    |
| Armbrust Bolzen                                                 |   28   |  0.075  |  2.1   |
| [[Obsidianscherben]]                                            |   5    |  0.25   |  1.25  |
| [[Gildenabzeichen]]                                             |   1    |    0    |   0    |
| Baumels ekliger Eintopf (in Flasche)                            |   1    |   0.5   |  0.5   |
| Edelsteine (durchsichtig, grün)                                 |   2    |    0    |   0    |
| Edelsteine (undurchsichtig, rotbraun)                           |   5    |    0    |   0    |
| Perle                                                           |   1    |    0    |   0    |
| Jade-Statuette eines Frosches mit winzigen Goldkugeln als Augen |   1    |    0    |   0    |
| [[Heiltrank]]                                                   |   1    |   0.5   |  0.5   |
| GESAMT                                                          |        |         | 39.35  |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->