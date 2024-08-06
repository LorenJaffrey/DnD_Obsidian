---
Stufe: 5
Bewegung: 6
Rüstung: "[[Fellrüstung]]"
Schild: "[[Holzschild]]"
Waffen:
  - "[[Kampfstab]]"
  - "[[Krummsäbel]]"
  - "[[Schleuder]]"
Gesundheit:
  MaxTP: 38
  TP: 38
  TW: 5
  TempTP: 0
Attribute:
  Stärke: 8
  Geschicklichkeit: 14
  Konstitution: 14
  Intelligenz: 12
  Weisheit: 19
  Charisma: 11
Rettungswürfe:
  Stärke: 0
  Geschicklichkeit: 0
  Konstitution: 0
  Intelligenz: 1
  Weisheit: 1
  Charisma: 0
Fertigkeiten:
  Akrobatik: 0
  Arkane_Kunde: 1
  Athletik: 0
  Auftreten: 0
  Einschüchtern: 0
  Fingerfertigkeit: 0
  Geschichte: 0
  Heilkunde: 1
  Heimlichkeit: 0
  Mit_Tieren_umgehen: 1
  Motiv_erkennen: 0
  Nachforschungen: 0
  Naturkunde: 1
  Religion: 1
  Täuschen: 0
  Überlebenskunst: 1
  Überzeugen: 0
  Wahrnehmung: 0
Übung:
  Sprachen:
    - "[[Gemeinsprache]]"
    - "[[Elfisch]]"
    - "[[Sylvanisch]]"
    - "[[Urtümlich]]"
    - "[[Druidisch]]"
  Werkzeuge:
    - "[[Kräuterkunde-Ausrüstung]]"
    - "[[Giftmischerausrüstung]]"
  Rüstungen:
    - "[[Leichte Rüstung]]"
    - "[[Mittelschwere Rüstung]]"
  Waffen:
    - "[[Knüppel]]"
    - "[[Dolch]]"
    - "[[Wurfmesser]]"
    - "[[Wurfspeer]]"
    - "[[Streitkolben]]"
    - "[[Kampfstab]]"
    - "[[Krummsäbel]]"
    - "[[Sichel]]"
    - "[[Schleuder]]"
    - "[[Speer]]"
Aussehen:
  Geschlecht: männlich
  Alter: 45 Jahre
  Größenkategorie: "[[Mittelgroß]]"
  Größe: 180 cm
  Gewicht: 150 Pfund
  Augenfarbe: Grau
  Haarfarbe: Dunkelbraun
  Hautfarbe: Sandfarben
Merkmale:
  Volk:
    - "[[Dunkelsicht]]"
    - "[[Feenblut]]"
  Klasse:
    - "[[Die Sprache des Waldes]]"
    - "[[Druidisch]]"
    - "[[Verbesserte Tiergestalt]]"
    - "[[Geistertotem]]"
    - "[[Druidisches Zauberwirken]]"
  Talente:
    - "[[Von Feen berührt]]"
Hintergrund:
  Volk: "[[Halbelfen|Halbelf]]"
  Klasse: "[[Druide]]"
  Subklasse: "[[Zirkel des Hirten]]"
  Gesinnung: "[[Rechtschaffen Gut]]"
  Hintergrund: "[[Einsiedler]]"
Persönlichkeit:
  Persönlichkeitsmerkmale:
    - Große Empathie für alle jene die großes Leid erfahren
    - Erlangt durch Meditation innere Ruhe und Frieden
    - Gesellig und trinkfest
  Ideale: Alles Böse zu vernichten!
  Bindungen: Rache für den ausgelöschten Stamm.
  Makel:
    - Visionen, Alpträume und unkontrollierte Teleportation
