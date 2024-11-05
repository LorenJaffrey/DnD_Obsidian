## Zaubertricks
```dataview
TABLE WITHOUT ID
file.link AS "Zauber",
Schule,
Zeitaufwand, 
Schadensart,
Schaden AS "Schaden ab Lv. 1",
SchadenLv5 AS "Schaden ab Lv. 5",
Ziel,
Reichweite, 
choice(Verbal,"X","") AS "Verbal", 
choice(Geste,"X","") AS "Geste", 
Dauer, 
choice(Konzentration,"X","") AS "Konzentration", 
choice(Ritual,"X","") AS "Ritual"
FROM #Zauber
WHERE contains(this.Zauber, file.link) AND Grad=0
SORT file.name
```

## Grad 1
```dataview
TABLE WITHOUT ID
file.link AS "Zauber",
Schule,
Zeitaufwand, 
Schadensart,
Schaden,
Ziel,
Reichweite, 
choice(Verbal,"X","") AS "Verbal", 
choice(Geste,"X","") AS "Geste", 
Dauer, 
choice(Konzentration,"X","") AS "Konzentration", 
choice(Ritual,"X","") AS "Ritual", 
choice(Skalierbar,"X","") AS "Skalierbar" 
FROM #Zauber
WHERE contains(this.Zauber, file.link) AND Grad=1
SORT file.name
```

## Grad 2
```dataview
TABLE WITHOUT ID
file.link AS "Zauber",
Schule,
Zeitaufwand, 
Schadensart,
Schaden,
Ziel,
Reichweite, 
choice(Verbal,"X","") AS "Verbal", 
choice(Geste,"X","") AS "Geste", 
Dauer, 
choice(Konzentration,"X","") AS "Konzentration", 
choice(Ritual,"X","") AS "Ritual", 
choice(Skalierbar,"X","") AS "Skalierbar" 
FROM #Zauber
WHERE contains(this.Zauber, file.link) AND Grad=2
SORT file.name
```

## Grad 3
```dataview
TABLE WITHOUT ID
file.link AS "Zauber",
Schule,
Zeitaufwand, 
Schadensart,
Schaden,
Ziel,
Reichweite, 
choice(Verbal,"X","") AS "Verbal", 
choice(Geste,"X","") AS "Geste", 
Dauer, 
choice(Konzentration,"X","") AS "Konzentration", 
choice(Ritual,"X","") AS "Ritual", 
choice(Skalierbar,"X","") AS "Skalierbar" 
FROM #Zauber
WHERE contains(this.Zauber, file.link) AND Grad=3
SORT file.name
```