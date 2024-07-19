---
tags:
---
# `=this.file.name`

```dataview
TABLE Schaden, Schadensart, Hände, Größe, Eigenschaften
FROM #Gegenstand/Waffe/Art/Hiebwaffe 
SORT größe, file.name
```