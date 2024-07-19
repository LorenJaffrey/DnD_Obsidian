---
tags:
---
# `=this.file.name`

```dataview
TABLE Schaden, Schadensart, Hände, Größe, Eigenschaften
FROM #Gegenstand/Waffe/Art/Wuchtwaffe AND #Gegenstand/Waffe/Klasse/Nahkampfwaffe 
SORT größe, file.name
```