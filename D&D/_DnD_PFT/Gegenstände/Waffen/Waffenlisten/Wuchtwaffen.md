---
tags:
- Gegenstand/Waffe
---
# `=this.file.name`

```dataview
TABLE Schaden, Schadensart, Hände, Größe, Eigenschaften
FROM "_DnD/Gegenstände/Waffen/Waffen" AND #Gegenstand/Waffe/Art/Wuchtwaffe AND #Gegenstand/Waffe/Klasse/Nahkampfwaffe 
SORT größe, file.name
```