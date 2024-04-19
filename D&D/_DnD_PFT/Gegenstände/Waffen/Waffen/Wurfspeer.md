---
tags:
  - Gegenstand/Waffe/Art/Stichwaffe
  - Gegenstand/Waffe/Gruppe/Speer
  - Gegenstand/Waffe/Klasse/Nahkampfwaffe
  - Gegenstand/Waffe/Klasse/Fernkampfwaffe/Wurfwaffe
  - Gegenstand/Waffe/Kategorie/Einfache_Waffe
  - Gegenstand/Waffe/Größe/Großwaffe
Schaden: 1W6
Schadensart: "[[Stichschaden]]"
Eigenschaften:

SchadenFern: 1W6
SchadensartFern: "[[Stichschaden]]"
Range1: 1,5(1)
Range2: 9(6)
Range3: 36(24)
EigenschaftenFern:
- "[[Wurfwaffe]]"
- "[[Rüstungsbrechend]] (1)"

Kategorie: "[[Kriegswaffen]]"
Hände: 1
Größe: 4
Gewicht: 3 Pfund
Kosten: 2 GM
Verfügbarkeit: häufig
---
## `=this.file.name`

| Waffe             | Schaden         | Art                 |     Hände     |     Größe     | Eigenschaften         |
| ----------------- | --------------- | ------------------- |:-------------:|:-------------:| --------------------- |
| `=this.file.name` | `=this.Schaden` | `=this.Schadensart` | `=this.Hände` | `=this.Größe` | `=this.Eigenschaften` |

## `=this.file.name` (Wurf)

| Waffe             | Schaden             | Art                     |     Hände     |     Größe     | Min RW         | Gnd RW         | Max RW         | Eigenschaften             |
| ----------------- | ------------------- | ----------------------- |:-------------:|:-------------:| -------------- | -------------- | -------------- | ------------------------- |
| `=this.file.name` | `=this.SchadenFern` | `=this.SchadensartFern` | `=this.Hände` | `=this.Größe` | `=this.Range1` | `=this.Range2` | `=this.Range3` | `=this.EigenschaftenFern` |

## Handel

| Waffe             |         Gewicht |         Kosten | Kategorie         | Verfügbarkeit         |
| ----------------- | ---------------:| --------------:| ----------------- | --------------------- |
| `=this.file.name` | `=this.Gewicht` | `=this.Kosten` | `=this.Kategorie` | `=this.Verfügbarkeit` |