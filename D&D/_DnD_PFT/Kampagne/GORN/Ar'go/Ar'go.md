---
cssclass: nord
Name: Ar'go
Stufe: 4
Bewegung: 6
Rüstung: 
Schild: 
Waffen:
  - "[[Kampfstab]]"
  - "[[Dolch]]"
Gesundheit:
  MaxTP: 33
  TP: 33
  TW: 4
  TempTP: 0
Attribute:
  Stärke: 8
  Geschicklichkeit: 13
  Konstitution: 16
  Intelligenz: 12
  Weisheit: 10
  Charisma: 18
Rettungswürfe:
  Stärke: 0
  Geschicklichkeit: 0
  Konstitution: 1
  Intelligenz: 0
  Weisheit: 0
  Charisma: 1
Fertigkeiten:
  Akrobatik: 0
  Arkane_Kunde: 1
  Athletik: 0
  Auftreten: 0
  Einschüchtern: 0
  Fingerfertigkeit: 0
  Geschichte: 0
  Heilkunde: 0
  Heimlichkeit: 0
  Mit_Tieren_umgehen: 0
  Motiv_erkennen: 0
  Nachforschungen: 0
  Naturkunde: 1
  Religion: 1
  Täuschen: 0
  Überlebenskunst: 0
  Überzeugen: 1
  Wahrnehmung: 0
Übung:
  Sprachen:
    - "[[Gemeinsprache]]"
    - "[[Urtümlich]]"
    - "[[Drakonisch]]"
    - "[[Celestisch]]"
  Werkzeuge:
    - "[[Navigationswerkzeug]]"
  Rüstungen: 
  Waffen:
    - "[[Dolch]]"
    - "[[Wurfmesser]]"
    - "[[Kampfstab]]"
    - "[[Leichte Armbrust]]"
Aussehen:
  Geschlecht: männlich
  Alter: 19 Jahre
  Größenkategorie: "[[Mittelgroß]]"
  Größe: 200 cm
  Gewicht: 120 Kilo
  Augenfarbe: Blau
  Haarfarbe: Dunkel Blau
  Hautfarbe: Blau
Merkmale:
  Volk:
    - "[[Odemwaffe]]"
    - "[[Drakonische Resistenz]]"
  Klasse:
    - "[[Quelle der Magie]]"
    - "[[Windsprecher]]"
    - "[[Stürmische Magie]]"
    - "[[Zauberwirken Zauberer]]"
  Talente:
    - "[[Kampferprobter Zauberwirker]]"
Hintergrund:
  Volk: "[[Drachenblütige|Drachenblütiger]]"
  Klasse: "[[Zauberer]]"
  Subklasse: "[[Sturmzauberei]]"
  Gesinnung: "[[Rechtschaffen Neutral]]"
  Hintergrund: "[[Einsiedler]]"
Persönlichkeit:
  Persönlichkeitsmerkmale:
    - <ul><b>Respekt vor der Natur</b></ul>Ar'gonthariel Maez'ralor empfindet eine tiefe Ehrfurcht vor den Elementen und dem Gleichgewicht der Natur. Er sieht sich selbst als Beschützer dieses Gleichgewichts und handelt dementsprechend.
  Ideale:
    - <ul><b>Gleichgewicht</b></ul>Das Gleichgewicht der Natur und der Elemente ist das höchste Gut und muss um jeden Preis bewahrt werden.
  Bindungen:
    - <ul><b>Tempestus-Kristall</b></ul>Die Fragmente des Kristalls sind für ihn mehr als nur ein Ziel; sie sind heilige Objekte, die er mit größtem Respekt behandelt.
  Makel:
    - <ul><b>Naivität</b></ul>Ar'gonthariel ist aufgrund seines abgeschiedenen Lebens auf einer Insel, auf der er kaum Kontakt zu Außenseitern hatte, etwas naiv und leichtgläubig. Dies kann dazu führen, dass er Menschen vertraut, die es nicht gut mit ihm meinen.
Zauber:
  - "[[Windbö]]"
  - "[[Schockgriff]]"
  - "[[Donnerschlag]]"
  - "[[Kältestrahl]]"
  - "[[Hexenpfeil]]"
  - "[[Magierrüstung]]"
  - "[[Chaospfeil]]"
  - "[[Klingenbann]]"
  - "[[Schutzwind]]"
  - "[[Snillocs Schneeballschwarm]]"
ZauberStatistik:
  Donnerschlag: 1
  Kältestrahl: 0
  Klingenbann: 0
  Schockgriff: 0
  Windbö: 0
  Chaospfeil: 0
  Hexenpfeil: 0
  Magierrüstung: 0
  Schutzwind: 0
  Snillocs_Schneeballschwarm: 0
InputData:
  Uhrzeit1: 00:00
  Uhrzeit2: 00:00
  UhrzeitToogle1: false
  UhrzeitToogle2: false
  GlücksPunkt1: false
  GlücksPunkt2: false
  GlücksPunkt3: false
  GlücksPunkt4: false
  GlücksPunkt5: false
  ErschöpfungsPunkte: 0
  Erschöpfung1: false
  Erschöpfung2: false
  Erschöpfung3: false
  Erschöpfung4: false
  Erschöpfung5: false
  Erschöpfung6: false
  Erschöpfung7: false
  Erschöpfung8: false
  Erschöpfung9: false
  NormaleRüstung: true
  MagierRüstung: false
  BlitzOdem: false
  Zauberpunkte: 17
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
tags:
  - Charakter/GORN
---

