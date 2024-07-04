---
tags:
- Gegenstand/Waffe
---

# `=this.file.name`

```dataview
TABLE Schaden, Schadensart, Hände, Größe, Eigenschaften
FROM "_DnD_PFT/Gegenstände/Waffen/Waffen" AND #Gegenstand/Waffe/Klasse/Nahkampfwaffe
SORT file.name
```