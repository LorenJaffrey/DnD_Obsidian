# `=this.file.name`

```dataview
TABLE WITHOUT ID 
file.link AS "Talent", Stufe, choice(Wiederholbar,"X","") AS "Wiederholbar", aliases AS "Alias"
FROM #Talent/Herkunft 
SORT Stufe, file.name ASC
```