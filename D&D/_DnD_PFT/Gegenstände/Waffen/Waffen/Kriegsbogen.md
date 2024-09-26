---
tags:
- Gegenstand/Waffe/Art/Stichwaffe
- Gegenstand/Waffe/Gruppe/Bogen
- Gegenstand/Waffe/Klasse/Fernkampfwaffe/Schusswaffe
- Gegenstand/Waffe/Kategorie/Kriegswaffe
- Gegenstand/Waffe/Größe/Großwaffe
Reichweite:
Schaden: 
Schadensart: 
Eigenschaften: []

SchadenFern: 1d10
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
## `=this.file.name` (Fernkampf)

| Waffe             | Schaden                           | Art                     |     Hände     |     Größe     | Min RW         | Gnd RW         | Max RW         | Eigenschaften             |
| ----------------- | --------------------------------- | ----------------------- |:-------------:|:-------------:| -------------- | -------------- | -------------- | ------------------------- |
| `=this.file.name` | `dice: SchadenFern\|none\|noform` | `=this.SchadensartFern` | `=this.Hände` | `=this.Größe` | `=this.Range1` | `=this.Range2` | `=this.Range3` | `=this.EigenschaftenFern` |

## Handel

| Waffe             |         Gewicht |         Kosten | Kategorie         | Verfügbarkeit         |
| ----------------- | ---------------:| --------------:| ----------------- | --------------------- |
| `=this.file.name` | `=this.Gewicht` | `=this.Kosten` | `=this.Kategorie` | `=this.Verfügbarkeit` |