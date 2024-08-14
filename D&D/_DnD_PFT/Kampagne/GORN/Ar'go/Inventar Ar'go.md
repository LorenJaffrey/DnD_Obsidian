---
Charakter: "[[Ar'go]]"
cssclass: nord
Geld:
  PM: 0
  GM: 5
  EM: 0
  SM: 0
  KM: 0
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
> 
> ##### Aktuelle Traglast: `=10+0+42.1`

## Am Körper
| Gegenstand                                  | Anzahl | Gewicht | Gesamt |
| ------------------------------------------- |:------:|:-------:|:------:|
| [[Dolch]]                                   |   2    |    1    |   2    |
| [[Kampfstab]]                               |   1    |    4    |   4    |
| [[Arkaner Fokus]] - Kristall                |   1    |    1    |   1    |
| Gewöhnliche Kleidung                        |   1    |    3    |   3    |
| Kultisten-Amulett (Symbol des Sturmdrachen) |   1    |    0    |   0    |
| **GESAMT**                                  |        |         |   10   |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->

## Schriftrollenbehälter
| Gegenstand                                                | Anzahl | Gewicht | Gesamt |
| --------------------------------------------------------- |:------:|:-------:|:------:|
| Karte der Insel (Drachenkult) und der umliegenden Gebiete |   1    |    0    |   0    |
| **GESAMT**                                                |        |         |   0    |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->

## Rucksack
| Gegenstand                                | Anzahl | Gewicht | Gesamt |
| ----------------------------------------- |:------:|:-------:|:------:|
| [[Brechstange]]                           |   1    |    5    |   5    |
| [[Hammer]]                                |   1    |    3    |   3    |
| [[Kletterhaken]]                          |   10   |  0.25   |  2.5   |
| [[Fackel]]                                |   10   |    1    |   10   |
| [[Zunderkästchen]]                        |   1    |    1    |   1    |
| [[Ration]]                                |   10   |    1    |   10   |
| [[Trinkschlauch]]                         |   1    |    0    |   0    |
| [[Seil aus Hanf]]  (Meter)                |   15   |   0.6   |   9    |
| Kompass                                   |   1    |   0.6   |  0.6   |
| Winterdecke                               |   1    |    0    |   0    |
| Ritualbuch (Drachenkult des Sturmdrachen) |   1    |    1    |   1    |
| [[Gildenabzeichen]]                       |   1    |    0    |   0    | 
| **GESAMT**                                |        |         |  42.1  |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->