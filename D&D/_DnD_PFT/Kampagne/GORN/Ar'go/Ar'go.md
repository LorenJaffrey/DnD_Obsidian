---
Name: Ar'go
Stufe: 4
Bewegung: 6
Rüstung: 
Schild: 
Waffen:
  - "[[Kampfstab]]"
  - "[[Dolch]]"
Gesundheit:
  MaxTP: 23
  TP: 23
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
  Einschüchtern: 1
  Fingerfertigkeit: 0
  Geschichte: 0
  Heilkunde: 1
  Heimlichkeit: 0
  Mit_Tieren_umgehen: 0
  Motiv_erkennen: 0
  Nachforschungen: 0
  Naturkunde: 0
  Religion: 1
  Täuschen: 0
  Überlebenskunst: 0
  Überzeugen: 0
  Wahrnehmung: 0
Übung:
  Sprachen:
    - "[[Gemeinsprache]]"
    - "[[Urtümlich]]"
    - "[[Drakonisch]]"
    - "[[Celestisch]]"
  Werkzeuge:
    - "[[Kräuterkunde-Ausrüstung]]"
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
    - "[[Windsprecher]]"
    - "[[Stürmische Magie]]"
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
    - <ul><b>Unbarmherzigkeit</b></ul>Im Kampf um das Gleichgewicht der Natur kann Ar'gonthariel Maez'ralor unbarmherzig und kompromisslos sein, was ihm Feinde einbringen kann.
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
tags:
  - Charakter/GORN
---

> [!infobox]
> ![[Argo.jpeg]]
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
> [!column | 3 ]
>>  ## Allgemeine Spiel - Parameter
>> | Erholungs-Art | 1 | 2 |
>> | :---: | :---: | :---: |
>> | [[Kurze Rast]]| <input type="checkbox" unchecked id="0675a7">| <input type="checkbox" unchecked id="f34473"> |
>> | Uhrzeit            | `INPUT[time():KurzeRast.Uhrzeit1]` | `INPUT[time():KurzeRast.Uhrzeit2]` |
>>  
>> |  Eigenschaft  |  Wert  |  
>> | :---: | :---: | 
>> | [[Übung\|Übungsbonus]]  |   `=ceil(this.Stufe/4)+1`  |
>> | [[Initiative\|Initiativebonus]]  |  `=floor(((this.Attribute.Geschicklichkeit)-10)/2)`  | 
>> 
>> | Eigenschaft  |  1  |  2  |  3  |  4  |  5  |  6  |  7  |  8  |  9  |
>> | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
>> | [[Glück\|Glückspunkte]]  | <input type="checkbox" unchecked id="ecb03e"> |  <input type="checkbox" unchecked id="5d748c"> | <input type="checkbox" unchecked id="d25850"> | <input type="checkbox" unchecked id="5a568a"> | <input type="checkbox" unchecked id="7199c2"> |  -  |  -  |  -  |  -  |
>> | [[Erschöpft\|Erschöpfung]]       |  <input type="checkbox" unchecked id="73f4b5">  |  <input type="checkbox" unchecked id="0297f5"> |  <input type="checkbox" unchecked id="cd9aab">  |  <input type="checkbox" unchecked id="003cca">  | <input type="checkbox" unchecked id="949a4c">  |  <input type="checkbox" unchecked id="c1e92f">  |  <input type="checkbox" unchecked id="a2b7ed">  |  <input type="checkbox" unchecked id="89be6f">  |  <input type="checkbox" unchecked id="f1bb52">  |
>
>> ## Gesundheit
>> |         | [[Trefferpunkte]]        | [[Trefferwürfel]] (`=this.Hintergrund.Klasse.Trefferwürfel`)       | [[Temporäre Trefferpunkte]] |
>> | ------- | ------------------------ | ------------------------ | --------------------------- |
>> | Maximal | `=this.Gesundheit.MaxTP` | `=this.Stufe` |                             |
>> | Aktuell | `INPUT[number():Gesundheit.TP]`    |`INPUT[number():Gesundheit.TW]` | `INPUT[number():Gesundheit.TempTP]`   |
>>
>>>[!column | 2 ] 
>>>>## Rüstung
>>>> | Aktiv | Rüstung         | [[Rüstungsklasse]]                                                                                             | [[Schadensreduktion]]                                                                                         |
>>>> | --------------- | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
>>>> | <input type="checkbox" checked id="067501"> | `=this.Rüstung` `=choice(this.Schild, ", ", "")` `=choice(this.Schild, this.Schild, "")`  | `=10+floor(((this.Attribute.Geschicklichkeit)-10)/2)+choice(this.Rüstung.RP, this.Rüstung.RP, 0)` + `=choice(this.Schild, this.Schild.RP, 0)`  | `=choice(this.Rüstung.SR, this.Rüstung.SR, 0)` + `=choice(this.Schild.SR, this.Schild.SR, 0)` |
>>>> | <input type="checkbox" unchecked id="067500"> |  [[Magierrüstung]]  |  `=13+floor(((this.Attribute.Geschicklichkeit)-10)/2)`| |
>>>
>>>>## Resistenz
>>>> - Blitz
>
>> ## Bewegung
>> | Gehen                                              | [[Spurt]]                                          | 
>> | -------------------------------------------------- | -------------------------------------------------- |
>> | `=this.Bewegung*1.5` m (`=this.Bewegung` Kästchen) | `=this.Bewegung*3` m (`=this.Bewegung*2` Kästchen) | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)` m | 
>>
>> | [[Hochsprung]] mit Anlauf                            | [[Hochsprung]] ohne Anlauf                             |
>> | ---------------------------------------------------- | ------------------------------------------------------ |
>> | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)` m | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)/2` m |
>>
>> | [[Weitsprung]] mit Anlauf                 | [[Weitsprung]] ohne Anlauf                  |
>> | ----------------------------------------- | ------------------------------------------- |
>> | `=round((this.Attribute.Stärke*0.3),2)` m | `=round((this.Attribute.Stärke*0.3)/2,2)` m |

## Stats
> [!column ]
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
> [!column | 2]
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
>> 
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
>>| Blitz-Odem | <input type="checkbox" unchecked id="3db931">|
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
>> 
>> ## Grad 3
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
>> WHERE contains(this.Zauber, file.link) AND Grad=3
>> SORT file.name
>> ```
>

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