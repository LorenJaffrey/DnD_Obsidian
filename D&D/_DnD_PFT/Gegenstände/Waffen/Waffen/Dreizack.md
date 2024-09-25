---
tags:
  - Gegenstand/Waffe/Art/Stichwaffe
  - Gegenstand/Waffe/Gruppe/Speer
  - Gegenstand/Waffe/Klasse/Nahkampfwaffe
  - Gegenstand/Waffe/Klasse/Fernkampfwaffe/Wurfwaffe
  - Gegenstand/Waffe/Kategorie/Kriegswaffe
  - Gegenstand/Waffe/Größe/Großwaffe
Schaden: 1d6
Schadensart: "[[Stichschaden]]"
Eigenschaften:
  - "[[Weitreichend]]"
  - "[[Vielseitig]]"
  - "[[Parieren]]"
SchadenFern: 1d6
SchadensartFern: "[[Stichschaden]]"
Range1: 1,5(1)
Range2: 6(4)
Range3: 18(12)
EigenschaftenFern:
  - "[[Wurfwaffe]]"
Kategorie: "[[Kriegswaffen]]"
Hände: 1
Größe: 4
Gewicht: 3 Pfund
Kosten: 5 GM
Verfügbarkeit: selten
---
## `=this.file.name`

| Waffe             | Schaden                       | Art                 |     Hände     |     Größe     | Eigenschaften         |
| ----------------- | ----------------------------- | ------------------- |:-------------:|:-------------:| --------------------- |
| `=this.file.name` | `dice: Schaden\|none\|noform` | `=this.Schadensart` | `=this.Hände` | `=this.Größe` | `=this.Eigenschaften` |

## `=this.file.name` (Wurf)

| Waffe             | Schaden                           | Art                     |     Hände     |     Größe     | Min RW         | Gnd RW         | Max RW         | Eigenschaften             |
| ----------------- | --------------------------------- | ----------------------- |:-------------:|:-------------:| -------------- | -------------- | -------------- | ------------------------- |
| `=this.file.name` | `dice: SchadenFern\|none\|noform` | `=this.SchadensartFern` | `=this.Hände` | `=this.Größe` | `=this.Range1` | `=this.Range2` | `=this.Range3` | `=this.EigenschaftenFern` |

## Handel

| Waffe             |         Gewicht |         Kosten | Kategorie         | Verfügbarkeit         |
| ----------------- | ---------------:| --------------:| ----------------- | --------------------- |
| `=this.file.name` | `=this.Gewicht` | `=this.Kosten` | `=this.Kategorie` | `=this.Verfügbarkeit` |