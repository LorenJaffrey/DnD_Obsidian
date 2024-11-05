```dataview
LIST
FROM #Gegenstand/Werkzeug
WHERE contains(this.Übung.Werkzeuge, file.link)
SORT file.name
```