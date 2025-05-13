---
Charakter: "[[Ar'go]]"
cssclass: slrvb-b, dvl-o, hc, h-line, k-o, table, t-c, t-w, tbl-nalt, tag-notion, tag-bubble, tag-outline, tag-text
Zaubertricks: 5
Bekannte_Zauber: 5
Zauber:
  - "[[Gedankensplitter]]"
  - "[[Explosion der Zauberei]]"
  - "[[Klingenbann]]"
  - "[[Schockgriff]]"
  - "[[Elementalismus]]"
  - "[[Chaospfeil]]"
  - "[[Hexenpfeil]]"
  - "[[Magierrüstung]]"
  - "[[Schild]]"
  - "[[Nebelschritt]]"
  - "[[Dunkelheit]]"
  - "[[Blitz]]"
  - "[[Blitze herbeirufen]]"
  - "[[Zauber/Zaubersprüche/Fliegen|Fliegen]]"
Metamagie:
  - "[[Weitreichender Zauber]]"
  - "[[Mächtiger Zauber]]"
---
# `=this.file.name`

> [!infobox]
> ###### Zauber wirken
> 
> [[Zauberangriffswürfe|Zauberangriffsbonus]]: `$=Math.ceil((dv.page(dv.current().Charakter).Stufe/4)+1)+Math.floor(((dv.page(dv.current().Charakter).Attribute[dv.page(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)`
> [[Zauberrettungswurf-Schwierigkeitsgrad|Zauberrettungswurf-SG]]: `$=8+Math.ceil((dv.page(dv.current().Charakter).Stufe/4)+1)+Math.floor(((dv.page(dv.current().Charakter).Attribute[dv.page(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)`
> 
>---
> ###### Bekannte Zauber
> 
> Zauberattribut: `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut`
> Zaubertricks: `$=dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberplätze["Stufe"+dv.page(dv.current().Charakter).Stufe].Grad0`
> Bekannte Zauber: `$=if(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Art_Bekannte_Zauber=="Tabelle"){dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Bekannte_Zauber["Stufe"+dv.page(dv.current().Charakter).Stufe]}else{if(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).file.name=="Paladin"){dv.page(dv.current().Charakter).Stufe+Math.floor(((dv.page(dv.current().Charakter).Attribute[dv.page(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)/2}else{dv.page(dv.current().Charakter).Stufe+Math.floor(((dv.page(dv.current().Charakter).Attribute[dv.page(dv.page(dv.page(dv.current().Charakter).Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)}}`  
>

> [!column | 2  no-title]
>> ### Merkmale
>>> [!column | 2 no-title]
>>>> ![[Stürmische Magie]]
>>>> ![[Magische Führung]]
>>>
>>>> ![[Quelle der Magie#Flexibles Zauberwirken]]
>>>> ![[Quelle der Magie#Zauberplätze in Zaubereipunkte umwandeln]]
>>
>> ### Metamagie
>>> [!column | 2 no-title]
>>>> ![[Weitreichender Zauber]]
>>>
>>>> ![[Gespiegelter Zauber]]
> 
>> ### Talente ([[Kampferprobter Zauberwirker]])
>>> [!column | 2 no-title] 
>>>> ![[Kampferprobter Zauberwirker#Konzentration]]
>>>
>>>> ![[Kampferprobter Zauberwirker#Somatische Zauber]]
>>>>  ![[Kampferprobter Zauberwirker#Reaktive Zauber]]

```dynamic-embed
[[embed Character Sheet Alle Grade]]
```