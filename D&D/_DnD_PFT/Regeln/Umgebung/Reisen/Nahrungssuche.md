# `=this.file.name`
Im Zuge einer [[Lange Rast|Langen Rast]] kann ein Gruppenmitglied auf Nahrungssuche gehen.
Der [[Schwierigkeitsgrad]] richtet sich dabei nach der Umgebung in der gesucht wird, sowie den Umständen der Suche anhand der untenstehenden Tabellen.
Bei Erfolg findet das Gruppenmitglied genügend Nahrung und Wasser um eine [[lange Rast]] durchzuführen und die Wasservorräte aufzufüllen

```dataview
TABLE WITHOUT ID
file.link AS "Umgebung",
Such-DC AS "Schwierigkeitsgrad"
FROM #Umgebung
SORT Such-DC, file.name
```

## Such-Modifikatoren
Das Finden von Nahrung wird von vielen Faktoren beeinflusst. 
Wie schnell bewegt sich die Gruppe? Wie ist das Wetter? Liegt Schnee auf dem Boden? etc. 
Wende diese Modifikatoren nach Bedarf an, wann immer die Gruppe eine DC-Weisheitsprobe (Überlebenskunst) während einer langen Reise macht.

| Typ                            |          Such-Modifikator          |
| ------------------------------ |:----------------------------------:|
| Schnelles Tempo                |           nicht möglich            |
| Langsames Tempo                |                 +5                 |
| Extremes Wetter                |                 -5                 |
| Befestigte Wege                |                 -5                 |
| einem Fluss/Strom folgend      |                 +5                 |
| Nacht                          | [[Vorteil und Nachteil\|Nachteil]] |