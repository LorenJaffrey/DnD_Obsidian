---
Stufe: 5
Niptac:
  Anzahl_Apparaturen: 2
  Energiekerngröße: W6
  Apparaturen:
    - "[[Gnomischer Flammenwerfer]]"
    - "[[Kobold Blitzwerfer]]"
Bewegung: 5
Verteidigung:
  Natürliche_Rüstung: 10
  Zusätzliche_Rüstung: 0
  Rüstung: "[[Beschlagene Lederrüstung]]"
  Schild: 
Waffen:
  - "[[Kurzschwert]]"
  - "[[Dolch]]"
  - "[[Axt]]"
  - "[[Schleuder]]"
  - "[[Leichte Armbrust]]"
Gesundheit:
  MaxTP: 42
  TP: 42
  TW: 5
  TempTP: 0
Attribute:
  Stärke: 8
  Geschicklichkeit: 17
  Konstitution: 14
  Intelligenz: 14
  Weisheit: 10
  Charisma: 14
Rettungswürfe:
  Stärke: 0
  Geschicklichkeit: 1
  Konstitution: 0
  Intelligenz: 1
  Weisheit: 0
  Charisma: 0
Fertigkeiten:
  Akrobatik: 0
  Arkane_Kunde: 0
  Athletik: 0
  Auftreten: 0
  Einschüchtern: 0
  Fingerfertigkeit: 2
  Geschichte: 0
  Heilkunde: 0
  Heimlichkeit: 1
  Mit_Tieren_umgehen: 0
  Motiv_erkennen: 0
  Nachforschungen: 0
  Naturkunde: 0
  Religion: 0
  Täuschen: 2
  Überlebenskunst: 0
  Überzeugen: 1
  Wahrnehmung: 1
Übung:
  Sprachen:
    - "[[Gemeinsprache]]"
    - "[[Gnomisch]]"
    - "[[Diebessprache]]"
  Werkzeuge:
    - "[[Diebeswerkzeug]]"
    - "[[Tüftlerwerkzeug]]"
    - "[[Fälscherausrüstung]]"
  Rüstungen:
    - "[[Leichte Rüstung]]"
  Waffen:
    - "[[Einfache Waffen]]"
    - "[[Handarmbrüste]]"
    - "[[Kurzschwert]]"
    - "[[Langschwert]]"
    - "[[Rapier]]"
Aussehen:
  Geschlecht: männlich
  Alter: 99 Jahre
  Größenkategorie: "[[Klein]]"
  Größe: 102 cm
  Gewicht: 49 Pfund
  Augenfarbe: Braun
  Haarfarbe: Schwarz
  Hautfarbe: Ocker
Merkmale:
  Volk:
    - "[[Dunkelsicht]]"
    - "[[Gnomische Gerissenheit]]"
    - "[[Artefaktkunde]]"
    - "[[Tüftler]]"
  Klasse:
    - "[[Hinterhältiger Angriff]]"
    - "[[Durchdachte Vorbereitung]]"
    - "[[Raffinierte Aktion]]"
    - "[[Zielsicher]]"
    - "[[Unglaubliches Ausweichen]]"
  Talente:
    - "[[Verschwinden]]"
Hintergrund:
  Volk: "[[Gnome|Gnom]]"
  Klasse: "[[Schurke]]"
  Subklasse: "[[Meistertüftler]]"
  Gesinnung: "[[Neutral Gut]]"
  Hintergrund: "[[Scharlatan]]"
Persönlichkeit:
  Persönlichkeitsmerkmale:
    - Ich kenne einen Witz für jede Situation, besonders für die, in denen Humor unangebracht ist.
  Ideale: Unabhängigkeit. Ich bin ein Freigeist, niemand kann mir vorschreiben, was ich zu tun oder zu lassen habe.
  Bindungen: Eine mächtige Person hat jemanden, den ich liebte, getötet. Der Tag meiner Rache wird kommen.
  Makel: Ich kann es nicht lassen, diejenigen zu beleidigen, die mächtiger sind als ich.
