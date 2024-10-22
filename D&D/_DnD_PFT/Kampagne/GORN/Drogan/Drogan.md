---
Stufe: 5
Bewegung: 7
Verteidigung:
  Natürliche_Rüstung: 10
  Zusätzliche_Rüstung: 0
  Rüstung:
  Schild:
Waffen:
  - "[[Zweihandaxt]]"
  - "[[Axt]]"
  - "[[Wurfspeer]]"
  - "[[Leichte Armbrust]]"
  - "[[Streitaxt]]"
Gesundheit:
  MaxTP: 59
  TP: 59
  TW: 5
  TempTP: 0
Attribute:
  Stärke: 18
  Geschicklichkeit: 14
  Konstitution: 16
  Intelligenz: 10
  Weisheit: 12
  Charisma: 8
Rettungswürfe:
  Stärke: 1
  Geschicklichkeit: 0
  Konstitution: 1
  Intelligenz: 0
  Weisheit: 0
  Charisma: 0
Fertigkeiten:
  Akrobatik: 0
  Arkane_Kunde: 0
  Athletik: 1
  Auftreten: 0
  Einschüchtern: 1
  Fingerfertigkeit: 0
  Geschichte: 0
  Heilkunde: 0
  Heimlichkeit: 0
  Mit_Tieren_umgehen: 0
  Motiv_erkennen: 0
  Nachforschungen: 1
  Naturkunde: 0
  Religion: 0
  Täuschen: 0
  Überlebenskunst: 0
  Überzeugen: 0
  Wahrnehmung: 1
Übung:
  Sprachen:
    - "[[Gemeinsprache]]"
    - "[[Zwergisch]]"
    - "[[Riesisch]]"
    - "[[Abyssisch]]"
  Werkzeuge:
    - "[[Brauereivorräte]]"
  Rüstungen:
    - "[[Leichte Rüstung]]"
    - "[[Mittelschwere Rüstung]]"
    - "[[Schilde]]"
  Waffen:
    - "[[Einfache Waffen]]"
    - "[[Kriegswaffen]]"
Aussehen:
  Geschlecht: männlich
  Alter: 115 Jahre
  Größenkategorie: "[[Mittelgroß]]"
  Größe: 140 cm
  Gewicht: 150 Pfund
  Augenfarbe: Blau
  Haarfarbe: Orange
  Hautfarbe: Sandfarben
Merkmale:
  Volk:
    - "[[Dunkelsicht]]"
    - "[[Unempfindlichkeit]]"
    - "[[Handwerkliches Geschick]]"
    - "[[Steingespür]]"
    - "[[Zwergisches Kampftraining]]"
    - "[[Zwergische Rüstungsvertrautheit]]"
  Klasse:
    - "[[Kampfrausch]]"
    - "[[Ungerüstete Verteidigung]]"
    - "[[Rücksichtsloser Angriff]]"
    - "[[Gefahrengespür]]"
    - "[[Titanengriff]]"
    - "[[Furchtlos]]"
    - "[[Schnelle Bewegung]]"
    - "[[Zusätzlicher Angriff]]"
  Talente:
    - "[[Meisterschaft Kampf mit zwei Waffen]]"
Hintergrund:
  Volk: "[[Zwerge#Gerbirgszwerge|Gebirgszwerg]]"
  Klasse: "[[Barbar]]"
  Subklasse: "[[Pfad des Slayers]]"
  Gesinnung: "[[Neutral Gut]]"
  Hintergrund: "[[Heimgesuchter]]"
Persönlichkeit:
  Persönlichkeitsmerkmale:
    - Ich fliehe nicht vor dem Bösen, das Böse flieht vor mir.
    - Ich spreche nicht über das, was mich quält.
    - Ich möchte andere nicht mit meinem Fluch belasten.
  Ideale: Ich versuche denjenigen zu helfen die Hilfe benötigen, egal was es mich kosten mag.
  Bindungen: Eine furchtbare Schuld verzehrt mich. Ich hoffe durch meine Taten Erlösung zu finden.
  Makel: Ich habe eine (Alkohol-)Sucht.
