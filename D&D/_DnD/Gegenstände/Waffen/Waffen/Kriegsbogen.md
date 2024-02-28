---
tags:
- Gegenstand/Waffe/Art/Stichwaffe
- Gegenstand/Waffe/Gruppe/Bogen
- Gegenstand/Waffe/Klasse/Fernkampfwaffe/Schusswaffe
- Gegenstand/Waffe/Kategorie/Kriegswaffe
- Gegenstand/Waffe/Größe/Großwaffe
Schaden: 
Schadensart: 
Eigenschaften: []

SchadenFern: 1W10
SchadensartFern: "[[Stichschaden]]"
Range1: 6(4)
Range2: 75(50)
Range3: 180(120)
EigenschaftenFern: 
- "[[Geschosse]] (Pfeile)"
- "[[Schwer]] (14)"
- "[[Rüstungsbrechend]] (1)"

Kategorie: "[[Kriegswaffen]]"
Hände: 2
Größe: 4
Gewicht: 4 Pfund
Kosten: 75 GM
Verfügbarkeit: selten
---
## Kriegsbogen

| Waffe       | Schaden | Art   | Hände | Größe | Min RW | Gnd RW | Max RW   | Eigenschaften                                                     |
| ----------- | ------- | ----- |:-----:|:-----:| ------ | ------ | -------- | ----------------------------------------------------------------- |
| Kriegsbogen | 1W10    | Stich |   2   |   4   | 6(4)   | 75(50) | 180(120) | [[Geschosse]] (Pfeile), [[Schwer]] (14), [[Rüstungsbrechend]] (1) |

## Handel

| Waffe       | Gewicht | Kosten | Kategorie   | Verfügbarkeit         |
| ----------- | -------:| ------:| ----------- | --------------------- |
| Kriegsbogen |       4 |  75 GM | Kriegswaffe | #Verfügbarkeit/selten |


## `=this.file.name` (Fernkampf)

| Waffe             | Schaden             | Art                     |     Hände     |     Größe     | Min RW         | Gnd RW         | Max RW         | Eigenschaften             |
| ----------------- | ------------------- | ----------------------- |:-------------:|:-------------:| -------------- | -------------- | -------------- | ------------------------- |
| `=this.file.name` | `=this.SchadenFern` | `=this.SchadensartFern` | `=this.Hände` | `=this.Größe` | `=this.Range1` | `=this.Range2` | `=this.Range3` | `=this.EigenschaftenFern` |

## Handel

| Waffe             |         Gewicht |         Kosten | Kategorie         | Verfügbarkeit         |
| ----------------- | ---------------:| --------------:| ----------------- | --------------------- |
| `=this.file.name` | `=this.Gewicht` | `=this.Kosten` | `=this.Kategorie` | `=this.Verfügbarkeit` |