# `=this.file.name`

>[!info]
>[[Schwierigkeitsgrad|SG]] = 10 + [[Herausforderungsgrad|HG]]

| Erfolgsgrad           |               | Effekt                                                                   |
| --------------------- | ------------- | ------------------------------------------------------------------------ |
| Kritischer Erfolg     | natürliche 20 | Genaue Kenntnis der Kreatur                                              |
| Dreifacher Erfolg     | W20 > SG + 10 | Kann Kreatur identifizieren, kennt mehrere Besonderheiten                |
| Doppelter Erfolg      | W20 > SG + 5  | Kann Kreatur identifizieren, kennt eine Besonderheit                     |
| Einfacher Erfolg      | W20 > SG      | Kann Kreatur identifizieren, weiß aber sonst nichts darüber              |
| Einfacher Misserfolg  | W20 < SG      | Kann Kreatur nicht identifizieren, kennt zumindest Art                   |
| Doppelter Misserfolg  | W20 < SG - 5   | Kann Kreatur nicht identifizieren                                        |
| Dreifacher Misserfolg | W20 < SG - 10  | Kann Kreatur vermeintlich identifizieren, weiß aber sonst nichts darüber |
| Kritischer Misserfolg | natürliche 1  | Kann Kreatur vermeintlich identifizieren, völlig falsche Informationen   |

## Fertigkeit zum Identifizieren
```dataview
TABLE Identifizieren
FROM #Kreatur/Typ 
SORT file.name
```