> [!infobox]
> ![[Argo.jpeg]]
> ```dataviewjs 
> const Gesundheit = dv.current().Gesundheit; 
> const percentage = Math.round((Gesundheit.TP / Gesundheit.MaxTP) * 100);
> const metaBindCode = `<div style="display: flex; align-items: center; width: 100%; position: relative;">        <div style="width: 30px; text-align: center;">0</div>        <div style="flex: 1; position: relative;">            <progress id="health" max="${Gesundheit.MaxTP}" value="${Gesundheit.TP}" style="width: 100%; height: 20px; --progress: rgb(136, 192, 208) !important;"></progress>            <span id="percentage" style="position: absolute; left: 50%; top: 50%; transform: translate(-50%, -70%); color: white; font-weight: bold;">${percentage}%</span>        </div>        <div style="width: 30px; text-align: center;">${Gesundheit.MaxTP}</div>    </div>`; 
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
> | Größenkategorie | `=this.Aussehen.Größenkategorie` |
> | Größe | `=this.Aussehen.Größe` |
> | Gewicht | `=this.Aussehen.Gewicht` |
> | Augenfarbe | `=this.Aussehen.Augenfarbe` |
> | Hornfarbe | `=this.Aussehen.Haarfarbe` |
> | Schuppenfarbe | `=this.Aussehen.Hautfarbe` |
>
> ### Persönlichkeitsmerkmale 
> `=this.Persönlichkeit.Persönlichkeitsmerkmale[0]`
> ### Ideale
> `=this.Persönlichkeit.Ideale`
> ### Bindungen
> `=this.Persönlichkeit.Bindungen`
> ### Makel
> `=this.Persönlichkeit.Makel`

#   `=this.file.name`nthariel Maez'ralor Sturmzorn
> [!column | flex 3 ]
>> ## Rasten
>> |                            |                           |
>> | -------------------------- | ------------------------- |
>> | `BUTTON[shortBreakButton]` | `BUTTON[longBreakButton]` | 
>> 
>>  ## Allgemeine Spiel - Parameter
>> | Erholungs-Art | 1 | 2 |
>> | :---: | :---: | :---: |
>> | [[Kurze Rast]]| `INPUT[toggle:InputData.UhrzeitToogle1]`| `INPUT[toggle:InputData.UhrzeitToogle2]` |
>> | Uhrzeit            | `INPUT[time():InputData.Uhrzeit1]` | `INPUT[time():InputData.Uhrzeit2]` |
>>  
>> |  Eigenschaft  |  Wert  |  
>> | :---: | :---: | 
>> | [[Übung\|Übungsbonus]]  |   `=ceil(this.Stufe/4)+1`  |
>> | [[Initiative\|Initiativebonus]]  |  `=floor(((this.Attribute.Geschicklichkeit)-10)/2)`  | 
>> 
>> | Eigenschaft  |  1  |  2  |  3  |  4  |  5  |  6  |  7  |  8  |  9  |
>> | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
>> | [[Glück\|Glückspunkte]]  | `INPUT[toggle:InputData.GlücksPunkt1]` |  `INPUT[toggle:InputData.GlücksPunkt2]` | `INPUT[toggle:InputData.GlücksPunkt3]` | `INPUT[toggle:InputData.GlücksPunkt4]` | `INPUT[toggle:InputData.GlücksPunkt5]` |  -  |  -  |  -  |  -  |
>> | [[Erschöpft\|Erschöpfung]]       |  `INPUT[toggle:InputData.Erschöpfung1]`  | `INPUT[toggle:InputData.Erschöpfung2]` |  `INPUT[toggle:InputData.Erschöpfung3]`  |  `INPUT[toggle:InputData.Erschöpfung4]`  | `INPUT[toggle:InputData.Erschöpfung5]`  |  `INPUT[toggle:InputData.Erschöpfung6]`  |  `INPUT[toggle:InputData.Erschöpfung7]`  |  `INPUT[toggle:InputData.Erschöpfung8]`  |  `INPUT[toggle:InputData.Erschöpfung9]`  |
>> 
>
>> ## Gesundheit
>> |         |  [[Trefferpunkte]]       | [[Trefferwürfel]] (`=this.Hintergrund.Klasse.Trefferwürfel`)       | [[Temporäre Trefferpunkte]] |
>> | ------- | :------------------------: | :------------------------: | :---------------------------: |
>> | Maximal | `=this.Gesundheit.MaxTP` | `=this.Stufe` |                             |
>> | Aktuell | `INPUT[number():Gesundheit.TP]`   |`INPUT[number():Gesundheit.TW]` | `INPUT[number():Gesundheit.TempTP]`   |
>>
>>
>>>[!column | flex 2 ] 
>>>>## Rüstung
>>>> | Aktiv | Rüstung         | [[Rüstungsklasse]]                                                                                             | [[Schadensreduktion]]                                                                                         |
>>>> | ------- | :--------------: | :---------------------------------------------------------------------------: | :-----------------------------------------------------------------------------: |
>>>> | `INPUT[toggle:InputData.NormaleRüstung]` | `=this.Rüstung` `=choice(this.Schild, ", ", "")` `=choice(this.Schild, this.Schild, "")`  | `=10+floor(((this.Attribute.Geschicklichkeit)-10)/2)+choice(this.Rüstung.RP, this.Rüstung.RP, 0)` + `=choice(this.Schild, this.Schild.RP, 0)`  | `=choice(this.Rüstung.SR, this.Rüstung.SR, 0)` + `=choice(this.Schild.SR, this.Schild.SR, 0)` |
>>>> | `INPUT[toggle:InputData.MagierRüstung]` |  [[Magierrüstung]]  |  `=13+floor(((this.Attribute.Geschicklichkeit)-10)/2)`| |
>>>
>>>>## [[Schadensarten#Schadensresistenz|Resistenz]]
>>>> - Blitz
>
>> ## Bewegung
>> | Gehen                                              |
>> | ---------------------------------- |
>> | `=this.Bewegung*1.5` m (`=this.Bewegung` Kästchen) | 
>>
>> | [[Spurt]]                                          |
>> | -------------------------------------------------- |
>> | `=this.Bewegung*3` m (`=this.Bewegung*2` Kästchen) | 
>>
>> | [[Hochsprung]] mit Anlauf                            | 
>> | ------------------------------------------------- | 
>> | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)` m | 
>>
>> | [[Hochsprung]] ohne Anlauf                                    |
>> | ------------------------------------------------------------- |
>> | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)/2` m | 
>>
>> | [[Weitsprung]] mit Anlauf                 | 
>> | ------------------------------------------ | 
>> | `=round((this.Attribute.Stärke*0.3),2)` m |
>>
>> | [[Weitsprung]] ohne Anlauf                  |
>> | --------------------------------------------- |
>> | `=round((this.Attribute.Stärke*0.3)/2,2)` m |
>>
>

## Stats
> [!column | flex ]
>> ## Attribute
>> | [[Attribute\|Attribut]] |           Attributswert            |         [[Attribute#Attributsmodifikator]]         |                                            Rettungswurfmodifikator                                             |
>> | ----------------------- |:----------------------------------:|:--------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------:|
>> | [[Stärke]]              |      `=this.Attribute.Stärke`      |      `=floor(((this.Attribute.Stärke)-10)/2)`      |           `=floor(((this.Attribute.Stärke)-10)/2)+(this.Rettungswürfe.Stärke*(ceil(this.Stufe/4)+1))`           |
>> | [[Geschicklichkeit]]    | `=this.Attribute.Geschicklichkeit` | `=min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)` | `=min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)+(this.Rettungswürfe.Geschicklichkeit*(ceil(this.Stufe/4)+1))` |
>> | [[Konstitution]]        |   `=this.Attribute.Konstitution`   |   `=floor(((this.Attribute.Konstitution)-10)/2)`   |     `=floor(((this.Attribute.Konstitution)-10)/2)+(this.Rettungswürfe.Konstitution*(ceil(this.Stufe/4)+1))`     |
>> | [[Intelligenz]]         |   `=this.Attribute.Intelligenz`    |   `=floor(((this.Attribute.Intelligenz)-10)/2)`    |      `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Rettungswürfe.Intelligenz*(ceil(this.Stufe/4)+1))`      |
>> | [[Weisheit]]            |     `=this.Attribute.Weisheit`     |     `=floor(((this.Attribute.Weisheit)-10)/2)`     |         `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Rettungswürfe.Weisheit*(ceil(this.Stufe/4)+1))`         |
>> | [[Charisma]]            |     `=this.Attribute.Charisma`     |     `=floor(((this.Attribute.Charisma)-10)/2)`     |         `=floor(((this.Attribute.Charisma)-10)/2)+(this.Rettungswürfe.Charisma*(ceil(this.Stufe/4)+1))`         |
>>
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
>> 
>> ### Zauberangriff / Zauber wirken
>> | [[Zauberattribut]] | Zauberangriffsbonus | Zauberrettungswurf-SG |
>> | ---------------------- | -------------------- | --------------------------------------------------------------------------------------- |
>> | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberattribut` | `$=Math.ceil((dv.current().Stufe/4)+1)+Math.floor(((dv.current().Attribute[dv.page(dv.page(dv.current().Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)` | `$=8+Math.ceil((dv.current().Stufe/4)+1)+Math.floor(((dv.current().Attribute[dv.page(dv.page(dv.current().Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)` |
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

