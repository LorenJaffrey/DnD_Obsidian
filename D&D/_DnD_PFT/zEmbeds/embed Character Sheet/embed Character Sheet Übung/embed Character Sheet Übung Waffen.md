```dataview
LIST
FROM #Gegenstand/Waffe 
OR #Liste/Waffen 
WHERE contains(this.Übung.Waffen, file.link) 
SORT file.name
```