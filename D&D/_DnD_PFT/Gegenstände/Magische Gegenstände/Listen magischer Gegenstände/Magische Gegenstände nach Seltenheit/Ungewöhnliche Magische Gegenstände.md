# `=this.file.name`

```dataview
TABLE WITHOUT ID
file.link AS "Megischer Gegenstand", 
Art, 
choice(Einstimmung,"X","") AS "Einstimmung", 
choice(Verflucht,"X","") AS "Verflucht", 
Kosten, 
Voraussetzung
FROM #Gegenstand/Magischer_Gegenstand
FROM #Magischer_Gegenstand
WHERE contains(Seltenheit, "ungewöhnlich")
SORT file.name
```