## Aktionen
>[!column | 2 ]
>> ### Blitz-Odem
>>|  Zeitaufwand |  Schadensart |  Schaden |   Ziel   |   Reichweite  |  [[Schwierigkeitsgrad]]  |   [[Rettungswurf]] |  Erholung  |
>>| ----------------- | ----------------  | ----------- | ------- | ---------------- | -------------------  |  -------------------  | ------------  |
>>| [[Aktion]]         | [[Blitzschaden]]| `=choice(this.Stufe<6,"2W6", choice(this.Stufe<11,"3W6", choice(this.Stufe<16,"4W6","5W6")))` | AoE (Linie) | 1.5 m (breit) / 9 m (lang) |  `=8+floor(((this.Attribute.Konstitution)-10)/2)`  | [[Geschicklichkeit]] | [[Kurze Rast]], [[Lange Rast]] |
>>    
>>| Merkmal            | Verfügbar |
>>| ------------------ |:---------:|
>>| Blitz-Odem | `INPUT[toggle:InputData.BlitzOdem]`|
>> 
>> ### Metamagie
>> ![[Beschleunigter Zauber]]
>> ![[Gespiegelter Zauber]]
> 
>> ## Zaubertricks
>> ```dataview
>> TABLE WITHOUT ID
>> file.link AS "Zauber",
>> Schule,
>> Zeitaufwand, 
>> Schadensart,
>> Schaden,
>> Ziel,
>> Reichweite, 
>> choice(Verbal,"X","") AS "Verbal", 
>> choice(Geste,"X","") AS "Geste", 
>> Dauer, 
>> choice(Konzentration,"X","") AS "Konzentration", 
>> choice(Ritual,"X","") AS "Ritual", 
>> choice(Skalierbar,"X","") AS "Skalierbar" 
>> FROM #Zauber
>> WHERE contains(this.Zauber, file.link) AND Grad=0
>> SORT file.name
>> ```
>> 
>> ## Grad 1
>> ```dataview
>> TABLE WITHOUT ID
>> file.link AS "Zauber",
>> Schule,
>> Zeitaufwand, 
>> Schadensart,
>> Schaden,
>> Ziel,
>> Reichweite, 
>> choice(Verbal,"X","") AS "Verbal", 
>> choice(Geste,"X","") AS "Geste", 
>> Dauer, 
>> choice(Konzentration,"X","") AS "Konzentration", 
>> choice(Ritual,"X","") AS "Ritual", 
>> choice(Skalierbar,"X","") AS "Skalierbar" 
>> FROM #Zauber
>> WHERE contains(this.Zauber, file.link) AND Grad=1
>> SORT file.name
>> ```
>> 
>> ## Grad 2
>> ```dataview
>> TABLE WITHOUT ID
>> file.link AS "Zauber",
>> Schule,
>> Zeitaufwand, 
>> Schadensart,
>> Schaden,
>> Ziel,
>> Reichweite, 
>> choice(Verbal,"X","") AS "Verbal", 
>> choice(Geste,"X","") AS "Geste", 
>> Dauer, 
>> choice(Konzentration,"X","") AS "Konzentration", 
>> choice(Ritual,"X","") AS "Ritual", 
>> choice(Skalierbar,"X","") AS "Skalierbar" 
>> FROM #Zauber
>> WHERE contains(this.Zauber, file.link) AND Grad=2
>> SORT file.name
>> ```
>

