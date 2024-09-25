---
tags:
- Gegenstand/Waffe/Art/Stichwaffe
- Gegenstand/Waffe/Gruppe/Bogen
- Gegenstand/Waffe/Klasse/Fernkampfwaffe/Schusswaffe
- Gegenstand/Waffe/Kategorie/Kriegswaffe
- Gegenstand/Waffe/Größe/Anderthalbhänder
Schaden: 
Schadensart: 
Eigenschaften: []

SchadenFern: 1d8
SchadensartFern: "[[Stichschaden]]"
Range1: 3(2)
Range2: 48(32)
Range3: 135(90)
EigenschaftenFern: 
- "[[Geschosse]] (Pfeile)"

Kategorie: "[[Kriegswaffen]]"
Hände: 2
Größe: 3
Gewicht: 3 Pfund
Kosten: 100 GM
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