InputData:
  GlücksPunkt1: true
  GlücksPunkt2: true
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
  Energiekern1: true
  Energiekern2: true
  Energiekern3: true
  Energiekern4: true
  Fähigkeiten:
    Verschwinden: false
tags:
  - Charakter/GORN
---
# `=this.file.name`
> [!infobox]
> ![[Niptac.jpeg]]
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
> ### Persönlichkeitsmerkmale 
> `=this.Persönlichkeit.Persönlichkeitsmerkmale[0]`
> ### Ideale
> `=this.Persönlichkeit.Ideale`
> ### Bindungen
> `=this.Persönlichkeit.Bindungen`
> ### Makel
> `=this.Persönlichkeit.Makel`


## Rasten
|                           | 
|:-------------------------:|
| `BUTTON[longBreakButton]` |

[[Übung|Übungsbonus]]:  `=ceil(this.Stufe/4)+1`
[[Initiative|Initiativebonus]]: `=floor(((this.Attribute.Geschicklichkeit)-10)/2)`

| Eigenschaft  |  1  |  2  |  3  |  4  |  5  |  6  |  7  |  8  |  9  |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| [[Glück\|Glückspunkte]]  | `INPUT[toggle:InputData.GlücksPunkt1]` |  `INPUT[toggle:InputData.GlücksPunkt2]` | `INPUT[toggle:InputData.GlücksPunkt3]` | `INPUT[toggle:InputData.GlücksPunkt4]` | `INPUT[toggle:InputData.GlücksPunkt5]` |  -  |  -  |  -  |  -  |
| [[Erschöpft\|Erschöpfung]]       |  `INPUT[toggle:InputData.Erschöpfung1]`  | `INPUT[toggle:InputData.Erschöpfung2]` |  `INPUT[toggle:InputData.Erschöpfung3]`  |  `INPUT[toggle:InputData.Erschöpfung4]`  | `INPUT[toggle:InputData.Erschöpfung5]`  |  `INPUT[toggle:InputData.Erschöpfung6]`  |  `INPUT[toggle:InputData.Erschöpfung7]`  |  `INPUT[toggle:InputData.Erschöpfung8]`  |  `INPUT[toggle:InputData.Erschöpfung9]`  |

