```dataview
LIST
FROM #Gegenstand/Rüstung
WHERE contains(this.Übung.Rüstungen, file.link) 
SORT file.name
```