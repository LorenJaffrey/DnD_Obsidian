---
cssclass: dnd
tags: 
Charakter: "[[Aranon]]"
Stufe: 5
Zaubertricks: 3
Bekannte_Zauber: 4
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
  - "[[Tiere beschwören]]"
  - "[[Mit Pflanzen sprechen]]"
---
# `=this.file.name`

> [!infobox]
> Aktuelle Stufe: `INPUT[number:Stufe]`
> 
> ###### Zauber wirken
> [[Zauberangriffswürfe|Zauberangriffsbonus]]: `$=Math.ceil((dv.page(dv.current().Charakter).Stufe/4)+1)+Math.floor(((dv.page(dv.current().Charakter).Attribute[dv.page(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)`
> [[Zauberrettungswurf-Schwierigkeitsgrad|Zauberrettungswurf-SG]]: `$=8+Math.ceil((dv.page(dv.current().Charakter).Stufe/4)+1)+Math.floor(((dv.page(dv.current().Charakter).Attribute[dv.page(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)`
> ###### Bekannte Zauber
> Zauberattribut: `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut`
> Zaubertricks: `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberplätze["Stufe"+dv.page(dv.current().Charakter).Stufe].Grad0`
> Bekannte Zauber: `$=if(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Art_Bekannte_Zauber=="Tabelle"){dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Bekannte_Zauber["Stufe"+dv.page(dv.current().Charakter).Stufe]}else{if(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).file.name=="Paladin"){dv.page(dv.current().Charakter).Stufe+Math.floor(((dv.page(dv.current().Charakter).Attribute[dv.page(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)/2}else{dv.page(dv.current().Charakter).Stufe+Math.floor(((dv.page(dv.current().Charakter).Attribute[dv.page(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)}}` 
>---

## Bemerkungen
![[Von Feen berührt#Feenmagie]]
```dynamic-embed
[[embed Character Sheet Alle Grade]]
```