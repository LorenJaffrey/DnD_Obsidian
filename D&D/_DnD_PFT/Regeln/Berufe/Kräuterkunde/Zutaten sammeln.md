# `=this.file.name`
Jeder Versuch, Zutaten zu sammeln, dauert 1 Stunde Zeit, wobei die Verfügbarkeit von Zutaten in der Umgebung anhand der jeweiligen Tabelle bestimmt wird.

Um Pflanzen zu finden und  zu ernten musst du einen Wurf auf [[Naturkunde]] ablegen.
Der [[Schwierigkeitsgrad|SG]] basiert auf der Umgebung gemäß der untenstehenden Tabelle. 
Wenn du nicht [[Übung|geübt]] in [[Naturkunde]] bist, füge deinen [[Übung|Übungsbonus]] für die [[Kräuterkunde-Ausrüstung]] zum Wurf hinzu.
Wenn du [[Übung|geübt]] in [[Naturkunde]] bist erhältst du [[Vorteil und Nachteil|Vorteil]] auf den Wurf.

Wenn du den Wurf bestehst erntest du erfolgreich eine Pflanze.
Für jeden Grad des [[Erfolg|Erfolgs]] erntest du eine weitere Pflanze.

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



Wenn du den Wurf bestehst erntest du erfolgreich jeden Teil der Pflanze.
Für jeden Grad des [[Misserfolg|Misserfolgs]] verlierst du einen Pflanzenteil.