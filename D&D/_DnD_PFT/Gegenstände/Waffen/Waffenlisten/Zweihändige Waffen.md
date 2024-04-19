---
tags:
- Gegenstand/Waffe
---
# `=this.file.name`

```dataview
TABLE Schaden, Schadensart, Hände, Größe, Eigenschaften
FROM "_DnD/Gegenstände/Waffen/Waffen"  AND #Gegenstand/Waffe/Klasse/Nahkampfwaffe 
WHERE Hände > 1
```