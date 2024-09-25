---
tags:
  - Gegenstand/Waffe/Art/Stichwaffe
  - Gegenstand/Waffe/Gruppe/Messer
  - Gegenstand/Waffe/Klasse/Nahkampfwaffe
  - Gegenstand/Waffe/Klasse/Fernkampfwaffe/Wurfwaffe
  - Gegenstand/Waffe/Kategorie/Einfache_Waffe
  - Gegenstand/Waffe/Größe/Kleine_Waffe
Schaden: 1d4
Schadensart: "[[Stichschaden]]"
Eigenschaften:
  - "[[Leicht]]"
  - "[[Finesse]]"
  - "[[Kritisch]]"
SchadenFern: 1d4
SchadensartFern: "[[Stichschaden]]"
Range1: 1,5(1)
Range2: 6(4)
Range3: 18(12)
EigenschaftenFern:
  - "[[Leicht]]"
  - "[[Finesse]]"
  - "[[Kritisch]]"
  - "[[Wurfwaffe]]"
Kategorie: "[[Einfache Waffen]]"
Hände: 1
Größe: 1
Gewicht: 1 Pfund
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