# `=this.file.name`

>[!info]
>[[Schwierigkeitsgrad|SG]] = 10 + [[Herausforderungsgrad|HG]]

| Erfolgsgrad           |               | Effekt                                         |
| --------------------- | ------------- | ---------------------------------------------- |
| Kritischer Erfolg     | natürliche 20 | Normaler Loot + 1 sehr seltener Loot           |
| Dreifacher Erfolg     | W20 > SG + 10 | Normaler Loot + 2 seltener Loot                |
| Doppelter Erfolg      | W20 > SG + 5  | Normaler Loot + 1 seltener Loot                |
| Einfacher Erfolg      | W20 > SG      | Normaler Loot                                  |
| Einfacher Misserfolg  | W20 < SG      | halber normaler Loot                           |
| Doppelter Misserfolg  | W20 < SG -5   | halber normaler Loot beschädigt                |
| Dreifacher Misserfolg | W20 < SG -10  | Loot zerstört                                  |
| Kritischer Misserfolg | natürliche 1  | Loot zerstört, beim Ausnehmen selbst geschadet |

## Fertigkeit zum Plündern
```dataview
TABLE Plündern
FROM #Kreatur/Typ 
SORT file.name
```