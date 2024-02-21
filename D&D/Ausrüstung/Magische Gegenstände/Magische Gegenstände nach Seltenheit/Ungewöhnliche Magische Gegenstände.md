# `=this.file.name`

```dataview
TABLE Art, choice(Einstimmung,"X","") AS "Einstimmung", Kosten, Voraussetzung
FROM #Magischer_Gegenstand
WHERE contains(Seltenheit, "ungewöhnlich")
SORT file.name
```