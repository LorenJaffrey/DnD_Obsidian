---
tags:
- Gegenstand/Waffe/Art/Wuchtwaffe
- Gegenstand/Waffe/Gruppe/Hammer
- Gegenstand/Waffe/Klasse/Nahkampfwaffe
- Gegenstand/Waffe/Klasse/Fernkampfwaffe/Wurfwaffe
- Gegenstand/Waffe/Kategorie/Kriegswaffe
- Gegenstand/Waffe/Größe/Einhandwaffe
Reichweite: 1,5(1)
Schaden: 1d6
Schadensart: "[[Wuchtschaden]]"
Eigenschaften:
- "[[Leicht]]"
- "[[Rüstungsbrechend]] (1)"

SchadenFern: 1d6
SchadensartFern: "[[Wuchtschaden]]"
Range1: 1,5(1)
Range2: 6(4)
Range3: 18(12)
EigenschaftenFern:
- "[[Leicht]]"
- "[[Wurfwaffe]]"

Kategorie: "[[Kriegswaffen]]"
Hände: 1
Größe: 2
Gewicht: 2 Pfund
Kosten: 2 GM
Verfügbarkeit: häufig
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