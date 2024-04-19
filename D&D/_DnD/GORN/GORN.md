# `=this.file.name`

```dataview
TABLE WITHOUT ID

file.link AS "Character", 
Hintergrund.Volk AS "Volk",
Hintergrund.Klasse AS "Klasse",
Hintergrund.Subklasse AS "Subklasse",
Hintergrund.Gesinnung AS "Gesinnung",
Hintergrund.Hintergrund AS "Hintergrund"

FROM #Charakter/GORN 

SORT file.name
```