---
tags:
  - Gegenstand/Waffe/Art/Stichwaffe
  - Gegenstand/Waffe/Gruppe/Bogen
  - Gegenstand/Waffe/Klasse/Fernkampfwaffe/Schusswaffe
  - Gegenstand/Waffe/Kategorie/Einfache_Waffe
  - Gegenstand/Waffe/Größe/Einhandwaffe
Schaden: 
Schadensart: 
Eigenschaften: []
SchadenFern: 1d6
SchadensartFern: "[[Stichschaden]]"
Range1: 1,5(1)
Range2: 24(16)
Range3: 96(64)
EigenschaftenFern:
  - "[[Geschosse]] (Pfeile)"
Kategorie: "[[Einfache Waffen]]"
Hände: 2
Größe: 1
Gewicht: 2 Pfund
Kosten: 50 GM
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