InputData:
  GlücksPunkt1: false
  GlücksPunkt2: false
  GlücksPunkt3: false
  GlücksPunkt4: false
  GlücksPunkt5: false
  Erschöpfung1: true
  Erschöpfung2: false
  Erschöpfung3: false
  Erschöpfung4: false
  Erschöpfung5: false
  Erschöpfung6: false
  Erschöpfung7: false
  Erschöpfung8: false
  Erschöpfung9: false
  TiergestaltLadung1: false
  TiergestaltLadung2: false
  GeistertotemLadung: false
  NebelschrittLadung: false
  IdentifizierenLadung: false
  Stresslevel1: false
  Stresslevel2: false
  Stresslevel3: false
  Stresslevel4: false
  Stresslevel5: false
  Zauberplätze:
    Grad_1: 4
    Grad_2: 3
    Grad_3: 2
    Grad_4: 0
    Grad_5: 0
    Grad_6: 0
    Grad_7: 0
    Grad_8: 0
    Grad_9: 0
tags:
  - Charakter/GORN
---
# `=this.file.name`
> [!infobox]
> ![[Aranon.jpg]]
> ```dataviewjs 
> const Gesundheit = dv.current().Gesundheit; 
> const percentage = Math.round((Gesundheit.TP / Gesundheit.MaxTP) * 100);
> const metaBindCode = `<div style="display: flex; align-items: center; width: 100%; position: relative;">        <div style="width: 30px; text-align: center;">0</div>        <div style="flex: 1; position: relative;">            <progress id="health" max="${Gesundheit.MaxTP}" value="${Gesundheit.TP}" style="width: 100%; height: 20px;"></progress>            <span id="percentage" style="position: absolute; left: 50%; top: 50%; transform: translate(-50%, -70%); color: white; font-weight: bold;">${percentage}%</span>        </div>        <div style="width: 30px; text-align: center;">${Gesundheit.MaxTP}</div>    </div>`; 
> dv.el('div', metaBindCode); 
> ```
> ## Hintergrund
> |  |  |
> | ---- | ---- |
> | Stufe | `=this.Stufe` |
> | [[Völker\|Volk]] | `=this.Hintergrund.Volk` |
> | [[Klassen\|Klasse]] | `=this.Hintergrund.Klasse` |
> |  `$=dv.page(dv.current().Hintergrund.Klasse).Name_Subklassen` | `=this.Hintergrund.Subklasse` |
> | [[Gesinnung]] | `=this.Hintergrund.Gesinnung` |
> | [[_Übersicht Hintergründe\|Hintergrund]] | `=this.Hintergrund.Hintergrund` |
> 
> ## Aussehen
> |  |  |
> | ---- | ---- |
> | Geschlecht | `=this.Aussehen.Geschlecht` |
> | Alter | `=this.Aussehen.Alter` |
> | [[Größenkategorie]] | `=this.Aussehen.Größenkategorie` |
> | Größe | `=this.Aussehen.Größe` |
> | Gewicht | `=this.Aussehen.Gewicht` |
> | Augenfarbe | `=this.Aussehen.Augenfarbe` |
> | Haarfarbe | `=this.Aussehen.Haarfarbe` |
> | Hautfarbe | `=this.Aussehen.Hautfarbe` |
>
> ## Persönlichkeit
> ---
> ### Persönlichkeitsmerkmale 
> `=this.Persönlichkeit.Persönlichkeitsmerkmale[0]`
> `=this.Persönlichkeit.Persönlichkeitsmerkmale[1]`
> `=this.Persönlichkeit.Persönlichkeitsmerkmale[2]`
>
> ### Ideale
> `=this.Persönlichkeit.Ideale`
> 
> ### Bindungen
> `=this.Persönlichkeit.Bindungen`
> 
> ### Makel
> `=this.Persönlichkeit.Makel`

[[Übung|Übungsbonus]]:  `=ceil(this.Stufe/4)+1`
[[Initiative|Initiativebonus]]: `=floor(((this.Attribute.Geschicklichkeit)-10)/2)`


