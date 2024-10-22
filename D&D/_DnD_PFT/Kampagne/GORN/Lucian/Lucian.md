---
Stufe: 5
Bewegung: 6
Verteidigung:
  Natürliche_Rüstung: 10
  Zusätzliche_Rüstung: 1
  Rüstung: "[[Beschlagene Lederrüstung]]"
  Schild: 
Waffen:
- "[[Dolch]]"
- "[[Kampfstab]]"
Gesundheit:
  MaxTP: 38
  TP: 38
  TW: 5
  TempTP: 0
Attribute:
  Stärke: 10
  Geschicklichkeit: 14
  Konstitution: 13
  Intelligenz: 14
  Weisheit: 8
  Charisma: 18
Rettungswürfe:
  Stärke: 0
  Geschicklichkeit: 0
  Konstitution: 0
  Intelligenz: 0
  Weisheit: 1
  Charisma: 1
Fertigkeiten:
  Akrobatik: 0
  Arkane_Kunde: 1
  Athletik: 0
  Auftreten: 0
  Einschüchtern: 0
  Fingerfertigkeit: 0
  Geschichte: 1
  Heilkunde: 0
  Heimlichkeit: 0
  Mit_Tieren_umgehen: 0
  Motiv_erkennen: 0
  Nachforschungen: 1
  Naturkunde: 0
  Religion: 0
  Täuschen: 1
  Überlebenskunst: 0
  Überzeugen: 0
  Wahrnehmung: 0
Übung:
  Sprachen:
    - "[[Gemeinsprache]]"
    - "[[Infernalisch]]"
    - "[[Abyssisch]]"
    - "[[Urtümlich]]"
  Werkzeuge:
  Rüstungen:
    - "[[Leichte Rüstung]]"
  Waffen:
    - "[[Einfache Waffen]]"
Aussehen:
  Geschlecht: männlich
  Alter: 39 Jahre
  Größenkategorie: "[[Mittelgroß]]"
  Größe: 184 cm
  Gewicht: 165 Pfund
  Augenfarbe: Gold
  Haarfarbe: Schwarz
  Hautfarbe: Menschlich
Merkmale:
  Volk:
    - "[[Dunkelsicht]]"
    - "[[Höllische Resistenz]]"
    - "[[Infernalisches Erbe]]"
  Klasse:
    - "[[Paktmagie]]"
    - "[[Pakt des Buches]]"
    - "[[Segen des dunklen Meisters]]"
    - "[[Qualvoller Strahl]]"
    - "[[Maske der vielen Gesichter]]"
  Talente:
    - "[[Infernalische Konstitution]]"
Hintergrund:
  Volk: "[[Tieflinge|Tiefling]]"
  Klasse: "[[Hexenmeister]]"
  Subklasse: "[[Der Unhold]]"
  Gesinnung: "[[Chaotisch Neutral]]"
  Hintergrund: "[[Weiser]]"
Persönlichkeit:
  Persönlichkeitsmerkmale:
  - wortgewandt
  - extrovertiert 
  - strategisch
  Ideale: Wissen, Macht, Selbstverwirklichung, Selbstfindung
  Bindungen: Buch der Schatten, Teuflischer Pakt
  Makel: eitel, egoistisch, kein Teilen von Gedanken oder Plänen
tags:
- Charakter/GORN
---
# `=this.file.name`

> [!infobox]
> > ![[Lucian.jpg]]
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

> [!checks | no-title] 
> -  
> 	- [[Glück|Glückspunkte]] 
> 	- [x] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> -  
> 	- [[Erschöpft|Erschöpfung]]     
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 

## Lucian
### Aufladungen
|           |               [[Thaumaturgie]]                |             [[Höllischer Tadel]]              |
| --------- |:---------------------------------------------:|:---------------------------------------------:|
| Maximal   | <input type="checkbox" unchecked id="dabe36"> | <input type="checkbox" unchecked id="c0a200"> |
| Aufladung |                [[Lange Rast]]                 |                [[Lange Rast]]                 |