## Zauber / Magie
> [!column | flex 3 ]
>> ###### Zauber wirken
>> 
>> [[Zauberangriffswürfe|Zauberangriffsbonus]]: `$=dv.page(dv.current().Hintergrund.Klasse).Zauberattribut` | `$=Math.ceil((dv.current().Stufe/4)+1)+Math.floor(((dv.current().Attribute[dv.page(dv.page(dv.current().Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)`
>> [[Zauberrettungswurf-Schwierigkeitsgrad|Zauberrettungswurf-SG]]: `$=8+Math.ceil((dv.current().Stufe/4)+1)+Math.floor(((dv.current().Attribute[dv.page(dv.page(dv.current().Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)`
>> 
>>---
>> ###### Bekannte Zauber
>> 
>> Zauberattribut: `$=dv.page(dv.current().Hintergrund.Klasse).Zauberattribut`
>> Zaubertricks: `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad0`
>> Bekannte Zauber: `$=if(dv.page(dv.current().Hintergrund.Klasse).Art_Bekannte_Zauber=="Tabelle"){dv.page(dv.current().Hintergrund.Klasse).Bekannte_Zauber["Stufe"+dv.current().Stufe]}else{if(dv.page(dv.current().Hintergrund.Klasse).file.name=="Paladin"){dv.current().Stufe+Math.floor(((dv.current().Attribute[dv.page(dv.current().Hintergrund.Klasse.Zauberattribut).file.name])-10)/2)/2}else{dv.current().Stufe+Math.floor(((dv.current().Attribute[dv.page(dv.current().Hintergrund.Klasse).Zauberattribut.file.name])-10)/2)}}`  
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
>
>> ###### Zauberpunkte
>> 
>> | Stufe |    [[Zauberpunkte]] Maximal     |      [[Zauberpunkte]] aktuell       |
>> |:----:|:-------------------------------:|:-----------------------------------:|
>> |  `$=dv.current().Stufe`  | `$=(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad1*2)+(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad2*3)+(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad3*5)+(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad4*6)+(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad5*7)+(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad6*9)+(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad7*10)+(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad8*11)+(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad9*13)` | `INPUT[number():InputData.Zauberpunkte]` |
>>
>> | Zauberlevel | Umwandlungskosten |
>> | ----------- |:-----------------:|
>> | Level 1     |         2         |
>> | Level 2     |         3         |
>> | Level 3     |         5         |
>> | Level 4     |         6         |
>> | Level 5     |         7         |
>> | Level 6     |          -         |
>> | Level 7     |          -         |
>> | Level 8     |          -         |
>> | Level 9     |          -         | 