|        Eigenschaft         |                   1                    |                   2                    |                   3                    |                   4                    |                   5                    |                   6                    |                   7                    |                   8                    |                   9                    |
|:--------------------------:|:--------------------------------------:|:--------------------------------------:|:--------------------------------------:|:--------------------------------------:|:--------------------------------------:|:--------------------------------------:|:--------------------------------------:|:--------------------------------------:|:--------------------------------------:|
|  [[Glück\|Glückspunkte]]   | `INPUT[toggle:InputData.Glückspunkt1]` | `INPUT[toggle:InputData.Glückspunkt3]` | `INPUT[toggle:InputData.Glückspunkt3]` | `INPUT[toggle:InputData.Glückspunkt4]` | `INPUT[toggle:InputData.Glückspunkt5]` |                                        |                                        |                                        |                                        |
|      [[Stresslevel]]       | `INPUT[toggle:InputData.Stresslevel1]` | `INPUT[toggle:InputData.Stresslevel2]` | `INPUT[toggle:InputData.Stresslevel3]` | `INPUT[toggle:InputData.Stresslevel4]` | `INPUT[toggle:InputData.Stresslevel5]` |                                        |                                        |                                        |                                        |
| [[Erschöpft\|Erschöpfung]] | `INPUT[toggle:InputData.Erschöpfung1]` | `INPUT[toggle:InputData.Erschöpfung2]` | `INPUT[toggle:InputData.Erschöpfung3]` | `INPUT[toggle:InputData.Erschöpfung4]` | `INPUT[toggle:InputData.Erschöpfung5]` | `INPUT[toggle:InputData.Erschöpfung6]` | `INPUT[toggle:InputData.Erschöpfung7]` | `INPUT[toggle:InputData.Erschöpfung8]` | `INPUT[toggle:InputData.Erschöpfung9]` | 

## Aranon
> [!column | flex 3 ] 
>> ## Aufladungen
>> |                          |                          [[Tiergestalt]]             |                   [[Geistertotem]]                  |             [[Nebelschritt]]                          |                       [[Identifizieren]]                  |
>> | -------------- |:--------------------------------------:|:----------------------------------------:|:----------------------------------------:|:-------------------------------------------:|
>>| Maximal      | `INPUT[toggle:InputData.TiergestaltLadung1]` `INPUT[toggle:InputData.TiergestaltLadung2]` |  `INPUT[toggle:InputData.GeistertotemLadung]` | `INPUT[toggle:InputData.NebelschrittLadung]`   | `INPUT[toggle:InputData.IdentifizierenLadung]` |
>> | Aufladung |                 [[Kurze Rast]]                      |                     [[Kurze Rast]]                      |                       [[Lange Rast]]                   |                          [[Lange Rast]]                      |
>
>> ## Tiergestalten
>> ```dataview
>> TABLE WITHOUT ID
>> file.link AS "Tier",
>> HG
>> FROM #Kreatur/Tier 
>> SORT HG DESC
>> WHERE HG = "1/4" OR HG = "1/8" OR HG = 0
>> ```
>
>> ## Rasten
>>> [!column | flex 2 ]
>>>> ```meta-bind-button
>>>> label: Kurze Rast
>>>> icon: switch
>>>> hidden: false
>>>> class: ""
>>>> tooltip: ""
>>>> id: ""
>>>> style: primary
>>>> actions:
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.TiergestaltLadung1
>>>>     evaluate: false
>>>>     value: "false"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.TiergestaltLadung2
>>>>     evaluate: false
>>>>     value: "false"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.GeistertotemLadung
>>>>     evaluate: false
>>>>     value: "false"
>>>> 
>>>> ```
>>>
>>>> 
>>>> ```meta-bind-button
>>>> label: Lange Rast
>>>> icon: reset
>>>> hidden: false
>>>> class: ""
>>>> tooltip: ""
>>>> id: ""
>>>> style: destructive
>>>> actions:
>>>>   - type: updateMetadata
>>>>     bindTarget: Gesundheit.TW
>>>>     evaluate: false
>>>>     value: "5"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.TiergestaltLadung1
>>>>     evaluate: false
>>>>     value: "false"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.TiergestaltLadung2
>>>>     evaluate: false
>>>>     value: "false"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.GeistertotemLadung
>>>>     evaluate: false
>>>>     value: "false"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.NebelschrittLadung
>>>>     evaluate: false
>>>>     value: "false"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.IdentifizierenLadung
>>>>     evaluate: false
>>>>     value: "false"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.Stresslevel1
>>>>     evaluate: false
>>>>     value: "false"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.Stresslevel2
>>>>     evaluate: false
>>>>     value: "false"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.Stresslevel3
>>>>     evaluate: false
>>>>     value: "false"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.Stresslevel4
>>>>     evaluate: false
>>>>     value: "false"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.Stresslevel5
>>>>     evaluate: false
>>>>     value: "false"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.Zauberplätze.Grad_1
>>>>     evaluate: false
>>>>     value: "4"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.Zauberplätze.Grad_2
>>>>     evaluate: false
>>>>     value: "3"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.Zauberplätze.Grad_3
>>>>     evaluate: false
>>>>     value: "2"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.Zauberplätze.Grad_4
>>>>     evaluate: false
>>>>     value: "0"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.Zauberplätze.Grad_5
>>>>     evaluate: false
>>>>     value: "0"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.Zauberplätze.Grad_6
>>>>     evaluate: false
>>>>     value: "0"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.Zauberplätze.Grad_7
>>>>     evaluate: false
>>>>     value: "0"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.Zauberplätze.Grad_8
>>>>     evaluate: false
>>>>     value: "0"
>>>>   - type: updateMetadata
>>>>     bindTarget: InputData.Zauberplätze.Grad_9
>>>>     evaluate: false
>>>>     value: "0"
>>>> 
>>>> ```