InputData:
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
  Rage1: false
  Rage2: false
  Rage3: false
tags:
  - Charakter/GORN
---
# `=this.file.name`

> [!infobox]
>  ![[Drogan.jpeg]]
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
> | Größenkategorie | `=this.Aussehen.Größenkategorie` |
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

## Tracker
|                           | 
|:-------------------------:|
| `BUTTON[longBreakButton]` |

| Eigenschaft  |  1  |  2  |  3  |  4  |  5  |  6  |  7  |  8  |  9  |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| [[Glück\|Glückspunkte]]  | `INPUT[toggle:InputData.GlücksPunkt1]` |  `INPUT[toggle:InputData.GlücksPunkt2]` | `INPUT[toggle:InputData.GlücksPunkt3]` | `INPUT[toggle:InputData.GlücksPunkt4]` | `INPUT[toggle:InputData.GlücksPunkt5]` |  -  |  -  |  -  |  -  |
| [[Erschöpft\|Erschöpfung]]       |  `INPUT[toggle:InputData.Erschöpfung1]`  | `INPUT[toggle:InputData.Erschöpfung2]` |  `INPUT[toggle:InputData.Erschöpfung3]`  |  `INPUT[toggle:InputData.Erschöpfung4]`  | `INPUT[toggle:InputData.Erschöpfung5]`  |  `INPUT[toggle:InputData.Erschöpfung6]`  |  `INPUT[toggle:InputData.Erschöpfung7]`  |  `INPUT[toggle:InputData.Erschöpfung8]`  |  `INPUT[toggle:InputData.Erschöpfung9]`  |

### Klasse
| Nutzungen [[Kampfrausch]] (max. `$=dv.page(dv.current().Hintergrund.Klasse).Kampfrausch["Stufe"+dv.current().Stufe].Anzahl`)              | Bonuschaden [[Kampfrausch]]                                                                        |
| ----------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| `INPUT[toggle:InputData.Rage1]` `INPUT[toggle:InputData.Rage2]` `INPUT[toggle:InputData.Rage3]` | +`$=dv.page(dv.current().Hintergrund.Klasse).Kampfrausch["Stufe"+dv.current().Stufe].Bonusschaden` |

## Bewegung
| Gehen                                              | [[Spurt]]                                          | [[Hochsprung]] mit Anlauf                            | [[Hochsprung]] ohne Anlauf                             | [[Weitsprung]] mit Anlauf                 | [[Weitsprung]] ohne Anlauf                  |
| -------------------------------------------------- | -------------------------------------------------- | ---------------------------------------------------- | ------------------------------------------------------ | ----------------------------------------- | ------------------------------------------- |
| `=this.Bewegung*1.5` m (`=this.Bewegung` Kästchen) | `=this.Bewegung*3` m (`=this.Bewegung*2` Kästchen) | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)` m | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)/2` m | `=round((this.Attribute.Stärke*0.3),2)` m | `=round((this.Attribute.Stärke*0.3)/2,2)` m |

