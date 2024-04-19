# `=this.file.name`

```dataview
TABLE Seltenheit, choice(Einstimmung,"X","") AS "Einstimmung", Kosten, Voraussetzung
FROM #Magischer_Gegenstand/Trank/Heiltrank
SORT Seltenheit
```