---
tags:
- Gegenstand/Waffe
---

# `=this.file.name`

```dataview
TABLE Schaden, Schadensart, Größe, Eigenschaften
FROM "_DnD/Ausrüstung/Waffen/Waffen" AND #Waffe/Klasse/Nahkampfwaffe 
WHERE Hände < 2
SORT file.name
```