## Verteidigung
> [!column | no-title] 
>> ### Gesundheit
>> |         | [[Trefferpunkte]]        | [[Trefferwürfel]] (`=this.Hintergrund.Klasse.Trefferwürfel`)        | [[Temporäre Trefferpunkte]] |
>> | ------- | ------------------------ | ------------------------ | --------------------------- |
>> | Maximal | `=this.Gesundheit.MaxTP` | `=this.Stufe`  |                             |
>> | Aktuell | `INPUT[number():Gesundheit.TP]`    |`INPUT[number():Gesundheit.TW]` | `INPUT[number():Gesundheit.TempTP]`   |
>
>>### Rüstung
>>|                                                                   Rüstung                                                                    |                                                                                        [[Rüstungsklasse]]                                                                                         |                                                        [[Schadensreduktion]]                                                         |
>>|:--------------------------------------------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------:|
>>| `=this.Verteidigung.Rüstung` `=choice(this.Verteidigung.Schild, ", ", "")` `=choice(this.Verteidigung.Schild, this.Verteidigung.Schild, "")` | `=this.Verteidigung.Natürliche_Rüstung+floor(((this.Attribute.Geschicklichkeit)-10)/2)+choice(this.Verteidigung.Rüstung.RP, this.Verteidigung.Rüstung.RP, 0)+this.Verteidigung.Zusätzliche_Rüstung+floor(((this.Attribute.Konstitution)-10)/2)` + `=choice(this.Verteidigung.Schild, this.Verteidigung.Schild.RP, 0)` | `=choice(this.Verteidigung.Rüstung.SR, this.Verteidigung.Rüstung.SR, 0)` + `=choice(this.Schild.SR, this.Verteidigung.Schild.SR, 0)` |
>>
>>| Beschreibung | Bonus (bereits eingerechnet) |
>>| :---: |  :---: |
>>| Zusätzliche Rüstung | `INPUT[number:Verteidigung.Zusätzliche_Rüstung]` |

## Angriff
> [!column | no-title]
>> ### Nahkampfwaffen
>> ```dataview
>> TABLE WITHOUT ID 
>> file.link AS "Waffe",
>> Reichweite,
>> "`dice:1d20+" + (floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)+ceil(this.Stufe/4)+1) + choice(Angriffsbonus,("+" + Angriffsbonus),"") + "|none|noform`" AS "Angriff",
>> "`dice:" + Schaden + "+" + floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2) + "\|none\|noform`"  AS "Schaden",
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
>> "`dice:1d20+" + (floor(((this.Attribute.Geschicklichkeit)-10)/2)+ceil(this.Stufe/4)+1) + choice(AngriffsbonusFern,("+" + AngriffsbonusFern),"") +"|none|noform`" AS "Angriff",
>> "`dice:" + SchadenFern + "+" + floor(((this.Attribute.Geschicklichkeit)-10)/2) + "\|none\|noform`"  AS "Schaden",
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
>> "`dice:1d20+" + (floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)+ceil(this.Stufe/4)+1) + choice(AngriffsbonusFern,("+" + AngriffsbonusFern),"") + "|none|noform`" AS "Angriff",
>> "`dice:" + SchadenFern + "+" + floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2) + "\|none\|noform`"  AS "Schaden",
>> SchadensartFern AS "Schadensart",
>> EigenschaftenFern AS "Eigenschaften"
>> FROM #Gegenstand/Waffe/Klasse/Fernkampfwaffe/Wurfwaffe  
>> WHERE contains(this.Waffen, file.link)
>> SORT file.name
>> ```

Disclaimer: Waffen haben immer Übungsbonus...

