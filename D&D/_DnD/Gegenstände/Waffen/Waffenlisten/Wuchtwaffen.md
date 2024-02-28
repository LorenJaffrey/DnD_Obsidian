---
tags:
- Gegenstand/Waffe
---
# `=this.file.name`

```dataview
TABLE Schaden, Schadensart, Hände, Größe, Eigenschaften
FROM "_DnD/Ausrüstung/Waffen/Waffen" AND #Waffe/Art/Wuchtwaffe AND #Waffe/Klasse/Nahkampfwaffe 
SORT größe, file.name
```