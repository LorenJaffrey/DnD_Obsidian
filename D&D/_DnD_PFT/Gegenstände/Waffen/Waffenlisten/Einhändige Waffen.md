---
tags:
---

# `=this.file.name`

```dataview
TABLE Schaden, Schadensart, Größe, Eigenschaften
FROM #Gegenstand/Waffe/Klasse/Nahkampfwaffe 
WHERE Hände < 2
SORT file.name
```