## Aufladungen 
| [[Durchdachte Vorbereitung#Engergiekerne]] | Anzahl [[Durchdachte Vorbereitung#Engergiekerne]]                                                                                                           |           [[Verschwinden#Verschwinden]]            |
|:------------------------------------------:| ----------------------------------------------------------------------------------------------------------------------------------------------------------- |:--------------------------------------------------:|
|      `=this.Niptac.Energiekerngröße`       | `INPUT[toggle:InputData.Energiekern1]` `INPUT[toggle:InputData.Energiekern2]` `INPUT[toggle:InputData.Energiekern3]` `INPUT[toggle:InputData.Energiekern4]` | `INPUT[toggle:InputData.Fähigkeiten.Verschwinden]` |

### Apparaturen (max `=this.Niptac.Anzahl_Apparaturen`)
```dataview
TABLE WITHOUT ID
file.link AS "Apparaturen", 
SG AS "Schwierigkeitsgrad"
FROM #Merkmal/Klasse/Schurke/Meistertüftler/Apparatur 
WHERE contains(this.Niptac.Apparaturen, file.link)
SORT SG, file.link
```

## Bewegung
| Gehen                                              | [[Spurt]]                                          | [[Hochsprung]] mit Anlauf                            | [[Hochsprung]] ohne Anlauf                             | [[Weitsprung]] mit Anlauf                 | [[Weitsprung]] ohne Anlauf                  |
| -------------------------------------------------- | -------------------------------------------------- | ---------------------------------------------------- | ------------------------------------------------------ | ----------------------------------------- | ------------------------------------------- |
| `=this.Bewegung*1.5` m (`=this.Bewegung` Kästchen) | `=this.Bewegung*3` m (`=this.Bewegung*2` Kästchen) | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)` m | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)/2` m | `=round((this.Attribute.Stärke*0.3),2)` m | `=round((this.Attribute.Stärke*0.3)/2,2)` m |

## Verteidigung

### Gesundheit
|             | [[Trefferpunkte]]               | [[Trefferwürfel]] (`=this.Hintergrund.Klasse.Trefferwürfel`) | [[Temporäre Trefferpunkte]]         |
| ----------- | ------------------------------- | ------------------------------------------------------------ | ----------------------------------- |
| **Aktuell** | `INPUT[number():Gesundheit.TP]` | `INPUT[number():Gesundheit.TW]`                              | `INPUT[number():Gesundheit.TempTP]` |
| Maximal     | `=this.Gesundheit.MaxTP`        | `=this.Stufe`                                                |                                     |


### Rüstung
|                                                                   Rüstung                                                                    |                                                                                        [[Rüstungsklasse]]                                                                                         |                                                        [[Schadensreduktion]]                                                         |
|:--------------------------------------------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------:|
| `=this.Verteidigung.Rüstung` `=choice(this.Verteidigung.Schild, ", ", "")` `=choice(this.Verteidigung.Schild, this.Verteidigung.Schild, "")` | `=this.Verteidigung.Natürliche_Rüstung+floor(((this.Attribute.Geschicklichkeit)-10)/2)+choice(this.Verteidigung.Rüstung.RP, this.Verteidigung.Rüstung.RP, 0)+this.Verteidigung.Zusätzliche_Rüstung` + `=choice(this.Verteidigung.Schild, this.Verteidigung.Schild.RP, 0)` | `=choice(this.Verteidigung.Rüstung.SR, this.Verteidigung.Rüstung.SR, 0)` + `=choice(this.Schild.SR, this.Verteidigung.Schild.SR, 0)` |

|    Beschreibung     |           Bonus (bereits eingerechnet)           |
|:-------------------:|:------------------------------------------------:|
| Zusätzliche Rüstung | `INPUT[number:Verteidigung.Zusätzliche_Rüstung]` | 

## Angriff

### Nahkampfwaffen
```dataview
TABLE WITHOUT ID 
file.link AS "Waffe",
Reichweite,
"`dice:1d20+" + (floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)+ceil(this.Stufe/4)+1) + "|none|noform`" AS "Angriff",
"`dice:" + Schaden + "+" + floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2) + "|none|noform`"  AS "Schaden",
Schadensart,
Eigenschaften
FROM #Gegenstand/Waffe/Klasse/Nahkampfwaffe
WHERE contains(this.Waffen, file.link)
SORT file.name
```

### Schusswaffen 
```dataview
TABLE WITHOUT ID 
file.link AS "Waffe",
Range1 AS "Min RW",
Range2 AS "Gnd RW",
Range3 AS "Max RW",
"`dice:1d20+" + (floor(((this.Attribute.Geschicklichkeit)-10)/2)+ceil(this.Stufe/4)+1) + "|none|noform`" AS "Angriff",
"`dice:" + SchadenFern + "+" + floor(((this.Attribute.Geschicklichkeit)-10)/2) + "|none|noform`"  AS "Schaden",
SchadensartFern AS "Schadensart",
EigenschaftenFern AS "Eigenschaften"
FROM #Gegenstand/Waffe/Klasse/Fernkampfwaffe/Schusswaffe
WHERE contains(this.Waffen, file.link)
SORT file.name
```

### Wurfwaffen
```dataview
TABLE WITHOUT ID 
file.link AS "Waffe",
Range1 AS "Min RW",
Range2 AS "Gnd RW",
Range3 AS "Max RW",
"`dice:1d20+" + (floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)+ceil(this.Stufe/4)+1) + "|none|noform`" AS "Angriff",
"`dice:" + SchadenFern + "+" + floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2) + "|none|noform`"  AS "Schaden",
SchadensartFern AS "Schadensart",
EigenschaftenFern AS "Eigenschaften"
FROM #Gegenstand/Waffe/Klasse/Fernkampfwaffe/Wurfwaffe 
WHERE contains(this.Waffen, file.link)
SORT file.name
```

Disclaimer: Waffen haben immer Übungsbonus...

## Attribute und Fertigkeiten
> [!column  | 2 no-title]
>> ## Stärke
>> | [[Stärke]]                                                                                                                 |                                                                                  Attributswert                                                                                  |
>> | -------------------------------------------------------------------------------------------------------------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
>> | [[Attribute\|Attributswert]]                                                                                               |                                                                            `=this.Attribute.Stärke`   (`=choice(floor(((this.Attribute.Stärke)-10)/2)>0, "+" + floor(((this.Attribute.Stärke)-10)/2), floor(((this.Attribute.Stärke)-10)/2))`)                                                                          |
>> | [[Attribute#Attributswurf]]                                                                                                |                                         `$="```dice:1d20+" + Math.floor(((dv.current().Attribute.Stärke)-10)/2) + "\|none\|noform\```"`                                         |
>> | [[Rettungswurf]] `=choice(this.Rettungswürfe.Stärke=2, "⭐⭐", choice(this.Rettungswürfe.Stärke=1, "⭐",""))`              |    `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Stärke)-10)/2)+(dv.current().Rettungswürfe.Stärke*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Athletik]] `=choice(this.Fertigkeiten.Athletik=2, "⭐⭐", choice(this.Fertigkeiten.Athletik=1, "⭐",""))`               |   `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Stärke)-10)/2)+(dv.current().Fertigkeiten.Athletik*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Einschüchtern]] `=choice(this.Fertigkeiten.Einschüchtern=2, "⭐⭐", choice(this.Fertigkeiten.Einschüchtern=1, "⭐",""))` | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Stärke)-10)/2)+(dv.current().Fertigkeiten.Einschüchtern*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>
>> ## Geschicklichkeit
>> | [[Geschicklichkeit]]                  |                                                                                  Attributswert                                                                                  |
>> | --------------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
>> | [[Attribute\|Attributswert]]                |                                                                            `=this.Attribute.Geschicklichkeit`    (`=choice(floor(((this.Attribute.Geschicklichkeit)-10)/2)>0, "+" + floor(((this.Attribute.Geschicklichkeit)-10)/2), floor(((this.Attribute.Geschicklichkeit)-10)/2))`)                                                                            |
>> | [[Attribute#Attributswurf]]  |                                         `$="```dice:1d20+" + Math.floor(((dv.current().Attribute.Geschicklichkeit)-10)/2) + "\|none\|noform\```"`                                         |
>> | [[Rettungswurf]] `=choice(this.Rettungswürfe.Geschicklichkeit=2, "⭐⭐", choice(this.Rettungswürfe.Geschicklichkeit=1, "⭐",""))`          |    `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Geschicklichkeit)-10)/2)+(dv.current().Rettungswürfe.Geschicklichkeit*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Akrobatik]] `=choice(this.Fertigkeiten.Akrobatik=2, "⭐⭐", choice(this.Fertigkeiten.Akrobatik=1, "⭐",""))`               |   `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Geschicklichkeit)-10)/2)+(dv.current().Fertigkeiten.Akrobatik*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Fingerfertigkeit]] `=choice(this.Fertigkeiten.Fingerfertigkeit=2, "⭐⭐", choice(this.Fertigkeiten.Fingerfertigkeit=1, "⭐",""))`          | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Geschicklichkeit)-10)/2)+(dv.current().Fertigkeiten.Fingerfertigkeit*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>> | [[Heimlichkeit]] `=choice(this.Fertigkeiten.Heimlichkeit=2, "⭐⭐", choice(this.Fertigkeiten.Heimlichkeit=1, "⭐",""))`         | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Geschicklichkeit)-10)/2)+(dv.current().Fertigkeiten.Heimlichkeit*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>
>> ## Konstitution
>> | [[Konstitution]]                  |                                                                                  Attributswert                                                                                  |
>> | --------------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
>> | [[Attribute\|Attributswert]]                |                                                                            `=this.Attribute.Konstitution`  (`=choice(floor(((this.Attribute.Konstitution)-10)/2)>0, "+" + floor(((this.Attribute.Konstitution)-10)/2), floor(((this.Attribute.Konstitution)-10)/2))`)                                                                            |
>> | [[Attribute#Attributswurf]] |                                         `$="```dice:1d20+" + Math.floor(((dv.current().Attribute.Konstitution)-10)/2) + "\|none\|noform\```"`                                         |
>> | [[Rettungswurf]] `=choice(this.Rettungswürfe.Konstitution=2, "⭐⭐", choice(this.Rettungswürfe.Konstitution=1, "⭐",""))`          |    `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Konstitution)-10)/2)+(dv.current().Rettungswürfe.Konstitution*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>
>> ## Intelligenz
>> | [[Intelligenz]]                  |                                                                                  Attributswert                                                                                  |
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
>> | [[Weisheit]]                  |                                                                                  Attributswert                                                                                  |
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
>> | [[Charisma]]                  |                                                                                  Attributswert                                                                                  |
>> | --------------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
>> | [[Attribute\|Attributswert]]                |                                                                            `=this.Attribute.Charisma`  (`=choice(floor(((this.Attribute.Charisma)-10)/2)>0, "+" + floor(((this.Attribute.Charisma)-10)/2), floor(((this.Attribute.Charisma)-10)/2))`)                                                                            |
>> | [[Attribute#Attributswurf]] |                                         `$="```dice:1d20+" + Math.floor(((dv.current().Attribute.Charisma)-10)/2) + "\|none\|noform\```"`                                         |
>> | [[Rettungswurf]] `=choice(this.Rettungswürfe.Charisma=2, "⭐⭐", choice(this.Rettungswürfe.Charisma=1, "⭐",""))`           |    `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Charisma)-10)/2)+(dv.current().Rettungswürfe.Charisma*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Auftreten]] `=choice(this.Fertigkeiten.Auftreten=2, "⭐⭐", choice(this.Fertigkeiten.Auftreten=1, "⭐",""))`             |   `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Charisma)-10)/2)+(dv.current().Fertigkeiten.Auftreten*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"`    |
>> | [[Einschüchtern]] `=choice(this.Fertigkeiten.Einschüchtern=2, "⭐⭐", choice(this.Fertigkeiten.Einschüchtern=1, "⭐",""))`        | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Charisma)-10)/2)+(dv.current().Fertigkeiten.Einschüchtern*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>> | [[Täuschen]] `=choice(this.Fertigkeiten.Täuschen=2, "⭐⭐", choice(this.Fertigkeiten.Täuschen=1, "⭐",""))`       | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Charisma)-10)/2)+(dv.current().Fertigkeiten.Täuschen*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |
>> | [[Überzeugen]] `=choice(this.Fertigkeiten.Überzeugen=2, "⭐⭐", choice(this.Fertigkeiten.Überzeugen=1, "⭐",""))`        | `$="```dice:1d20+" + (Math.floor(((dv.current().Attribute.Charisma)-10)/2)+(dv.current().Fertigkeiten.Überzeugen*(Math.ceil(dv.current().Stufe/4)+1))) + "\|none\|noform\```"` |

## Übung

### Rüstung
```dataview
LIST
FROM #Gegenstand/Rüstung
WHERE contains(this.Übung.Rüstungen, file.link) 
SORT file.name
```
 
### Waffen
```dataview
LIST
FROM #Gegenstand/Waffe 
WHERE contains(this.Übung.Waffen, file.link) 
SORT file.name
```

### Sprachen
```dataview
LIST
FROM #Sprache
WHERE contains(this.Übung.Sprachen, file.link)
SORT file.name
```

## Werkzeuge
```dataview
LIST
FROM #Gegenstand/Werkzeug
WHERE contains(this.Übung.Werkzeuge, file.link)
SORT file.name
```

## Merkmale
### Volksmerkmale
```dataview
LIST
FROM #Merkmal
WHERE contains(this.Merkmale.Volk, file.link)
SORT file.name
```

### Talente
```dataview
LIST
FROM #Talent
WHERE contains(this.Merkmale.Talente, file.link)
SORT file.name
```

### Klassenmerkmale
```dataview
LIST
FROM #Merkmal
WHERE contains(this.Merkmale.Klasse, file.link)
SORT file.name
```

## Aussehen
Niptac ist ein kleiner, schlanker Gnom mit wildem, struppigem Haar und einer spitzen Nase. Er trägt oft schmutzige Kleidung und eine alte Lederjacke, um sich vor Wind und Wetter zu schützen. Seine Augen sind immer wachsam und vorsichtig, und er hält sich oft im Hintergrund, um nicht aufzufallen.

## Hintergrundgeschichte
Niptac wurde als jüngstes Kind einer Familie von Gnome geboren. Sein Vater war ein Magier, der in vielen Schlachten gekämpft hatte, um das Königreich zu verteidigen. Seine Mutter war eine begabte Mechanikerin und Ingenieurin, die viele nützliche Maschinen und Werkzeuge entwickelt hatte, um das Leben ihrer Familie einfacher zu gestalten.
Niptac wuchs in einer glücklichen Familie auf, leider besaß er keinerlei Talent für Magie, wie sein Vater, auch wenn er es oft versuchte Ihm beizubringen. Daher ließ er sich von seiner Mutter in die Geheimnisse der Mechanik einweihen und versuchte damit sein mangelndes magisches Geschick auszugleichen.

Eines Tages kehrte sein Vater nicht von einer Schlacht zurück, und die Familie war am Boden zerstört. Niptacs Mutter musste hart arbeiten, um die Familie über Wasser zu halten, und Niptac übernahm viele Aufgaben im Haushalt, um ihr zu helfen.

Als Niptac älter wurde, entwickelte er eine Leidenschaft für das Schmuggeln und den Handel mit verbotenen Gütern. Er erkannte, dass er damit seiner Familie helfen und seine Mutter von der harten Arbeit entlasten konnte. Er begann, seine Fähigkeiten als Dieb und Schmuggler zu entwickeln und wurde schließlich zu einem der besten in der Stadt.

Obwohl Niptac ein Dieb war, hatte er eine starke Moral und stahl nur von reichen Händlern und Adligen, die es sich leisten konnten, etwas zu verlieren. Er spendete auch regelmäßig einen Teil seines Einkommens an Bedürftige in der Stadt und unterstützte seine Familie so gut er konnte.

Niptac hat immer noch die Erinnerung an seinen Vater und den Mut, sowie die Weisheit, die er in der Schlacht gezeigt hat, in sich. Er hofft, dass er eines Tages selbst in der Lage sein wird, sein Königreich zu verteidigen und seine Familie stolz zu machen.


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
    bindTarget: InputData.Energiekern1
    evaluate: false
    value: "true"
  - type: updateMetadata
    bindTarget: InputData.Energiekern2
    evaluate: false
    value: "true"
  - type: updateMetadata
    bindTarget: InputData.Energiekern3
    evaluate: false
    value: "true"
  - type: updateMetadata
    bindTarget: InputData.Energiekern4
    evaluate: false
    value: "true"
  - type: updateMetadata
    bindTarget: InputData.Fähigkeiten.Verschwinden
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