## Bewegung
| Gehen                                              | [[Spurt]]                                          | [[Hochsprung]] mit Anlauf                            | [[Hochsprung]] ohne Anlauf                             | [[Weitsprung]] mit Anlauf                 | [[Weitsprung]] ohne Anlauf                  |
| -------------------------------------------------- | -------------------------------------------------- | ---------------------------------------------------- | ------------------------------------------------------ | ----------------------------------------- | ------------------------------------------- |
| `=this.Bewegung*1.5` m (`=this.Bewegung` Kästchen) | `=this.Bewegung*3` m (`=this.Bewegung*2` Kästchen) | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)` m | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)/2` m | `=round((this.Attribute.Stärke*0.3),2)` m | `=round((this.Attribute.Stärke*0.3)/2,2)` m |

## Verteidigung
> [!column | flex no-title] 
>> ## Gesundheit
>> |         | [[Trefferpunkte]]        | [[Trefferwürfel]] (`=this.Hintergrund.Klasse.Trefferwürfel`)       | [[Temporäre Trefferpunkte]] |
>> | :-------: | :------------------------: | :------------------------: | :---------------------------: |
>> | Maximal | `=this.Gesundheit.MaxTP` | `=this.Stufe`  |                             |
>> | Aktuell | `INPUT[number():Gesundheit.TP]`    |`INPUT[number():Gesundheit.TW]` | `INPUT[number():Gesundheit.TempTP]`   |
>
>>## Rüstung
>> | Rüstung         | [[Rüstungsklasse]]                                                                                             | [[Schadensreduktion]]                                                                                         |
>> | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
>> | `=this.Rüstung` `=choice(this.Schild, ", ", "")` `=choice(this.Schild, this.Schild, "")`  | `=10+floor(((this.Attribute.Geschicklichkeit)-10)/2)+choice(this.Rüstung.RP, this.Rüstung.RP, 0)` + `=choice(this.Schild, this.Schild.RP, 0)` | `=choice(this.Rüstung.SR, this.Rüstung.SR, 0)` + `=choice(this.Schild.SR, this.Schild.SR, 0)` |

