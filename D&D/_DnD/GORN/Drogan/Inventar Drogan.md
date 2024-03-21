---
tags:
- Charakter/GORN/Drogan
Charakter: "[[Drogan]]"
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
| Gegenstand        | Anzahl | Gewicht | Gesamt |
| ----------------- |:------:|:-------:|:------:|
| [[Zweihandaxt]]   |   1    |   10    |   10   |
| [[Streitaxt]]     |   2    |    5    |   10   |
| [[Beil]]          |   2    |    2    |   4    |
| [[Wurfspeer]]     |   4    |    2    |   8    |
| [[Rucksack]]      |   1    |    5    |   5    |
| GESAMT            |        |         |   38   |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->

## Rucksack
| Gegenstand                   | Anzahl | Gewicht | Gesamt |
| ---------------------------- |:------:|:-------:|:------:|
| [[Schlafsack]]               |   1    |    7    |   7    |
| [[Reisegeschirr]]            |   1    |    1    |   1    |
| [[Zunderkästchen]]           |   1    |    1    |   1    |
| [[Fackel]]                   |   3    |    1    |   3    |
| [[Ration]]                   |   10   |    2    |   20   |
| [[Trinkschlauch]]            |   1    |    4    |   4    |
| [[Seil aus Hanf]] in Metern  |   15   |   0.6   |   9    |
| [[Einfacher Wein (Flasche)]] |   1    |   1.5   |  1.5   |
| [[Windsporen-Pilz]]          |   1    |    0    |   0    |
| [[Obsidianscherben]]         |   5    |    1    |   5    |
| [[Tigerauge]]                |   2    |    0    |   0    |
| Sack mit Nelken              |   1    |   20    |   20   |
| kleines Goldarmband          |   1    |    0    |   0    |
| Goldohrring                  |   1    |    0    |   0    |
| Edelstein blutrot            |   1    |    0    |   0    |
| Besonderer Gegenstand        |   1    |    0    |   0    |
| GESAMT                       |        |         |  70.5  |
<!-- TBLFM: $>=($-1*$-2) -->
<!-- TBLFM: @>$>=sum(@I..@-1) -->