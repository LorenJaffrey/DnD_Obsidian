# `=this.file.name`
Jede Kreatur besitzt eine [[Bewegungsrate]], welche die Distanz in Metern angibt, die sie in einer Runde zurücklegen kann.
Dieser Wert geht davon aus, dass die Bewegung in lebens-bedrohlichen Situationen in kurzen energischen Schüben stattfindet. 
Die folgenden Regeln legen fest, wie weit ein Charakter oder ein Monster in einer Minute, einer Stunde oder einem Tag kommen kann.

Während sie reist, kann eine Gruppe von Abenteurern in normalem, schnellem oder langsamem Tempo vorankommen.
Ein schnelles Reisetempo etwa lässt die Charaktere unaufmerksamer werden, wohingegen ein langsames es ermöglicht, zu schleichen und die Gegend eingehender zu untersuchen.

| Reisetempo | Minute | Stunde |   Tag | Effekt                                      |
| ---------- | ------:| ------:| -----:| ------------------------------------------- |
| Schnell    |  120 m |   6 km | 48 km | - 5 auf [[Wahrnehmung#Passive Wahrnehmung]] |
| Normal     |   90 m | 4,5 km | 36 km |                                             |
| Langsam    |   60 m |   3 km | 24 km | Einsatz von [[Heimlichkeit]] möglich        |

## Gewaltmarsch
In der Tabelle [[Reisen#Reisetempo]] wird davon ausgegangen, dass die Charaktere maximal 8 Stunden am Tag reisen. 
Diese Grenze kann auch überschritten werden, auf die Gefahr der [[Erschöpft|Erschöpfung]] hin. 
Für jede weitere Stunde über 8 hinaus legen die Charaktere die in der Stundenspalte angegebene Distanz zurück. 
Anschließend muss jeder Charakter einen [[Rettungswurf]] auf [[Konstitution]] ablegen.
Der [[Schwierigkeitsgrad]] beträgt 10 + 1 für jede Stunde über 8 hinaus. 
Bei einem Misserfolg erleidet der Charakter eine Stufe an [[Erschöpft|Erschöpfung]].

## Fahrzeuge und Reittiere
Für kurze Zeitspannen (bis zu 1 Stunde) können berittene Charaktere mit wesentlich höherer Geschwindigkeit reisen. 
Ein Reittier kann bis zu 1 Stunde galoppieren, wobei es das Doppelte der gewöhnlichen Distanz zurücklegt. 
Stehen alle acht bis zehn Meilen frische Reittiere zur Verfügung, können so auch längere Strecken überbrückt werden, was jedoch selten der Fall ist (außer in dicht besiedelten Gebieten).

Charaktere in Wagen, Karren oder anderen Landfahrzeugen wählen wie gewohnt eine Reisegeschwindigkeit.
Charaktere in Wasserfahrzeugen sind auf dessen Reisegeschwindigkeit beschränkt (siehe Kapitel 5 „Ausrüstung"), außerdem werden sie nicht von den Effekten der Reisegeschwindigkeit betroffen. 
Abhängig vom Schiffstyp und der Größe der Besatzung können Wasserfahrzeuge bis zu 24 Stunden am Tag reisen.
Bestimmte Reittiere wie Pegasi oder Greifen und auch besondere Fahrzeuge wie ein fliegender Teppich erlauben es, noch schneller zu reisen. 

## Schwieriges Gelände
Die in der Tabelle angegebenen Distanzen setzen relativ einfaches Terrain voraus: befestigte Straßen, offene Ebenen oder freie Gewölbekorridore. 
Doch Abenteurer sehen sich oft dichten Wäldern, endlosen Sümpfen, schuttübersäten Ruinen, steilen Bergketten oder vereisten Steppen gegenüber, die alle als schwieriges Gelände angesehen werden.
Durch schwieriges Gelände bewegt man sich mit halber Bewegungsrate. Um also 1 Meter in schwierigem Gelände zu bewältigen, muss man 2 Meter der Bewegungsrate aufwenden.
Dadurch legt eine Kreatur nur die Hälfte der normalen Entfernung pro Minute, Stunde oder Tag zurück.

```dataview
TABLE WITHOUT ID
file.link AS "Umgebung",
Typ
FROM #Umgebung
SORT Typ, file.name
```