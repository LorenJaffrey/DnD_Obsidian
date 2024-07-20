---
tags:
Charakter: "[[Aranon]]"
Zaubertricks: 3
Bekannte_Zauber: 4
Zauberplätze:
  Grad_1: 4
  Grad_2: 3
  Grad_3: 0
  Grad_4: 0
  Grad_5: 0
  Grad_6: 0
  Grad_7: 0
  Grad_8: 0
  Grad_9: 0
Zauber:
  - "[[Gift versprühen]]"
  - "[[Druidenkunst]]"
  - "[[Shillelagh]]"
  - "[[Donnerwoge]]"
  - "[[Wunden heilen]]"
  - "[[Mit Tieren sprechen]]"
  - "[[Nebelschritt]]"
  - "[[Identifizieren]]"
  - "[[Heilendes Wort]]"
  - "[[Schwache Genesung]]"
  - "[[Fallen finden]]"
  - "[[Spurloses Gehen]]"
---
# `=this.file.name`

> [!infobox]
> ###### Zauber wirken
> [[Zauberangriffswürfe|Zauberangriffsbonus]]: `$=Math.ceil((dv.page(dv.current().Charakter).Stufe/4)+1)+Math.floor(((dv.page(dv.current().Charakter).Attribute[dv.page(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)`
> [[Zauberrettungswurf-Schwierigkeitsgrad|Zauberrettungswurf-SG]]: `$=8+Math.ceil((dv.page(dv.current().Charakter).Stufe/4)+1)+Math.floor(((dv.page(dv.current().Charakter).Attribute[dv.page(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)`
> ###### Bekannte Zauber
> Zauberattribut: `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut`
> Zaubertricks: `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberplätze["Stufe"+dv.page(dv.current().Charakter).Stufe].Grad0`
> Bekannte Zauber: `$=if(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Art_Bekannte_Zauber=="Tabelle"){dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Bekannte_Zauber["Stufe"+dv.page(dv.current().Charakter).Stufe]}else{if(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).file.name=="Paladin"){dv.page(dv.current().Charakter).Stufe+Math.floor(((dv.page(dv.current().Charakter).Attribute[dv.page(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)/2}else{dv.page(dv.current().Charakter).Stufe+Math.floor(((dv.page(dv.current().Charakter).Attribute[dv.page(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)}}` 
>---
> ###### Zauberplätze
> | Grad |    [[Zauberplätze]] Maximal     |      [[Zauberplätze]] aktuell       |
> |:----:|:-------------------------------:|:-----------------------------------:|
> |  1   | `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberplätze["Stufe"+dv.page(dv.current().Charakter).Stufe].Grad1` | `INPUT[number():Zauberplätze.Grad_1]` |
> |  2   | `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberplätze["Stufe"+dv.page(dv.current().Charakter).Stufe].Grad2` | `INPUT[number():Zauberplätze.Grad_2]` |
> |  3   | `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberplätze["Stufe"+dv.page(dv.current().Charakter).Stufe].Grad3` | `INPUT[number():Zauberplätze.Grad_3]` |
> |  4   | `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberplätze["Stufe"+dv.page(dv.current().Charakter).Stufe].Grad4` | `INPUT[number():Zauberplätze.Grad_4]` |
> |  5   | `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberplätze["Stufe"+dv.page(dv.current().Charakter).Stufe].Grad5` | `INPUT[number():Zauberplätze.Grad_5]` |
> |  6   | `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberplätze["Stufe"+dv.page(dv.current().Charakter).Stufe].Grad6` | `INPUT[number():Zauberplätze.Grad_6]` |
> |  7   | `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberplätze["Stufe"+dv.page(dv.current().Charakter).Stufe].Grad7` | `INPUT[number():Zauberplätze.Grad_7]` |
> |  8   | `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberplätze["Stufe"+dv.page(dv.current().Charakter).Stufe].Grad8` | `INPUT[number():Zauberplätze.Grad_8]` |
> |  9   | `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberplätze["Stufe"+dv.page(dv.current().Charakter).Stufe].Grad9` | `INPUT[number():Zauberplätze.Grad_9]` |

