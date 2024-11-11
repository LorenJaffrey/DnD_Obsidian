### Wurf
```dataview
TABLE WITHOUT ID

file.link AS "Waffe",
Range1 AS "Min RW",
Range2 AS "Gnd RW",
Range3 AS "Max RW",
"`dice:1d20+" + (floor(((choice(contains(Eigenschaften, [[Finesse]]), max(this.Attribute.Geschicklichkeit,this.Attribute.Stärke), this.Attribute.Stärke))-10)/2)+ceil(this.Herausforderungsgrad/4)+1) + "`" AS "Angriff",
"`dice:" + Schaden + "+"+floor(((choice(contains(Eigenschaften, [[Finesse]]), max(this.Attribute.Geschicklichkeit,this.Attribute.Stärke), this.Attribute.Stärke))-10)/2) + "`"  AS "Schaden",
SchadensartFern AS "Schadensart",
EigenschaftenFern AS "Eigenschaften"

FROM #Gegenstand/Waffe/Klasse/Fernkampfwaffe/Wurfwaffe   
WHERE contains(this.Angriff.Angriffe, file.link)
SORT file.name
```

- [ ] #task Umbau konditional [priority:: high]