---
tags:
  - Kreatur
aliases:
  - Monster Statblock Vorlage
Größenkategorie: "[[Mittelgroß]]"
Typ: "[[Humanoide]]"
Subtyp: "[[Orks|Ork]]"
Gesinnung: "[[Chaotisch Böse]]"
Stufe: 3
Herausforderungsgrad: 1
Bewegung: 
  Boden: 9
  Fliegen: 0
  Schwimmen: 0
  Klettern: 0
  Graben: 0
Rüstung: "[[Lederrüstung]]"
Schild: "[[Holzschild]]"
Natürliche_Rüstung: 10
Waffen:
  - "[[Axt]]"
  - "[[Kurzbogen]]"
Trefferwürfel: "W10"
Attribute:
  Stärke: 12
  Geschicklichkeit: 18
  Konstitution: 14
  Intelligenz: 8
  Weisheit: 14
  Charisma: 10
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
  Nachforschungen: 0
  Naturkunde: 0
  Religion: 0
  Täuschen: 0
  Überlebenskunst: 1
  Überzeugen: 0
  Wahrnehmung: 1
Sprachen:
  - "[[Gemeinsprache]]"
  - "[[Orkisch]]"
Merkmale:
  - "[[Aggressiv]]"
  - "[[Unbeugsamkeit]]"
  - "[[Amorph]]"
---
# `=this.file.name`

> [!infobox]
> # `=this.file.name`
> ![[orc.jpg]]
> ###### Stats
> | Type | Stat |
> | ---- | ---- |
> | Größenkategorie | `=this.Größenkategorie` |
> | Typ | `=this.Typ` |
> | Subtyp | `=this.Subtyp` |
> | Gesinnung | `=this.Gesinnung` |
> ---
> [[Herausforderungsgrad]]: `=this.Herausforderungsgrad`
> [[Sprachen]]: `=this.Sprachen`

> [!column | 2 flex ]
>> ## Bewegung
>> | Bewegungsart |                                                                                                                                                                         |
>> | ------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
>> | Boden        | `=choice(this.Bewegung.Boden>0, this.Bewegung.Boden + " m", "")` `=choice(this.Bewegung.Boden>0, ("(" + this.Bewegung.Boden/1.5) + " Kästchen)", "--")`                 |
>> | Fliegen      | `=choice(this.Bewegung.Fliegen>0, this.Bewegung.Fliegen + " m", "")` `=choice(this.Bewegung.Fliegen>0, ("(" + this.Bewegung.Fliegen/1.5) + "Kästchen)", "--")`          |
>> | Schwimmen    | `=choice(this.Bewegung.Schwimmen>0, this.Bewegung.Schwimmen + " m", "")` `=choice(this.Bewegung.Schwimmen>0, ("(" + this.Bewegung.Schwimmen/1.5) + " Kästchen)", "--")` |
>> | Klettern     | `=choice(this.Bewegung.Klettern>0, this.Bewegung.Klettern + " m", "")` `=choice(this.Bewegung.Klettern>0, ("(" + this.Bewegung.Klettern/1.5) + " Kästchen)", "--")`     |
>> | Graben       | `=choice(this.Bewegung.Graben>0, this.Bewegung.Graben + " m", "")` `=choice(this.Bewegung.Graben>0, ("(" + this.Bewegung.Graben/1.5) + " Kästche)", "--")`              |
>>
>>## Verteidigung
>> [[Trefferpunkte]]: `=this.Stufe + "" + this.Trefferwürfel + choice(floor(((this.Attribute.Konstitution)-10)/2)!=0, (" + " + this.Stufe*floor(((this.Attribute.Konstitution)-10)/2)), "")`
>>
>> | Rüstung               | [[Rüstungsklasse]]                                                                                                                                                 |
>> | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
>> | Rüstung               | `=this.Rüstung` `=choice(this.Schild, ", ", "")` `=choice(this.Schild, this.Schild, "")`                                                                           |
>> | [[Rüstungsklasse]]    | `=this.Natürliche_Rüstung+floor(((this.Attribute.Geschicklichkeit)-10)/2)+choice(this.Rüstung.RP, this.Rüstung.RP, 0)` + `=choice(this.Schild, this.Schild.RP, 0)` |
>> | [[Schadensreduktion]] | `=choice(this.Rüstung.SR, this.Rüstung.SR, 0)` + `=choice(this.Schild.SR, this.Schild.SR, 0)`           
>
>> ## Angriff
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
>> ### Schusswaffen 
>> ```dataview
>> TABLE WITHOUT ID 
>> file.link AS "Waffe",
>> Range1 AS "Min RW",
>> Range2 AS "Gnd RW",
>> Range3 AS "Max RW",
>> floor(((this.Attribute.Geschicklichkeit)-10)/2)+ceil(this.Stufe/4)+1 AS "Bonus",
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

> [!column | 2 ]
>> ## Attribute
>> |         |                                       [[Stärke\|ST]]                                        |                                                         [[Geschicklichkeit\|GE]]                                                          |                                          [[Konstitution\|KO]]                                           |                                          [[Intelligenz\|IN]]                                          |                                        [[Weisheit\|WE]]                                         |                                        [[Charisma\|CH]]                                         |
>> | ------- |:-------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------:|
>> |         |                                  `=this.Attribute.Stärke`                                   |                                                    `=this.Attribute.Geschicklichkeit`                                                     |                                     `=this.Attribute.Konstitution`                                      |                                     `=this.Attribute.Intelligenz`                                     |                                   `=this.Attribute.Weisheit`                                    |                                   `=this.Attribute.Charisma`                                    |
>> | **MOD** |                          `=floor(((this.Attribute.Stärke)-10)/2)`                           |                               `=min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)`                                |                             `=floor(((this.Attribute.Konstitution)-10)/2)`                              |                             `=floor(((this.Attribute.Intelligenz)-10)/2)`                             |                           `=floor(((this.Attribute.Weisheit)-10)/2)`                            |                           `=floor(((this.Attribute.Charisma)-10)/2)`                            |
>> | **RW**  | `=floor(((this.Attribute.Stärke)-10)/2)+(this.Rettungswürfe.Stärke*(ceil(this.Stufe/4)+1))` | `=min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)+(this.Rettungswürfe.Geschicklichkeit*(ceil(this.Stufe/4)+1))` | `=floor(((this.Attribute.Konstitution)-10)/2)+(this.Rettungswürfe.Konstitution*(ceil(this.Stufe/4)+1))` | `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Rettungswürfe.Intelligenz*(ceil(this.Stufe/4)+1))` | `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Rettungswürfe.Weisheit*(ceil(this.Stufe/4)+1))` | `=floor(((this.Attribute.Charisma)-10)/2)+(this.Rettungswürfe.Charisma*(ceil(this.Stufe/4)+1))` |
>>
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
>> [[Wahrnehmung#Passive Wahrnehmung]]: `=10+floor(((this.Attribute.Weisheit)-10)/2)`
>
>> ## Merkmale
>> ```dataviewjs
>> const merkmale = dv.current().Merkmale; 
>> for (var i = 0, j = merkmale.length; i < j; i++) {
>> dv.span("![[" + dv.page(merkmale[i]).file.name + " | no-title]]");
>> }
>> ```