## Bemerkungen
![[Von Feen berührt#Feenmagie]]
## Zaubertricks
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
choice(Material,"X","") AS "Material", 
choice(Materialkosten, "X", "") AS "Materialkosten", 
Dauer, 
choice(Konzentration,"X","") AS "Konzentration", 
choice(Ritual,"X","") AS "Ritual", 
choice(Skalierbar,"X","") AS "Skalierbar" 
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
choice(Material,"X","") AS "Material", 
choice(Materialkosten, "X", "") AS "Materialkosten", 
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
choice(Material,"X","") AS "Material", 
choice(Materialkosten, "X", "") AS "Materialkosten", 
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
choice(Material,"X","") AS "Material", 
choice(Materialkosten, "X", "") AS "Materialkosten", 
Dauer, 
choice(Konzentration,"X","") AS "Konzentration", 
choice(Ritual,"X","") AS "Ritual", 
choice(Skalierbar,"X","") AS "Skalierbar" 
FROM #Zauber
WHERE contains(this.Zauber, file.link) AND Grad=3
SORT file.name
```

## Grad 4
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
choice(Material,"X","") AS "Material", 
choice(Materialkosten, "X", "") AS "Materialkosten", 
Dauer, 
choice(Konzentration,"X","") AS "Konzentration", 
choice(Ritual,"X","") AS "Ritual", 
choice(Skalierbar,"X","") AS "Skalierbar" 
FROM #Zauber
WHERE contains(this.Zauber, file.link) AND Grad=4
SORT file.name
```

## Grad 5
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
choice(Material,"X","") AS "Material", 
choice(Materialkosten, "X", "") AS "Materialkosten", 
Dauer, 
choice(Konzentration,"X","") AS "Konzentration", 
choice(Ritual,"X","") AS "Ritual", 
choice(Skalierbar,"X","") AS "Skalierbar" 
FROM #Zauber
WHERE contains(this.Zauber, file.link) AND Grad=5
SORT file.name
```

## Grad 6
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
choice(Material,"X","") AS "Material", 
choice(Materialkosten, "X", "") AS "Materialkosten", 
Dauer, 
choice(Konzentration,"X","") AS "Konzentration", 
choice(Ritual,"X","") AS "Ritual", 
choice(Skalierbar,"X","") AS "Skalierbar" 
FROM #Zauber
WHERE contains(this.Zauber, file.link) AND Grad=6
SORT file.name
```

## Grad 7
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
choice(Material,"X","") AS "Material", 
choice(Materialkosten, "X", "") AS "Materialkosten", 
Dauer, 
choice(Konzentration,"X","") AS "Konzentration", 
choice(Ritual,"X","") AS "Ritual", 
choice(Skalierbar,"X","") AS "Skalierbar" 
FROM #Zauber
WHERE contains(this.Zauber, file.link) AND Grad=7
SORT file.name
```

## Grad 8
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
choice(Material,"X","") AS "Material", 
choice(Materialkosten, "X", "") AS "Materialkosten", 
Dauer, 
choice(Konzentration,"X","") AS "Konzentration", 
choice(Ritual,"X","") AS "Ritual", 
choice(Skalierbar,"X","") AS "Skalierbar" 
FROM #Zauber
WHERE contains(this.Zauber, file.link) AND Grad=8
SORT file.name
```

## Grad 9
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
choice(Material,"X","") AS "Material", 
choice(Materialkosten, "X", "") AS "Materialkosten", 
Dauer, 
choice(Konzentration,"X","") AS "Konzentration", 
choice(Ritual,"X","") AS "Ritual", 
choice(Skalierbar,"X","") AS "Skalierbar" 
FROM #Zauber
WHERE contains(this.Zauber, file.link) AND Grad=9
SORT file.name
```