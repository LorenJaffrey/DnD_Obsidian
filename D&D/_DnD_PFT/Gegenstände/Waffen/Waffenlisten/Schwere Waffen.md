---
aliases: Schweren Waffen
tags:
---
# `=this.file.name`

```dataview
TABLE Schaden, Schadensart, Hände, Größe, Eigenschaften
FROM #Gegenstand/Waffe/Klasse/Nahkampfwaffe
WHERE contains(Eigenschaften, "Schwer")
```