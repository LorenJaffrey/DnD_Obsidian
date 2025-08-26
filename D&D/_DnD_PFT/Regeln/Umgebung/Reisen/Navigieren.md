# `=this.file.name`
Wenn die Charaktere keinem vorhandenen Pfad folgen und auch kein Geländemerkmal in Sicht ist, an dem sie sich orientieren können, riskieren sie sich zu verirren.
Unter anderem können folgende Umstände dazu führen, dass eine den Weg verliert: 
- unterirdische Gänge die sich verzweigen
- Gelände wie dichter Wald, das den Horizont verdeckt
- Verschleierndes Wetter wie starker Regen oder Nebel
- Reisen bei Nacht
- Reisen auf See, ohne den Himmel oder eine bekannte Küste zu sehen

Jedes Mal, wenn eine Gruppe sich bei einer Reise in ein neues Hex-Feld bewegt, muss sie einen Wurf auf [[Überlebenskunst]] ablegen.
Bestimmt dazu ein Gruppenmitglied als Navigator.
Der grundlegende [[Schwierigkeitsgrad]] wird von dem jeweiligen Geländetyp bestimmt in den sich die Gruppe bewegt.

```dataview
TABLE WITHOUT ID
file.link AS "Umgebung",
Navigation-DC AS "Schwierigkeitsgrad"
FROM #Umgebung
SORT Navigation-DC, file.name
```

## Navigations-Modifikatoren
Das Navigieren im Gelände wird von vielen Faktoren beeinflusst. 
Wie schnell bewegt sich die Gruppe? Wie ist das Wetter? Liegt Schnee auf dem Boden? etc. 
Wende diese Modifikatoren nach Bedarf an, wann immer die Gruppe einen Wurf auf [[Überlebenskunst]] während einer langen Reise ablegt.

| Typ             |      Navigations-Modifikator       |
| --------------- |:----------------------------------:|
| Schnelles Tempo | [[Vorteil und Nachteil\|Nachteil]] |
| Langsames Tempo | [[Vorteil und Nachteil\|Vorteil]]  |
| Extremes Wetter | [[Vorteil und Nachteil\|Nachteil]] |
| Nacht           | [[Vorteil und Nachteil\|Nachteil]] |

## Verlaufen
Wenn eine Gruppe den [[Schwierigkeitsgrad|SG]] für die Navigation in einem Gelände nicht besteht, haben sie sich verlaufen. 

Jedes Hex auf der Karte ist von sechs anderen Hexfeldern umgeben.
Jedes Mal, wenn eine verlorene Gruppe ein Hexfeld bewegt, würfle einen W3, um zufällig zu bestimmen, in welches benachbarte Hexfeld die Gruppe eintritt, und gib den Spielern nicht den aktuellen Standort der Gruppe preis. 
Solange die Gruppe verirrt ist, können die Spieler den Standort ihrer Gruppe auf ihrer Karte nicht genau bestimmen. 
Das nächste Mal, wenn ein Navigator einen Wurf auf [[Überlebenskunst]] für die Navigation erfolgreich besteht, enthülle den Spielern den tatsächlichen Standort der Gruppe.

| dice: 1d6 | Himmelsrichtung |
| --------- | --------------- |
| 1         | Norden          |
| 2         | Nord-Osten      |
| 3         | Süd-Osten       |
| 4         | Süden           |
| 5         | Süd-Westen      |
| 6         | Nord-Westen     |
^Himmelsrichtungen

`dice: [[Navigieren#^Himmelsrichtungen]]|norender|none|noform`