## Attribute und Fertigkeiten
> [!column  | 6 no-title]
>> ## Stärke
>> |                                                                                                                  |                                                                                                                                                                    |
>> | -------------------------------------------------------------------------------------------------------------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
>> | [[Attribute\|Attributswert]]                                                                                               |                                                                            `=this.Attribute.Stärke`   (`=choice(floor(((this.Attribute.Stärke)-10)/2)>0, "+" + floor(((this.Attribute.Stärke)-10)/2), floor(((this.Attribute.Stärke)-10)/2))`)                                                                          |
>> | [[Attribute#Attributswurf]]                                                                                                |                                         `$="```dice:1d20+" + Math.floor(((dv.current().Attribute.Stärke)-10)/2) + "\|none\|noform\```"`                                         |
>> | [[Rettungswurf]] `=choice(this.Rettungswürfe.Stärke=2, "⭐⭐", choice(this.Rettungswürfe.Stärke=1, "⭐",""))`              |    `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Stärke)-10)/2)+(dv.current().Rettungswürfe.Stärke*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Athletik]] `=choice(this.Fertigkeiten.Athletik=2, "⭐⭐", choice(this.Fertigkeiten.Athletik=1, "⭐",""))`               |   `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Stärke)-10)/2)+(dv.current().Fertigkeiten.Athletik*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Einschüchtern]] `=choice(this.Fertigkeiten.Einschüchtern=2, "⭐⭐", choice(this.Fertigkeiten.Einschüchtern=1, "⭐",""))` | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Stärke)-10)/2)+(dv.current().Fertigkeiten.Einschüchtern*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>
>> ## Geschicklichkeit
>> |                   |                                                                                                                                                                    |
>> | --------------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
>> | [[Attribute\|Attributswert]]                |                                                                            `=this.Attribute.Geschicklichkeit`    (`=choice(floor(((this.Attribute.Geschicklichkeit)-10)/2)>0, "+" + floor(((this.Attribute.Geschicklichkeit)-10)/2), floor(((this.Attribute.Geschicklichkeit)-10)/2))`)                                                                            |
>> | [[Attribute#Attributswurf]]  |                                         `$="```dice:1d20+" + Math.floor(((dv.current().Attribute.Geschicklichkeit)-10)/2) + "\|none\|noform\```"`                                         |
>> | [[Rettungswurf]] `=choice(this.Rettungswürfe.Geschicklichkeit=2, "⭐⭐", choice(this.Rettungswürfe.Geschicklichkeit=1, "⭐",""))`          |    `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Geschicklichkeit)-10)/2)+(dv.current().Rettungswürfe.Geschicklichkeit*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Akrobatik]] `=choice(this.Fertigkeiten.Akrobatik=2, "⭐⭐", choice(this.Fertigkeiten.Akrobatik=1, "⭐",""))`               |   `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Geschicklichkeit)-10)/2)+(dv.current().Fertigkeiten.Akrobatik*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Fingerfertigkeit]] `=choice(this.Fertigkeiten.Fingerfertigkeit=2, "⭐⭐", choice(this.Fertigkeiten.Fingerfertigkeit=1, "⭐",""))`          | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Geschicklichkeit)-10)/2)+(dv.current().Fertigkeiten.Fingerfertigkeit*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>> | [[Heimlichkeit]] `=choice(this.Fertigkeiten.Heimlichkeit=2, "⭐⭐", choice(this.Fertigkeiten.Heimlichkeit=1, "⭐",""))`         | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Geschicklichkeit)-10)/2)+(dv.current().Fertigkeiten.Heimlichkeit*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>
>> ## Konstitution
>> |                   |                                                                                                                                                                    |
>> | --------------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
>> | [[Attribute\|Attributswert]]                |                                                                            `=this.Attribute.Konstitution`  (`=choice(floor(((this.Attribute.Konstitution)-10)/2)>0, "+" + floor(((this.Attribute.Konstitution)-10)/2), floor(((this.Attribute.Konstitution)-10)/2))`)                                                                            |
>> | [[Attribute#Attributswurf]] |                                         `$="```dice:1d20+" + Math.floor(((dv.current().Attribute.Konstitution)-10)/2) + "\|none\|noform\```"`                                         |
>> | [[Rettungswurf]] `=choice(this.Rettungswürfe.Konstitution=2, "⭐⭐", choice(this.Rettungswürfe.Konstitution=1, "⭐",""))`          |    `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Konstitution)-10)/2)+(dv.current().Rettungswürfe.Konstitution*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>
>> ## Intelligenz
>> |                   |                                                                                                                                                                    |
>> | --------------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
>> | [[Attribute\|Attributswert]]                |                                                                            `=this.Attribute.Intelligenz`   (`=choice(floor(((this.Attribute.Intelligenz)-10)/2)>0, "+" + floor(((this.Attribute.Intelligenz)-10)/2), floor(((this.Attribute.Intelligenz)-10)/2))`)                                                                             |
>> | [[Attribute#Attributswurf]] |                                         `$="```dice:1d20+" + Math.floor(((dv.current().Attribute.Intelligenz)-10)/2) + "\|none\|noform\```"`                                         |
>> | [[Rettungswurf]] `=choice(this.Rettungswürfe.Intelligenz=2, "⭐⭐", choice(this.Rettungswürfe.Intelligenz=1, "⭐",""))`          |    `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Intelligenz)-10)/2)+(dv.current().Rettungswürfe.Intelligenz*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Arkane Kunde]] `=choice(this.Fertigkeiten.Arkane_Kunde=2, "⭐⭐", choice(this.Fertigkeiten.Arkane_Kunde=1, "⭐",""))`               |   `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Intelligenz)-10)/2)+(dv.current().Fertigkeiten.Arkane_Kunde*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Geschichte]] `=choice(this.Fertigkeiten.Geschichte=2, "⭐⭐", choice(this.Fertigkeiten.Geschichte=1, "⭐",""))`         | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Intelligenz)-10)/2)+(dv.current().Fertigkeiten.Geschichte*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>> | [[Nachforschungen]] `=choice(this.Fertigkeiten.Nachforschungen=2, "⭐⭐", choice(this.Fertigkeiten.Nachforschungen=1, "⭐",""))`          | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Intelligenz)-10)/2)+(dv.current().Fertigkeiten.Nachforschungen*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>> | [[Naturkunde]] `=choice(this.Fertigkeiten.Naturkunde=2, "⭐⭐", choice(this.Fertigkeiten.Naturkunde=1, "⭐",""))`         | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Intelligenz)-10)/2)+(dv.current().Fertigkeiten.Naturkunde*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>> | [[Religion]] `=choice(this.Fertigkeiten.Religion=2, "⭐⭐", choice(this.Fertigkeiten.Religion=1, "⭐",""))`         | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Intelligenz)-10)/2)+(dv.current().Fertigkeiten.Religion*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>
>> ## Weisheit
>> |                   |                                                                                                                                                                    |
>> | --------------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
>> | [[Attribute\|Attributswert]]                |                                                                            `=this.Attribute.Weisheit`   (`=choice(floor(((this.Attribute.Weisheit)-10)/2)>0, "+" + floor(((this.Attribute.Weisheit)-10)/2), floor(((this.Attribute.Weisheit)-10)/2))`)                                                                             |
>> | [[Attribute#Attributswurf]] |                                         `$="```dice:1d20+" + Math.floor(((dv.current().Attribute.Weisheit)-10)/2) + "\|none\|noform\```"`                                         |
>> | [[Rettungswurf]] `=choice(this.Rettungswürfe.Weisheit=2, "⭐⭐", choice(this.Rettungswürfe.Weisheit=1, "⭐",""))`           |    `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Weisheit)-10)/2)+(dv.current().Rettungswürfe.Weisheit*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Heilkunde]] `=choice(this.Fertigkeiten.Heilkunde=2, "⭐⭐", choice(this.Fertigkeiten.Heilkunde=1, "⭐",""))`               |   `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Weisheit)-10)/2)+(dv.current().Fertigkeiten.Heilkunde*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Mit Tieren umgehen]] `=choice(this.Fertigkeiten.Mit_Tieren_umgehen=2, "⭐⭐", choice(this.Fertigkeiten.Mit_Tieren_umgehen=1, "⭐",""))`          | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Weisheit)-10)/2)+(dv.current().Fertigkeiten.Mit_Tieren_umgehen*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>> | [[Motiv erkennen]] `=choice(this.Fertigkeiten.Motiv_erkennen=2, "⭐⭐", choice(this.Fertigkeiten.Motiv_erkennen=1, "⭐",""))`               |   `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Weisheit)-10)/2)+(dv.current().Fertigkeiten.Motiv_erkennen*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Überlebenskunst]] `=choice(this.Fertigkeiten.Überlebenskunst=2, "⭐⭐", choice(this.Fertigkeiten.Überlebenskunst=1, "⭐",""))`              |   `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Weisheit)-10)/2)+(dv.current().Fertigkeiten.Überlebenskunst*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Wahrnehmung]] `=choice(this.Fertigkeiten.Wahrnehmung=2, "⭐⭐", choice(this.Fertigkeiten.Wahrnehmung=1, "⭐",""))`             |   `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Weisheit)-10)/2)+(dv.current().Fertigkeiten.Wahrnehmung*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> [[Wahrnehmung#Passive Wahrnehmung]]: `=10+floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Wahrnehmung*(ceil(this.Stufe/4)+1))`
>
>> ## Charisma
>> |                   |                                                                                                                                                                    |
>> | --------------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
>> | [[Attribute\|Attributswert]]                |                                                                            `=this.Attribute.Charisma`  (`=choice(floor(((this.Attribute.Charisma)-10)/2)>0, "+" + floor(((this.Attribute.Charisma)-10)/2), floor(((this.Attribute.Charisma)-10)/2))`)                                                                            |
>> | [[Attribute#Attributswurf]] |                                         `$="```dice:1d20+" + Math.floor(((dv.current().Attribute.Charisma)-10)/2) + "\|none\|noform\```"`                                         |
>> | [[Rettungswurf]] `=choice(this.Rettungswürfe.Charisma=2, "⭐⭐", choice(this.Rettungswürfe.Charisma=1, "⭐",""))`           |    `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Charisma)-10)/2)+(dv.current().Rettungswürfe.Charisma*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Auftreten]] `=choice(this.Fertigkeiten.Auftreten=2, "⭐⭐", choice(this.Fertigkeiten.Auftreten=1, "⭐",""))`             |   `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Charisma)-10)/2)+(dv.current().Fertigkeiten.Auftreten*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Einschüchtern]] `=choice(this.Fertigkeiten.Einschüchtern=2, "⭐⭐", choice(this.Fertigkeiten.Einschüchtern=1, "⭐",""))`        | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Charisma)-10)/2)+(dv.current().Fertigkeiten.Einschüchtern*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>> | [[Täuschen]] `=choice(this.Fertigkeiten.Täuschen=2, "⭐⭐", choice(this.Fertigkeiten.Täuschen=1, "⭐",""))`       | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Charisma)-10)/2)+(dv.current().Fertigkeiten.Täuschen*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>> | [[Überzeugen]] `=choice(this.Fertigkeiten.Überzeugen=2, "⭐⭐", choice(this.Fertigkeiten.Überzeugen=1, "⭐",""))`        | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Charisma)-10)/2)+(dv.current().Fertigkeiten.Überzeugen*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |

## Übung

> [!column | flex | no-title]
>> ## Rüstung
>> ```dataview
>> LIST
>> FROM #Gegenstand/Rüstung
>> WHERE contains(this.Übung.Rüstungen, file.link) 
>> SORT file.name
>> ```
> 
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
>
>> ## Werkzeuge
>> ```dataview
>> LIST
>> FROM #Gegenstand/Werkzeug
>> WHERE contains(this.Übung.Werkzeuge, file.link)
>> SORT file.name
>> ```

## Merkmale
> [!column | flex | no-title]
>> ## Volksmerkmale
>> ```dataview
>> LIST
>> FROM #Merkmal
>> WHERE contains(this.Merkmale.Volk, file.link)
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
>
>> ## Klassenmerkmale
>> ```dataview
>> LIST
>> FROM #Merkmal
>> WHERE contains(this.Merkmale.Klasse, file.link)
>> SORT file.name
>> ```

## Hintergrundgeschichte
TBD

## Versteckte Logiken & Button Konfigurationen

```meta-bind-button
label: Lange Rast
icon: reset
hidden: true
class: ""
tooltip: ""
id: longBreakButton
style: primary
actions:
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const tw = mb.parseBindTarget('Gesundheit.TW', context.file.path); const stufe = mb.getMetadata(mb.parseBindTarget('Stufe', context.file.path)); mb.setMetadata(tw, stufe);"
  - type: updateMetadata
    bindTarget: InputData.Rage1
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.Rage2
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.Rage3
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.ErschöpfungsPunkte
    evaluate: true
    value: x - 1
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const TP = mb.parseBindTarget('Gesundheit.TP', context.file.path); const maxTP = mb.getMetadata(mb.parseBindTarget('Gesundheit.MaxTP', context.file.path));  mb.setMetadata(TP, maxTP);"
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
