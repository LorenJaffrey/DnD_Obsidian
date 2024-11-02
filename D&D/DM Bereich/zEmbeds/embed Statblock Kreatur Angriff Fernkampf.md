```dataview
TABLE WITHOUT ID 
file.link AS "Waffe",
Range1 AS "Min RW",
Range2 AS "Gnd RW",
Range3 AS "Max RW",
"`dice:1d20+" + (floor(((this.Attribute.Geschicklichkeit)-10)/2)+ceil(this.Herausforderungsgrad/4)+1) + "|none|noform`" AS "Angriff",
"`dice:" + Schaden + "+" + floor(((this.Attribute.Geschicklichkeit)-10)/2) + "|none|noform`"  AS "Schaden",
Schadensart,
Eigenschaften
FROM #Angriff/Fernkampf
WHERE contains(this.Angriff.Angriffe, file.link)
SORT file.name
```