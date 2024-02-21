---
aliases: Ritual
---
# `=this.file.name`
Bestimmte Zauber sind in ihrer Beschreibung als [[Rituale]] gekennzeichnet. 
Diese können sowohl nach den normalen Regeln gewirkt werden als auch nach den Regeln für [[Rituale]].
Einen Zauber als [[Rituale|Ritual]] zu wirken, erhöht seinen [[Zauber wirken#Zeitaufwand]] um 10 Minuten.

Ein [[Rituale|Ritual]] verbraucht zudem keinen [[Zauberplätze|Zauberplatz]], was auch bedeutet, dass die Ritualversion eines Spruches nicht auf einem höheren Grad gewirkt werden kann.

Um einen Zauber als [[Rituale|Ritual]] wirken zu können, muss der Zauberwirker ein Merkmal besitzen, das ihm dies erlaubt (wie etwa der [[Kleriker]] und der [[Druide]]). Er muss den Spruch außerdem vorbereitet oder auf seiner Liste bekannter Zauber haben, es sei denn, das [[Rituale|Ritual]]-Merkmal des Charakters gibt es anders an, wie es beim Magier der Fall ist.

```dataview
TABLE schule AS "Schule", zeitaufwand AS "Zeitaufwand", reichweite AS "Reichweite", verbal AS "Verbal", geste AS "Geste", material AS "Material", dauer AS "Dauer", konzentration AS "Konzentration", ritual AS "Ritual", skalierbar AS "Skalierbar" 
FROM #Zauber/Ritual
SORT file.name
```