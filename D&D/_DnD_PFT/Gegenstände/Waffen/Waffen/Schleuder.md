---
tags:
  - Gegenstand/Waffe/Art/Wuchtwaffe
  - Gegenstand/Waffe/Klasse/Fernkampfwaffe/Schusswaffe
  - Gegenstand/Waffe/Kategorie/Einfache_Waffe
  - Gegenstand/Waffe/Gruppe/Schleuder
  - Gegenstand/Waffe/Größe/Einhandwaffe
Schaden: 
Schadensart: 
Eigenschaften: []
SchadenFern: 1d4
SchadensartFern: "[[Wuchtschaden]]"
Range1: 1,5(1)
Range2: 9(6)
Range3: 36(24)
EigenschaftenFern:
  - "[[Geschosse]] (Kugeln)"
  - "[[Tödlich]]"
Kategorie: "[[Einfache Waffen]]"
Hände: 1
Größe: 1
Gewicht: 
Kosten: 1 SM
Verfügbarkeit: häufig
---
## `=this.file.name` (Fernkampf)

| Waffe             | Schaden                           | Art                     |     Hände     |     Größe     | Min RW         | Gnd RW         | Max RW         | Eigenschaften             |
| ----------------- | --------------------------------- | ----------------------- |:-------------:|:-------------:| -------------- | -------------- | -------------- | ------------------------- |
| `=this.file.name` | `dice: SchadenFern\|none\|noform` | `=this.SchadensartFern` | `=this.Hände` | `=this.Größe` | `=this.Range1` | `=this.Range2` | `=this.Range3` | `=this.EigenschaftenFern` |

## Handel

| Waffe             |         Gewicht |         Kosten | Kategorie         | Verfügbarkeit         |
| ----------------- | ---------------:| --------------:| ----------------- | --------------------- |
| `=this.file.name` | `=this.Gewicht` | `=this.Kosten` | `=this.Kategorie` | `=this.Verfügbarkeit` |