```dataview
TABLE WITHOUT ID 
file.link AS "Waffe",
Reichweite,
"`dice:1d20+" + (floor(((choice(contains(Eigenschaften, [[Finesse]]), max(this.Attribute.Geschicklichkeit,this.Attribute.Stärke), this.Attribute.Stärke))-10)/2)+ceil(this.Herausforderungsgrad/4)+1) + "`" AS "Angriff",
"`dice:" + Schaden + "+"+floor(((choice(contains(Eigenschaften, [[Finesse]]), max(this.Attribute.Geschicklichkeit,this.Attribute.Stärke), this.Attribute.Stärke))-10)/2) + "`"  AS "Schaden",
Schadensart,
Eigenschaften
FROM #Angriff/Nahkampf
WHERE contains(this.Angriff.Angriffe, file.link)
SORT file.name
```