## Zauber / Magie
> [!column | flex 2 ]
>> ### Zauberangriff / Zauber wirken
>> | [[Zauberattribut]] | Zauberangriffsbonus | Zauberrettungswurf-SG |
>> | ---------------------- | -------------------- | --------------------------------------------------------------------------------------- |
>> | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberattribut` | `$=Math.ceil((dv.current().Stufe/4)+1)+Math.floor(((dv.current().Attribute[dv.page(dv.page(dv.current().Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)` | `$=8+Math.ceil((dv.current().Stufe/4)+1)+Math.floor(((dv.current().Attribute[dv.page(dv.page(dv.current().Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)` |
>> 
>>---
>> ###### Bekannte Zauber
>> 
>> Zauberattribut: `$=dv.page(dv.current().Hintergrund.Klasse).Zauberattribut`
>> Zaubertricks: `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad0`
>> Bekannte Zauber: `$=dv.current().Stufe+Math.floor(((dv.current().Attribute[dv.page(dv.page(dv.current().Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)`  
> 
>>  ###### Zauberplätze
>>  
>> | Grad |    [[Zauberplätze]] Maximal     |      [[Zauberplätze]] aktuell       |
>> |:----:|:-------------------------------:|:-----------------------------------:|
>> |  1   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad1` | `INPUT[number():InputData.Zauberplätze.Grad_1]` |
>> |  2   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad2` | `INPUT[number():InputData.Zauberplätze.Grad_2]` |
>> |  3   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad3` | `INPUT[number():InputData.Zauberplätze.Grad_3]` |
>> |  4   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad4` | `INPUT[number():InputData.Zauberplätze.Grad_4]` |
>> |  5   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad5` | `INPUT[number():InputData.Zauberplätze.Grad_5]` |
>> |  6   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad6` | `INPUT[number():InputData.Zauberplätze.Grad_6]` |
>> |  7   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad7` | `INPUT[number():InputData.Zauberplätze.Grad_7]` |
>> |  8   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad8` | `INPUT[number():InputData.Zauberplätze.Grad_8]` |
>> |  9   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad9` | `INPUT[number():InputData.Zauberplätze.Grad_9]` |

## Angriff
> [!column | flex 3]
>> ### Nahkampfwaffen
>> ```dataview
>> TABLE WITHOUT ID 
>> file.link AS "Waffe",
>> Reichweite,
>> floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)+ceil(this.Stufe/4)+1 AS "Bonus",
>> Schaden+"+"+(floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)) AS "Schaden",
>> Schadensart,
>> Eigenschaften
>> FROM #Gegenstand/Waffe/Klasse/Nahkampfwaffe 
>> WHERE contains(this.Waffen, file.link)
>> SORT file.name
>> ```
>
>> ### Schusswaffen 
>> ```dataview
>> TABLE WITHOUT ID 
>> file.link AS "Waffe",
>> Range1 AS "Min RW",
>> Range2 AS "Gnd RW",
>> Range3 AS "Max RW",
>> 2+floor(((this.Attribute.Geschicklichkeit)-10)/2)+ceil(this.Stufe/4)+1 AS "Bonus",
>> SchadenFern+"+"+floor((((this.Attribute.Geschicklichkeit)-10)/2)) AS "Schaden",
>> SchadensartFern AS "Schadensart",
>> EigenschaftenFern AS "Eigenschaften"
>> FROM #Gegenstand/Waffe/Klasse/Fernkampfwaffe/Schusswaffe 
>> WHERE contains(this.Waffen, file.link)
>> SORT file.name
>> ```
> 
>> ### Wurfwaffen
>> ```dataview
>> TABLE WITHOUT ID 
>> file.link AS "Waffe",
>> Range1 AS "Min RW",
>> Range2 AS "Gnd RW",
>> Range3 AS "Max RW",
>> floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)+ceil(this.Stufe/4)+1 AS "Bonus",
>> SchadenFern+"+"+(floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)) AS "Schaden",
>> SchadensartFern AS "Schadensart",
>> EigenschaftenFern AS "Eigenschaften"
>> FROM #Gegenstand/Waffe/Klasse/Fernkampfwaffe/Wurfwaffe  
>> WHERE contains(this.Waffen, file.link)
>> SORT file.name
>> ```
>
Disclaimer: Waffen haben immer Übungsbonus...

## Stats
> [!column | flex no-title]
>> ## Attribute
>> | [[Attribute\|Attribut]] |           Attributswert            |         [[Attribute#Attributsmodifikator]]         |                                            Rettungswurfmodifikator                                             |
>> | ----------------------- |:----------------------------------:|:--------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------:|
>> | [[Stärke]]              |      `=this.Attribute.Stärke`      |      `=floor(((this.Attribute.Stärke)-10)/2)`      |           `=floor(((this.Attribute.Stärke)-10)/2)+(this.Rettungswürfe.Stärke*(ceil(this.Stufe/4)+1))`           |
>> | [[Geschicklichkeit]]    | `=this.Attribute.Geschicklichkeit` | `=min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)` | `=min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)+(this.Rettungswürfe.Geschicklichkeit*(ceil(this.Stufe/4)+1))` |
>> | [[Konstitution]]        |   `=this.Attribute.Konstitution`   |   `=floor(((this.Attribute.Konstitution)-10)/2)`   |     `=floor(((this.Attribute.Konstitution)-10)/2)+(this.Rettungswürfe.Konstitution*(ceil(this.Stufe/4)+1))`     |
>> | [[Intelligenz]]         |   `=this.Attribute.Intelligenz`    |   `=floor(((this.Attribute.Intelligenz)-10)/2)`    |      `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Rettungswürfe.Intelligenz*(ceil(this.Stufe/4)+1))`      |
>> | [[Weisheit]]            |     `=this.Attribute.Weisheit`     |     `=floor(((this.Attribute.Weisheit)-10)/2)`     |         `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Rettungswürfe.Weisheit*(ceil(this.Stufe/4)+1))`         |
>> | [[Charisma]]            |     `=this.Attribute.Charisma`     |     `=floor(((this.Attribute.Charisma)-10)/2)`     |         `=floor(((this.Attribute.Charisma)-10)/2)+(this.Rettungswürfe.Charisma*(ceil(this.Stufe/4)+1))`         |
>
>> ## Fertigkeiten
>> | [[Fertigkeiten\|Fertigkeit]] | Attribut                  |                                                                                       Fertigkeitswurfmodifikator                                                                                        | Übung                                                                                                                       |
>> | ---------------------------- | ------------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:| --------------------------------------------------------------------------------------------------------------------------- |
>> | [[Akrobatik]]                | [[Geschicklichkeit]]      |                                                 `=floor(((this.Attribute.Geschicklichkeit)-10)/2)+(this.Fertigkeiten.Akrobatik*(ceil(this.Stufe/4)+1))`                                                 | `=choice(this.Fertigkeiten.Akrobatik=2, "Expertise", choice(this.Fertigkeiten.Akrobatik=1, "Übung", ""))`                   |
>> | [[Arkane Kunde]]             | [[Intelligenz]]           |                                                  `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Arkane_Kunde*(ceil(this.Stufe/4)+1))`                                                  | `=choice(this.Fertigkeiten.Arkane_Kunde=2, "Expertise", choice(this.Fertigkeiten.Arkane_Kunde=1, "Übung", ""))`             |
>> | [[Athletik]]                 | [[Stärke]]                |                                                      `=floor(((this.Attribute.Stärke)-10)/2)+(this.Fertigkeiten.Athletik*(ceil(this.Stufe/4)+1))`                                                       | `=choice(this.Fertigkeiten.Athletik=2, "Expertise", choice(this.Fertigkeiten.Athletik=1, "Übung", ""))`                     |
>> | [[Auftreten]]                | [[Charisma]]              |                                                     `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Auftreten*(ceil(this.Stufe/4)+1))`                                                     | `=choice(this.Fertigkeiten.Auftreten=2, "Expertise", choice(this.Fertigkeiten.Auftreten=1, "Übung", ""))`                   |
>> | [[Einschüchtern]]            | [[Charisma]] / [[Stärke]] | `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Einschüchtern*(ceil(this.Stufe/4)+1))` / `=floor(((this.Attribute.Stärke)-10)/2)+(this.Fertigkeiten.Einschüchtern*(ceil(this.Stufe/4)+1))` | `=choice(this.Fertigkeiten.Einschüchtern=2, "Expertise", choice(this.Fertigkeiten.Einschüchtern=1, "Übung", ""))`           |
>> | [[Fingerfertigkeit]]         | [[Geschicklichkeit]]      |                                             `=floor(((this.Attribute.Geschicklichkeit)-10)/2)+(this.Fertigkeiten.Fingerfertigkeit*(ceil(this.Stufe/4)+1))`                                              | `=choice(this.Fertigkeiten.Fingerfertigkeit=2, "Expertise", choice(this.Fertigkeiten.Fingerfertigkeit=1, "Übung", ""))`     |
>> | [[Geschichte]]               | [[Intelligenz]]           |                                                   `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Geschichte*(ceil(this.Stufe/4)+1))`                                                   | `=choice(this.Fertigkeiten.Geschichte=2, "Expertise", choice(this.Fertigkeiten.Geschichte=1, "Übung", ""))`                 |
>> | [[Heilkunde]]                | [[Weisheit]]              |                                                     `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Heilkunde*(ceil(this.Stufe/4)+1))`                                                     | `=choice(this.Fertigkeiten.Heilkunde=2, "Expertise", choice(this.Fertigkeiten.Heilkunde=1, "Übung", ""))`                   |
>> | [[Heimlichkeit]]             | [[Geschicklichkeit]]      |                                               `=floor(((this.Attribute.Geschicklichkeit)-10)/2)+(this.Fertigkeiten.Heimlichkeit*(ceil(this.Stufe/4)+1))`                                                | `=choice(this.Fertigkeiten.Heimlichkeit=2, "Expertise", choice(this.Fertigkeiten.Heimlichkeit=1, "Übung", ""))`             |
>> | [[Mit Tieren umgehen]]       | [[Weisheit]]              |                                                `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Mit_Tieren_umgehen*(ceil(this.Stufe/4)+1))`                                                 | `=choice(this.Fertigkeiten.Mit_Tieren_umgehen=2, "Expertise", choice(this.Fertigkeiten.Mit_Tieren_umgehen=1, "Übung", ""))` |
>> | [[Motiv erkennen]]           | [[Weisheit]]              |                                                  `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Motiv_erkennen*(ceil(this.Stufe/4)+1))`                                                   | `=choice(this.Fertigkeiten.Motiv_erkennen=2, "Expertise", choice(this.Fertigkeiten.Motiv_erkennen=1, "Übung", ""))`         |
>> | [[Nachforschungen]]          | [[Intelligenz]]           |                                                `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Nachforschungen*(ceil(this.Stufe/4)+1))`                                                 | `=choice(this.Fertigkeiten.Nachforschungen=2, "Expertise", choice(this.Fertigkeiten.Nachforschungen=1, "Übung", ""))`       |
>> | [[Naturkunde]]               | [[Intelligenz]]           |                                                   `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Naturkunde*(ceil(this.Stufe/4)+1))`                                                   | `=choice(this.Fertigkeiten.Naturkunde=2, "Expertise", choice(this.Fertigkeiten.Naturkunde=1, "Übung", ""))`                 |
>> | [[Religion]]                 | [[Intelligenz]]           |                                                    `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Religion*(ceil(this.Stufe/4)+1))`                                                    | `=choice(this.Fertigkeiten.Religion=2, "Expertise", choice(this.Fertigkeiten.Religion=1, "Übung", ""))`                     |
>> | [[Täuschen]]                 | [[Charisma]]              |                                                     `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Täuschen*(ceil(this.Stufe/4)+1))`                                                      | `=choice(this.Fertigkeiten.Täuschen=2, "Expertise", choice(this.Fertigkeiten.Täuschen=1, "Übung", ""))`                     |
>> | [[Überlebenskunst]]          | [[Weisheit]]              |                                                  `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Überlebenskunst*(ceil(this.Stufe/4)+1))`                                                  | `=choice(this.Fertigkeiten.Überlebenskunst=2, "Expertise", choice(this.Fertigkeiten.Überlebenskunst=1, "Übung", ""))`       |
>> | [[Überzeugen]]               | [[Charisma]]              |                                                    `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Überzeugen*(ceil(this.Stufe/4)+1))`                                                     | `=choice(this.Fertigkeiten.Überzeugen=2, "Expertise", choice(this.Fertigkeiten.Überzeugen=1, "Übung", ""))`                 |
>> | [[Wahrnehmung]]              | [[Weisheit]]              |                                                    `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Wahrnehmung*(ceil(this.Stufe/4)+1))`                                                    | `=choice(this.Fertigkeiten.Wahrnehmung=2, "Expertise", choice(this.Fertigkeiten.Wahrnehmung=1, "Übung", ""))`               |
>>
>>[[Wahrnehmung#Passive Wahrnehmung]]: `=10+floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Wahrnehmung*(ceil(this.Stufe/4)+1))`

## Übung

> [!column | no-title]
>> ## Rüstung
>> ```dataview
>> LIST
>> FROM #Gegenstand/Rüstung 
>> WHERE contains(this.Übung.Rüstungen, file.link) 
>> SORT file.name
>> ```
>> 
>> ## Waffen
>> ```dataview
>> LIST
>> FROM #Gegenstand/Waffe 
>> WHERE contains(this.Übung.Waffen, file.link) 
>> SORT file.name
>> ```
>
>> ## Sprachen
>> ```dataview
>> LIST
>> FROM #Sprache
>> WHERE contains(this.Übung.Sprachen, file.link)
>> SORT file.name
>> ```
>> 
>> ## Werkzeuge
>> ```dataview
>> LIST
>> FROM #Gegenstand/Werkzeug 
>> WHERE contains(this.Übung.Werkzeuge, file.link)
>> SORT file.name
>> ```

## Merkmale
> [!column |  no-title]
>> ## Volksmerkmale
>> ```dataview
>> LIST
>> FROM #Merkmal
>> WHERE contains(this.Merkmale.Volk, file.link)
>> SORT file.name
>> ```
>>
>> ## Talente
>> ```dataview
>> LIST
>> FROM #Talent
>> WHERE contains(this.Merkmale.Talente, file.link)
>> SORT file.name
>> ```
>
>> ## Klassenmerkmale
>> ```dataview
>> LIST
>> FROM #Merkmal
>> WHERE contains(this.Merkmale.Klasse, file.link)
>> SORT file.name
>> ```

## Hintergrundgeschichte
* Vater Waldelf 
* Mutter Mensch (lebt in der Stadt)
* aufgewachsen im Stamm des Vaters
* Der Stamm lebte im Wald in besonderer Beziehung zu einem Einhorn
* Stamm wurde von einem bösen Wesen ausgelöscht
* Während des Angriffs schnell ausgeschaltet / getötet
* Das Einhorn wurde ebenfalls getötet und fiel auf den Halbelfen
* Durch die Berührung des Hornes überlebte der Halbelf
* Sagte durch das traumatische Erlebnis den dämonischen Mächten den Kampf an
* Leidet seit dem Angriff gelegentlich unter angsteinflössenden Visionen und Alpträumen, die er mit diversen Mitteln betäubt
* Trägt das abgetrennte Einhorn als Totem