## Übung / Merkmale
> [!column | 3]
>> ## Rüstung
>> 
>> ## Waffen
>> ```dataview
>> LIST
>> FROM #Gegenstand/Waffe 
>> WHERE contains(this.Übung.Waffen, file.link) 
>> SORT file.name
>> ```
>>
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
>
>> ## Talente
>> ```dataview
>> LIST
>> FROM #Talent
>> WHERE contains(this.Merkmale.Talente, file.link)
>> SORT file.name
>> ```
>>
>> ![[Kampferprobter Zauberwirker]]
>
>> ## Klassenmerkmale
>> ```dataview
>> LIST
>> FROM #Merkmal
>> WHERE contains(this.Merkmale.Klasse, file.link)
>> SORT file.name
>> ```
>> 
>> ![[Stürmische Magie]]
>> 
>> ![[Quelle der Magie#Flexibles Zauberwirken]]
>> 
>> ![[Quelle der Magie#Zauberplätze in Zaubereipunkte umwandeln]]

## Statistik

> [!column | 2]
>> ```dataviewjs
>> const currentPage = dv.current();
>> const labels = ["Donnerschlag", "Kältestrahl", "Klingenbann", "Schockgriff", "Windbö", "Chaospfeil", "Hexenpfeil", "Magierrüstung", "Schutzwind", "Snillocs Schneeballschwarm"];
>> const data = [currentPage.ZauberStatistik.Donnerschlag, currentPage.ZauberStatistik.Kältestrahl, currentPage.ZauberStatistik.Klingenbann, currentPage.ZauberStatistik.Schockgriff, currentPage.ZauberStatistik.Windbö, currentPage.ZauberStatistik.Chaospfeil, currentPage.ZauberStatistik.Hexenpfeil, currentPage.ZauberStatistik.Magierrüstung, currentPage.ZauberStatistik.Schutzwind, currentPage.ZauberStatistik.Snillocs_Schneeballschwarm];
>> 
>> const chartData = {  
>>     type: 'line',
>>     data: {
>>         labels: labels,
>>         datasets: [{
>>             label: 'Zauber Anwendungen',
>>             data: data,
>>             backgroundColor: [ 'rgb(136, 192, 208)' ],
>>             borderColor: [ 'rgb(136, 192, 208)' ],
>>             pointStyle: 'circle',
>>             pointRadius: 10,
>> 		    pointHoverRadius: 15
>>         }]
>>     },
>>     options: {
>> 	    indexAxis: 'y',
>> 	    scales: {
>> 		  min: 0,
>> 		  max: 100,		  
>> 	      x: {
>> 	        beginAtZero: true
>> 	      }
>> 	    },
>> 	    animations: {
>> 	      tension: {
>> 	        duration: 1000,
>> 	        easing: 'linear',
>> 	        from: 1,
>> 	        to: 0,
>> 	        loop: true
>> 	      }
>> 	    }
>> 	}
>> }
>> 
>> window.renderChart(chartData, this.container);
>> ```
>
>> |                     Verwendungen                     | Zauber                         |             +              |              -               |
>> |:----------------------------------------------------:|:------------------------------ |:--------------------------:|:----------------------------:|
>> |        `VIEW[{ZauberStatistik.Donnerschlag}]`        | [[Donnerschlag]]               | `BUTTON[donnerschlag_up]`  | `BUTTON[donnerschlag_down]`  |
>> |        `VIEW[{ZauberStatistik.Kältestrahl}]`         | [[Kältestrahl]]                |  `BUTTON[kältestrahl_up]`  |  `BUTTON[kältestrahl_down]`  |
>> |        `VIEW[{ZauberStatistik.Klingenbann}]`         | [[Klingenbann]]                |  `BUTTON[klingenbann_up]`  |  `BUTTON[klingenbann_down]`  |
>> |        `VIEW[{ZauberStatistik.Schockgriff}]`         | [[Schockgriff]]                |  `BUTTON[schockgriff_up]`  |  `BUTTON[schockgriff_down]`  |
>> |           `VIEW[{ZauberStatistik.Windbö}]`           | [[Windbö]]                     |    `BUTTON[windbö_up]`     |    `BUTTON[windbö_down]`     |
>> |         `VIEW[{ZauberStatistik.Chaospfeil}]`         | [[Chaospfeil]]                 |  `BUTTON[chaospfeil_up]`   |  `BUTTON[chaospfeil_down]`   |
>> |         `VIEW[{ZauberStatistik.Hexenpfeil}]`         | [[Hexenpfeil]]                 |  `BUTTON[hexenpfeil_up]`   |  `BUTTON[hexenpfeil_down]`   |
>> |       `VIEW[{ZauberStatistik.Magierrüstung}]`        | [[Magierrüstung]]              | `BUTTON[magierrüstung_up]` | `BUTTON[magierrüstung_down]` |
>> |         `VIEW[{ZauberStatistik.Schutzwind}]`         | [[Schutzwind]]                 |  `BUTTON[schutzwind_up]`   |  `BUTTON[schutzwind_down]`   |
>> | `VIEW[{ZauberStatistik.Snillocs_Schneeballschwarm}]` | [[Snillocs Schneeballschwarm]] |   `BUTTON[snillocs_up]`    |   `BUTTON[snillocs_down]`    | 
>> 

## Vergangenheit

- kommt in Niewinter an um dort seine Suche nach den Splittern des [[Tempestus Kristall|Tempestus Kristalls]] zu starten
- die Anhänger des bösen Sturmgottes [[Talos]] sind ebenfalls hinter den Splittern und dem [[Tempestus Kristall]] her
- hört Gerüchte über einen Kristall auf den die Beschreibung eines Splitters des [[Tempestus Kristall|Tempestus Kristalls]] passt und der bei einem örtlichen Händler aufgetaucht ist
- forscht nach und findet heraus, dass der Kristall vor einigen Tagen aus der Stadt geschmuggelt worden sein soll
- da er neu in der Gegend ist und niemanden kennt schließt er sich der [[Abenteurergilde]] an
- schließt sich einer dubiosen Gruppe an, die auf dem Weg nach [[Phandalin]] ist um den geheimnisvollen Geschehnissen dort auf den Grund zu gehen...
- Gruppe ließ ihn in [[Phandalin]] zurück als sie vom [[Tempestus Kristall]] gehört hatten
- seitdem wartet er immer noch auf die Gruppe..

## Hintergrundgeschichte

**Ar'gonthariel Maez'ralor Sturmzorn** wurde nicht in einer Gemeinschaft von Drachengeborenen geboren, sondern in einer isolierten Inselkolonie, die von einem uralten, fast vergessenen Drachenkult bewohnt wurde. Der Kult verehrte den Sturm als göttliche Manifestation und sah es als seine heilige Pflicht an, das Gleichgewicht der Natur durch rituelle Praktiken und magische Rituale zu wahren. Die Mitglieder dieses Kultes waren hauptsächlich Menschen und Halbelfen, und Ar'gonthariel Maez'ralor war der einzige Drachengeborene unter ihnen.

Seine Eltern, Mitglieder des Kultes, hatten ihn als besonderes Geschenk des Sturmgottes betrachtet, ein lebendiges Bindeglied zwischen den Drachen und den Sterblichen. Ar'gonthariel Maez'ralor wuchs in einer Umgebung auf, die von tiefem mystischen Wissen und strengen, archaischen Traditionen geprägt war. Er lernte die alte Magie der Sturmrituale und verbrachte viele Stunden damit, das Verhalten der Winde und das Flüstern des Donners zu studieren.

Während eines besonders mächtigen Sturms, bei dem die Insel beinahe zerstört wurde, erschien Ar'gonthariel Maez'ralor in einer Vision der uralte Sturmdrache, den der Kult verehrte. Der Drache offenbarte ihm, dass das Gleichgewicht der Welt in Gefahr war und dass es Ar'gonthariel Maez'ralor's Schicksal sei, hinaus in die Welt zu gehen und die Fragmente eines uralten Artefakts zu sammeln, das die Macht besaß, die Elemente zu harmonisieren.

Dieses Artefakt, der **Tempestus-Kristall**, war vor Jahrhunderten in vier Teile zerbrochen und über die Verlorenen Reiche verstreut worden. Jedes Fragment beherbergte die Essenz eines Aspekts der Sturmkraft:

1. **Fragment des Windes**: Ein Teil, der die Kontrolle über die Luftströme und Winde verleiht.
2. **Fragment des Blitzes**: Ein Teil, der die Macht des Blitzes und der Elektrizität kanalisiert.
3. **Fragment des Donners**: Ein Teil, der die Gewalt des Donners und Schalls entfesselt.
4. **Fragment des Regens**: Ein Teil, der die Kräfte des Wassers und des Regens birgt.

Der Kult hatte über die Jahre von der Existenz des Kristalls gewusst, aber nur Ar'gonthariel Maez'ralor besaß die einzigartige Fähigkeit, seine Fragmente zu erspüren und zu vereinen.

Von dieser Vision tief bewegt, verließ Ar'gonthariel Maez'ralor die Insel und machte sich auf den Weg, die Fragmente des Tempestus-Kristalls zu finden. Seine Abenteuer führten ihn durch uralte Wälder, über weite Wüsten und in die tiefsten Tiefen vergessener Ruinen. Jedes Fragment, das er fand, stärkte seine Verbindung zur Sturmmagie und enthüllte neue Geheimnisse der Elementarkräfte.

Ar'gonthariel Maez'ralor's Motivation ist nicht Ruhm oder Reichtum, sondern die tiefe Überzeugung, dass das Schicksal der Welt und das Gleichgewicht der Natur auf dem Spiel stehen. Er ist getrieben von der Verantwortung, die ihm vom Sturmdrachen übertragen wurde, und der tiefen Liebe zu der Welt, die er schützen muss. Sein Weg ist gefährlich und voller Herausforderungen, aber Ar'gonthariel Maez'ralor weiß, dass er der einzige ist, der diese Aufgabe erfüllen kann.

## Versteckte Logiken & Button Konfigurationen

```meta-bind-button
label: Kurze Rast
icon: switch
hidden: true
class: ""
tooltip: ""
id: shortBreakButton
style: primary
actions:
  - type: updateMetadata
    bindTarget: InputData.BlitzOdem
    evaluate: false
    value: "false"
```

```meta-bind-button
label: Lange Rast
icon: reset
hidden: true
class: ""
tooltip: ""
id: longBreakButton
style: primary
actions:
  - type: updateMetadata
    bindTarget: Gesundheit.TW
    evaluate: false
    value: "4"
  - type: updateMetadata
    bindTarget: InputData.Uhrzeit1
    evaluate: false
    value: 00:00
  - type: updateMetadata
    bindTarget: InputData.Uhrzeit2
    evaluate: false
    value: 00:00
  - type: updateMetadata
    bindTarget: InputData.UhrzeitToogle1
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.UhrzeitToogle2
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.Zauberpunkte
    evaluate: false
    value: "17"
  - type: updateMetadata
    bindTarget: InputData.Zauberplätze.Grad_1
    evaluate: false
    value: "4"
  - type: updateMetadata
    bindTarget: InputData.Zauberplätze.Grad_2
    evaluate: false
    value: "3"
  - type: updateMetadata
    bindTarget: InputData.Zauberplätze.Grad_3
    evaluate: false
    value: "0"
  - type: updateMetadata
    bindTarget: InputData.Zauberplätze.Grad_4
    evaluate: false
    value: "0"
  - type: updateMetadata
    bindTarget: InputData.Zauberplätze.Grad_5
    evaluate: false
    value: "0"
  - type: updateMetadata
    bindTarget: InputData.Zauberplätze.Grad_6
    evaluate: false
    value: "0"
  - type: updateMetadata
    bindTarget: InputData.Zauberplätze.Grad_7
    evaluate: false
    value: "0"
  - type: updateMetadata
    bindTarget: InputData.Zauberplätze.Grad_8
    evaluate: false
    value: "0"
  - type: updateMetadata
    bindTarget: InputData.Zauberplätze.Grad_9
    evaluate: false
    value: "0"
  - type: updateMetadata
    bindTarget: InputData.NormaleRüstung
    evaluate: false
    value: "true"
  - type: updateMetadata
    bindTarget: InputData.MagierRüstung
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.BlitzOdem
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.ErschöpfungsPunkte
    evaluate: true
    value: x - 1
```


```meta-bind-button
 icon: up-arrow-with-tail
 label: ""
 hidden: true
 class: ""
 tooltip: ""
 id: "donnerschlag_up"
 style: primary
 actions:
   - type: updateMetadata
     bindTarget: ZauberStatistik.Donnerschlag
     evaluate: true
     value: x + 1
```

 ```meta-bind-button
 icon: down-arrow-with-tail
 label: ""
 hidden: true
 class: ""
 tooltip: ""
 id: "donnerschlag_down"
 style: primary
 actions:
   - type: updateMetadata
     bindTarget: ZauberStatistik.Donnerschlag
     evaluate: true
     value: x - 1
 
 ```

```meta-bind-button
 label: ""
 icon: up-arrow-with-tail
 hidden: true
 class: ""
 tooltip: ""
 id: "kältestrahl_up"
 style: primary
 actions:
    - type: updateMetadata
      bindTarget: ZauberStatistik.Kältestrahl
      evaluate: true
      value: x + 1
 
```

 ```meta-bind-button
 label: ""
 icon: down-arrow-with-tail
 hidden: true
 class: ""
 tooltip: ""
 id: "kältestrahl_down"
 style: primary
 actions:
   - type: updateMetadata
     bindTarget: ZauberStatistik.Kältestrahl
     evaluate: true
     value: x - 1
 
 ```

 ```meta-bind-button
 label: ""
 icon: up-arrow-with-tail
 hidden: true
 class: ""
 tooltip: ""
 id: "klingenbann_up"
 style: primary
 actions:
    - type: updateMetadata
      bindTarget: ZauberStatistik.Klingenbann
      evaluate: true
      value: x + 1
 
 ```

 ```meta-bind-button
 label: ""
 icon: down-arrow-with-tail
 hidden: true
 class: ""
 tooltip: ""
 id: "klingenbann_down"
 style: primary
 actions:
   - type: updateMetadata
     bindTarget: ZauberStatistik.Klingenbann
     evaluate: true
     value: x - 1
 
 ```

 ```meta-bind-button
 label: ""
 icon: up-arrow-with-tail
 hidden: true
 class: ""
 tooltip: ""
 id: "schockgriff_up"
 style: primary
 actions:
    - type: updateMetadata
      bindTarget: ZauberStatistik.Schockgriff
      evaluate: true
      value: x + 1
 
 ```
 
```meta-bind-button
label: ""
icon: down-arrow-with-tail
hidden: true
class: ""
tooltip: ""
id: "schockgriff_down"
style: primary
actions:
  - type: updateMetadata
    bindTarget: ZauberStatistik.Schockgriff
    evaluate: true
    value: x - 1

```

```meta-bind-button
 label: ""
 icon: up-arrow-with-tail
 hidden: true
 class: ""
 tooltip: ""
 id: "windbö_up"
 style: primary
 actions:
   - type: updateMetadata
     bindTarget: ZauberStatistik.Windbö
     evaluate: true
     value: x + 1

```

```meta-bind-button
label: ""
icon: down-arrow-with-tail
hidden: true
class: ""
tooltip: ""
id: "windbö_down"
style: primary
actions:
  - type: updateMetadata
    bindTarget: ZauberStatistik.Windbö
    evaluate: true
    value: x - 1

```

```meta-bind-button
 label: ""
 icon: up-arrow-with-tail
 hidden: true
 class: ""
 tooltip: ""
 id: "chaospfeil_up"
 style: primary
 actions:
   - type: updateMetadata
     bindTarget: ZauberStatistik.Chaospfeil
     evaluate: true
     value: x + 1

```

```meta-bind-button
label: ""
icon: down-arrow-with-tail
hidden: true
class: ""
tooltip: ""
id: "chaospfeil_down"
style: primary
actions:
  - type: updateMetadata
    bindTarget: ZauberStatistik.Chaospfeil
    evaluate: true
    value: x - 1

```

```meta-bind-button
 label: ""
 icon: up-arrow-with-tail
 hidden: true
 class: ""
 tooltip: ""
 id: "hexenpfeil_up"
 style: primary
 actions:
   - type: updateMetadata
     bindTarget: ZauberStatistik.Hexenpfeil
     evaluate: true
     value: x + 1

```

```meta-bind-button
label: ""
icon: down-arrow-with-tail
hidden: true
class: ""
tooltip: ""
id: "hexenpfeil_down"
style: primary
actions:
  - type: updateMetadata
    bindTarget: ZauberStatistik.Hexenpfeil
    evaluate: true
    value: x - 1

```

```meta-bind-button
 label: ""
 icon: up-arrow-with-tail
 hidden: true
 class: ""
 tooltip: ""
 id: "magierrüstung_up"
 style: primary
 actions:
   - type: updateMetadata
     bindTarget: ZauberStatistik.Magierrüstung
     evaluate: true
     value: x + 1

```

```meta-bind-button
label: ""
icon: down-arrow-with-tail
hidden: true
class: ""
tooltip: ""
id: "magierrüstung_down"
style: primary
actions:
  - type: updateMetadata
    bindTarget: ZauberStatistik.Magierrüstung
    evaluate: true
    value: x - 1

```

```meta-bind-button
 label: ""
 icon: up-arrow-with-tail
 hidden: true
 class: ""
 tooltip: ""
 id: "schutzwind_up"
 style: primary
 actions:
   - type: updateMetadata
     bindTarget: ZauberStatistik.Schutzwind
     evaluate: true
     value: x + 1

```

```meta-bind-button
label: ""
icon: down-arrow-with-tail
hidden: true
class: ""
tooltip: ""
id: "schutzwind_down"
style: primary
actions:
  - type: updateMetadata
    bindTarget: ZauberStatistik.Schutzwind
    evaluate: true
    value: x - 1

```

```meta-bind-button
 label: ""
 icon: up-arrow-with-tail
 hidden: true
 class: ""
 tooltip: ""
 id: "snillocs_up"
 style: primary
 actions:
   - type: updateMetadata
     bindTarget: ZauberStatistik.Snillocs_Schneeballschwarm
     evaluate: true
     value: x + 1
```

```meta-bind-button
label: ""
icon: down-arrow-with-tail
hidden: true
class: ""
tooltip: ""
id: "snillocs_down"
style: primary
actions:
  - type: updateMetadata
    bindTarget: ZauberStatistik.Snillocs_Schneeballschwarm
    evaluate: true
    value: x - 1
```
 
 ```js-engine
// Grab the Meta Bind API and extract metadata fields
const mb = engine.getPlugin('obsidian-meta-bind-plugin').api;

const ErschöpfungsPunkte = mb.parseBindTarget('InputData.ErschöpfungsPunkte', context.file.path);
const reactiveErschöpfungsPunkte = engine.reactive(onErschöpfungsPunkteChange, mb.getMetadata(ErschöpfungsPunkte)); 
setTimeout(() => {
	mb.subscribeToMetadata(ErschöpfungsPunkte, component, (value) => { reactiveErschöpfungsPunkte.refresh(value); }); 
}, 50);

const Erschöpfung1 = mb.parseBindTarget('InputData.Erschöpfung1', context.file.path);
const reactiveErschöpfung1 = engine.reactive(onChange1, mb.getMetadata(Erschöpfung1)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung1, component, (value) => { reactiveErschöpfung1.refresh(value); }); 
}, 50);

const Erschöpfung2 = mb.parseBindTarget('InputData.Erschöpfung2', context.file.path);
const reactiveErschöpfung2 = engine.reactive(onChange2, mb.getMetadata(Erschöpfung2)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung2, component, (value) => { reactiveErschöpfung2.refresh(value); }); 
}, 50);

const Erschöpfung3 = mb.parseBindTarget('InputData.Erschöpfung3', context.file.path);
const reactiveErschöpfung3 = engine.reactive(onChange3, mb.getMetadata(Erschöpfung3)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung3, component, (value) => { reactiveErschöpfung3.refresh(value); }); 
}, 50);

const Erschöpfung4 = mb.parseBindTarget('InputData.Erschöpfung4', context.file.path);
const reactiveErschöpfung4 = engine.reactive(onChange4, mb.getMetadata(Erschöpfung4)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung4, component, (value) => { reactiveErschöpfung4.refresh(value); }); 
}, 50);

const Erschöpfung5 = mb.parseBindTarget('InputData.Erschöpfung5', context.file.path);
const reactiveErschöpfung5 = engine.reactive(onChange5, mb.getMetadata(Erschöpfung5)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung5, component, (value) => { reactiveErschöpfung5.refresh(value); }); 
}, 50);

const Erschöpfung6 = mb.parseBindTarget('InputData.Erschöpfung6', context.file.path);
const reactiveErschöpfung6 = engine.reactive(onChange6, mb.getMetadata(Erschöpfung6)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung6, component, (value) => { reactiveErschöpfung6.refresh(value); }); 
}, 50);

const Erschöpfung7 = mb.parseBindTarget('InputData.Erschöpfung7', context.file.path);
const reactiveErschöpfung7 = engine.reactive(onChange7, mb.getMetadata(Erschöpfung7)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung7, component, (value) => { reactiveErschöpfung7.refresh(value); }); 
}, 50);

const Erschöpfung8 = mb.parseBindTarget('InputData.Erschöpfung8', context.file.path);
const reactiveErschöpfung8 = engine.reactive(onChange8, mb.getMetadata(Erschöpfung8)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung8, component, (value) => { reactiveErschöpfung8.refresh(value); }); 
}, 50);

const Erschöpfung9 = mb.parseBindTarget('InputData.Erschöpfung9', context.file.path);
const reactiveErschöpfung9 = engine.reactive(onChange9, mb.getMetadata(Erschöpfung9)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung9, component, (value) => { reactiveErschöpfung9.refresh(value); }); 
}, 50);

//events
function onErschöpfungsPunkteChange(value) {

	if( value < 0 ) {
		mb.setMetadata(ErschöpfungsPunkte, 0);
		return;
	}

	const metadataBind = {
		'Erschöpfung1': Erschöpfung1,
		'Erschöpfung2': Erschöpfung2,
		'Erschöpfung3': Erschöpfung3,
		'Erschöpfung4': Erschöpfung4,
		'Erschöpfung5': Erschöpfung5,
		'Erschöpfung6': Erschöpfung6,
		'Erschöpfung7': Erschöpfung7,
		'Erschöpfung8': Erschöpfung8,
		'Erschöpfung9': Erschöpfung9
	}

    const oldStates = [
        mb.getMetadata(Erschöpfung1),
        mb.getMetadata(Erschöpfung2),
        mb.getMetadata(Erschöpfung3),
        mb.getMetadata(Erschöpfung4),
        mb.getMetadata(Erschöpfung5),
        mb.getMetadata(Erschöpfung6),
        mb.getMetadata(Erschöpfung7),
        mb.getMetadata(Erschöpfung8),
        mb.getMetadata(Erschöpfung9)
    ];

    const newStates = Array(9).fill(false).map((_, index) => index < value);

    newStates.forEach((newState, index) => {
        if (oldStates[index] !== newState) {
            mb.setMetadata(metadataBind[`Erschöpfung${index + 1}`], newState);
        }
    });
}


function onChange1(value){
	onErschöpfungChange(1, value, Erschöpfung1);
}

function onChange2(value){
	onErschöpfungChange(2, value, Erschöpfung2);
}

function onChange3(value){
	onErschöpfungChange(3, value, Erschöpfung3);
}

function onChange4(value){
	onErschöpfungChange(4, value, Erschöpfung4);
}

function onChange5(value){
	onErschöpfungChange(5, value, Erschöpfung5);
}

function onChange6(value){
	onErschöpfungChange(6, value, Erschöpfung6);
}

function onChange7(value){
	onErschöpfungChange(7, value, Erschöpfung7);
}

function onChange8(value){
	onErschöpfungChange(8, value, Erschöpfung8);
}

function onChange9(value){
	onErschöpfungChange(9, value, Erschöpfung9);
}

function onErschöpfungChange(ErschöpfungsValue, newValue, metadataBind){	
	const currentPoints = mb.getMetadata(ErschöpfungsPunkte);
	const lowerValue = parseInt(ErschöpfungsValue-1);

	if(currentPoints == lowerValue && !newValue){
		return;
	} else if (currentPoints == lowerValue && newValue) {
		mb.setMetadata(ErschöpfungsPunkte, ErschöpfungsValue);
	} else if (currentPoints == ErschöpfungsValue && !newValue) {
		mb.setMetadata(ErschöpfungsPunkte, lowerValue);
	} else if (currentPoints > ErschöpfungsValue) {
		if(newValue == false) mb.setMetadata(metadataBind, true);
	} else if (currentPoints < ErschöpfungsValue) {
		if(newValue == true) mb.setMetadata(metadataBind, false);
	}
}

```