> [!checks | no-title] 
> -  
> 	- [[Stecken der Verteidigung]]     
> 	- [x] %% %% 
> 	- [x] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 

## Bewegung
| Gehen                                              | [[Spurt]]                                          | [[Hochsprung]] mit Anlauf                                   | [[Hochsprung]] ohne Anlauf                                    | [[Weitsprung]] mit Anlauf                 | [[Weitsprung]] ohne Anlauf                  |
| -------------------------------------------------- | -------------------------------------------------- | ----------------------------------------------------------- | ------------------------------------------------------------- | ----------------------------------------- | ------------------------------------------- |
| `=this.Bewegung*1.5` m (`=this.Bewegung` Kästchen) | `=this.Bewegung*3` m (`=this.Bewegung*2` Kästchen) | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)` m | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)/2` m | `=round((this.Attribute.Stärke*0.3),2)` m | `=round((this.Attribute.Stärke*0.3)/2,2)` m |

## Verteidigung
> [!column | no-title] 
>> ### Gesundheit
>> |         | [[Trefferpunkte]]        | [[Trefferwürfel]] (`=this.Hintergrund.Klasse.Trefferwürfel`)       | [[Temporäre Trefferpunkte]] |
>> | ------- | ------------------------ | ------------------------ | --------------------------- |
>> | Maximal | `=this.Gesundheit.MaxTP` | `=this.Stufe` |                             |
>> | Aktuell | `INPUT[number():Gesundheit.TP]`    |`INPUT[number():Gesundheit.TW]` | `INPUT[number():Gesundheit.TempTP]`   |
>
>>### Rüstung
>>|                                                                   Rüstung                                                                    |                                                                                        [[Rüstungsklasse]]                                                                                         |                                                        [[Schadensreduktion]]                                                         |
>>|:--------------------------------------------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------:|
>>| `=this.Verteidigung.Rüstung` `=choice(this.Verteidigung.Schild, ", ", "")` `=choice(this.Verteidigung.Schild, this.Verteidigung.Schild, "")` | `=this.Verteidigung.Natürliche_Rüstung+floor(((this.Attribute.Geschicklichkeit)-10)/2)+choice(this.Verteidigung.Rüstung.RP, this.Verteidigung.Rüstung.RP, 0)+this.Verteidigung.Zusätzliche_Rüstung` + `=choice(this.Verteidigung.Schild, this.Verteidigung.Schild.RP, 0)` | `=choice(this.Verteidigung.Rüstung.SR, this.Verteidigung.Rüstung.SR, 0)` + `=choice(this.Schild.SR, this.Verteidigung.Schild.SR, 0)` |

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
>
>> ## Schauerliche Anrufungen (max. `$=dv.page(dv.current().Hintergrund.Klasse).Bekannte_Anrufungen["Stufe"+dv.current().Stufe]`)
>> ```dataview
>> LIST
>> FROM #Merkmal/Klasse/Hexenmeister/Schauerliche_Anrufungen 
>> WHERE contains(this.Merkmale.Klasse, file.link)
>> SORT file.name
>> ```

## Hintergrundgeschichte

### Aussehen
Lucian Blackthorn ist ein männlicher Tiefling-Hexenmeister von auffallender Erscheinung. 
Er ist groß und schlank mit einer athletischen Statur. 
Seine Haut ist menschlich und seine Augen leuchten in einem lebhaften Goldton, was ihm einen exotischen und fesselnden Blick verleiht. 
Sein Haar ist wild und schwarz, oft in unkonventionellen Frisuren gestylt, und er trägt einen gepflegten Drei-Tage-Bart, der sein selbstbewusstes Lächeln betont.

Lucians Hörner sind lang und geschwungen, ähnlich wie die eines gehörnten Dämons, und sie sind mit goldenen Verzierungen verziert, die seine Stärke und Macht betonen. 
Er kleidet sich gerne in auffällige und extravagante Roben, die mit goldenen oder silbernen Akzenten geschmückt sind und seinen selbstbewussten und extrovertierten Charakter widerspiegeln.

