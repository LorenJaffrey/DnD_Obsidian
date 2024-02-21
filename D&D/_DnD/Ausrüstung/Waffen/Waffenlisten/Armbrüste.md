---
aliases: Armbrust, Armbrüsten
tags:
- Waffe
---
# `=this.file.name`

```dataview
TABLE SchadenFern as "Schaden", SchadensartFern AS "Schadensart", Range1 AS "Minimalreichweite", Range2 AS "Grundreichweite", Range3 AS "Maximalreichweite", Hände AS "Hände", Gewicht, Kosten
FROM "_DnD/Ausrüstung/Waffen/Waffen" AND #Waffe/Gruppe/Armbrust
```