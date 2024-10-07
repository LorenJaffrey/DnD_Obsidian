# `=this.file.name`

```dataview
TABLE WITHOUT ID
file.link AS "Megischer Gegenstand", 
Seltenheit, 
choice(Einstimmung,"X","") AS "Einstimmung", 
choice(Verflucht,"X","") AS "Verflucht", 
Kosten, 
Voraussetzung
FROM #Gegenstand/Magischer_Gegenstand/Wundersamer_Gegenstand/Stiefel
```