## Charakterbeschreibung
Lucian wurde als Sohn einer angesehenen Hexenmeisterfamilie in einer düsteren und mysteriösen Stadt geboren. 
Von klein auf war er von der Magie fasziniert und zeigte ein außergewöhnliches Talent für die dunklen Künste. 
Seine Eltern erkannten sein Potenzial und unterrichteten ihn in den Geheimnissen der Hexerei und des Okkultismus.

Mit der Zeit entwickelte sich Lucians Persönlichkeit zu einem extrovertierten und charismatischen Charakter, der es liebte, die Menschen um sich herum zu beeindrucken und zu unterhalten. 
Er reiste durch die Welt, um sein Wissen über die Magie zu erweitern und seine Fähigkeiten als Hexenmeister zu perfektionieren. 
Während seiner Reisen traf er auf verschiedene Abenteurergruppen und beteiligte sich an epischen Schlachten gegen dunkle Mächte und gefährliche Kreaturen.

Lucian ist bekannt für seine unkonventionellen Methoden und seinen unbändigen Hunger nach Macht und Wissen. 
Er ist jedoch auch bereit, seine Fähigkeiten und seine Magie einzusetzen, um denjenigen zu helfen, die seine Hilfe suchen und die gegen das Böse kämpfen. 
Sein Ruf als furchtloser und charismatischer Hexenmeister verbreitet sich weit und breit, und sein außergewöhnliches Aussehen und seine theatralische Persönlichkeit machen ihn zu einer unvergesslichen Figur in jeder Gesellschaft, der er begegnet.

Trotz seiner extrovertierten Natur und seinem gelegentlichen Hang zur Dramatik ist Lucian nicht ohne innere Dämonen.
Er trägt die Last seiner tieflingischen Herkunft und die ständige Versuchung der dunklen Künste, die in ihm schlummern. 
Er ist jedoch entschlossen, seine Kräfte für das Gute einzusetzen und das Böse zu bekämpfen, auch wenn er manchmal am Rande des Abgrunds tanzt.

Das ist Lucian Blackthorn, ein extrovertierter und charismatischer Tiefling-Hexenmeister, der mit seinem exotischen Aussehen, seiner theatralischen Persönlichkeit und seinen mächtigen Hexenmeisterzaubern die Menschen um sich herum fasziniert und beeindruckt.

Lucian ist ein Charakter mit extrovertierter Persönlichkeit und einem ausgeprägten Selbstbewusstsein. 
Er liebt es, im Mittelpunkt der Aufmerksamkeit zu stehen und zieht die Blicke anderer auf sich, sei es durch seine imposante Erscheinung oder seine gewandte Art zu sprechen.
Er ist charmant und überzeugend, mit einer ausgeprägten sozialen Intelligenz, die es ihm ermöglicht, mit Menschen auf unterschiedlichen Ebenen zu interagieren.

Lucian ist ein leidenschaftlicher Redner und liebt es, seine magischen Kräfte und sein Wissen über die dunklen Künste zu präsentieren. 
Er ist bekannt für seine theatralischen Auftritte und seine Fähigkeit, die Massen zu begeistern und zu faszinieren.
Er ist ein extrovertierter Entertainer und liebt es, die Grenzen des Konventionellen zu überschreiten und neue Erfahrungen zu machen.

Trotz seines extrovertierten Charakters ist Lucian auch klug und strategisch in seinen Entscheidungen. 
Er ist ein erfahrener Hexenmeister, der seine magischen Kräfte geschickt einsetzt, um seine Ziele zu erreichen und seine Feinde zu besiegen. 
Er ist jedoch auch bekannt für seine Unberechenbarkeit und seine Fähigkeit, in unerwartete Richtungen zu handeln, was ihn zu einem faszinierenden und manchmal beängstigenden Charakter macht.

Der Name des Unholdes muss erfahren werden um gesamtheitlich Macht über ihn zu gelangen. 
Der Unhold ist schon lange Begleiter der Familie und ist Fluch und Segen zu gleich. 
Er hilft in Notsituationen und kämpft an der Seite der Familie, verfolgt aber seine eigenen eher dunklen Interessen. 