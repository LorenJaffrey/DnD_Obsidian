# `=this.file.name`

Mache einen Wurf auf [[Überlebenskunst]].
Wenn du nicht [[Übung|geübt]] in [[Überlebenskunst]] bist, füge deinen [[Übung|Übungsbonus]] für die [[Kräuterkunde-Ausrüstung]] zum Wurf hinzu.
Wenn du [[Übung|geübt]] in [[Überlebenskunst]] bist erhältst du [[Vorteil und Nachteil|Vorteil]] auf den Wurf.

Der [[Schwierigkeitsgrad|SG]] basiert auf der Umgebung gemäß der untenstehenden Tabelle. 
Jeder Versuch, Zutaten zu sammeln, dauert 1 Stunde Zeit, wobei die Verfügbarkeit von Zutaten in der Umgebung anhand der jeweiligen Tabelle bestimmt wird.

```dataview
TABLE WITHOUT ID
file.link AS "Umgebung",
Such-DC AS "Schwierigkeitsgrad"
FROM #Umgebung
SORT Such-DC, file.name
```

## Such-Modifikatoren
| Typ                            |          Such-Modifikator          |
| ------------------------------ |:----------------------------------:|
| Schnelles Tempo                |           nicht möglich            |
| Langsames Tempo                |                 +5                 |
| Extremes Wetter                |                 -5                 |
| Befestigte Wege                |                 -5                 |
| einem Fluss/Strom folgend      |                 +5                 | 
| Arktische Bedingungen / Winter | [[Vorteil und Nachteil\|Nachteil]] |
| Nacht                          | [[Vorteil und Nachteil\|Nachteil]] |

Bei einem [[Erfolg]] findest du eine Zutat aus der jeweiligen Ortstabelle.
Bei einem [[Misserfolg]] findest du nichts. 