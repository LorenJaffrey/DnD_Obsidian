# `=this.file.name`
Im Zuge einer [[Lange Rast|Langen Rast]] kann ein Gruppenmitglied auf Nahrungssuche gehen.
Der Charakter macht einen Wurf auf [[Überlebenskunst]].
Der [[Schwierigkeitsgrad]] richtet sich dabei nach der Umgebung in der gesucht wird, sowie den Umständen der Suche anhand der untenstehenden Tabelle.
Extreme Wetter- oder Sichtverhältnisse können die Suche beeinflussen ([[Vorteil und Nachteil|Nachteil]]).
Bei Erfolg findet das Gruppenmitglied genügend Nahrung und Wasser um eine [[lange Rast]] durchzuführen und die Wasservorräte aufzufüllen.

```dataview
TABLE WITHOUT ID
file.link AS "Umgebung",
Such-DC AS "Schwierigkeitsgrad"
FROM #Umgebung
SORT Such-DC, file.name
```