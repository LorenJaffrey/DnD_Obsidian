---
tags:
Charakter: "[[Lucian]]"
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
| Gegenstand               | Anzahl | Gewicht | Gesamt |
| ------------------------ |:------:|:-------:|:------:|
| [[Dolch]]                |   1    |    1    |   1    |
| [[Gewöhnliche Kleidung]] |   1    |    3    |   3    |
| [[Lederrüstung]]         |   1    |   10    |   10   |
| GESAMT                   |        |         |   14   |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->

## Rucksack
| Gegenstand                                                          | Anzahl | Gewicht | Gesamt |
| ------------------------------------------------------------------- |:------:|:-------:|:------:|
| [[Buch der Schatten]]                                               |   1    |    3    |   3    |
| [[Gildenabzeichen]]                                                 |   1    |    1    |   1    |
| [[Zauberfokus]]                                                     |   1    |    1    |   1    |
| Glasphiole mit blauschimmernder Flüssigkeit                         |   1    |    1    |   1    |
| Tintenfässchen                                                      |   1    |    0    |   0    |
| Kleines Messer                                                      |   1    |    0    |   0    |
| Brechstange                                                         |   1    |    5    |   5    |
| Hammer                                                              |   1    |    3    |   3    |
| [[Kletterhaken]]                                                    |   10   |  0.25   |  2.5   |
| [[Ration]]                                                          |   15   |    1    |   15   |
| Hanfseil in Metern                                                  |   15   |  0.66   |  9.9   |
| Zunderkästchen                                                      |   1    |    1    |   1    |
| Fackel                                                              |   3    |    1    |   3    |
| [[Trinkschlauch]]                                                   |   1    |    4    |   4    |
| Schreibfeder                                                        |   1    |    0    |   0    |
| [[Dianthuskraut]]                                                   |   1    |    0    |   0    |
| [[Einfacher Wein (Flasche)]]                                        |   3    |   1.5   |  4.5   |
| Brief eines verstorbenen Freundes mit Frage                         |   1    |   0.1   |  0.1   |
| [[Heiltrank]]                                                       |   1    |   0.5   |  0.5   |
| Kompassrose                                                         |   1    |    1    |   1    |
| [[Glücksmünze]]                                                     |   1    |   0.1   |  0.1   |
| [[Quartz]]                                                          |   1    |    0    |   0    |
| [[Obsidianscherben]]                                                |   5    |   0.2   |   1    |
| [[Zauberstab der Magieerkennung]]                                   |   1    |    1    |   1    |
| [[Zauberschriftrollen\|Zauberschriftrolle]] ([[Person festhalten]]) |   1    |  0.25   |  0.25  |
| GESAMT                                                              |        |         | 57.85  |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->