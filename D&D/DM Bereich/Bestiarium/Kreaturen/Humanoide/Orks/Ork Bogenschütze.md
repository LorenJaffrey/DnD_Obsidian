---
aliases:
- Orks
tags:
- Kreatur/Humanoide/Ork
Größenkategorie: "[[Mittelgroß]]"
Typ: "[[Humanoide]]"
Subtyp: "[[Orks|Ork]]"
Gesinnung: "[[Chaotisch Böse]]"
Herausforderungsgrad: 0.5
Stufe: 3
Trefferwürfel: W8
Bewegung:
  Boden: 9
  Fliegen:
  Schwimmen:
  Klettern: 
  Graben:
Sinne:
  - "[[Dunkelsicht]] 36m (24 Kästchen)"
Verteidigung:
  Rüstung: "[[Lederrüstung]]"
  Schild:
  Natürliche_Rüstung: 10
  Natürliche_SR: 0
  Resistenzen:
    Schadensresistenz:
    Schadensimmunität: 
    Zustandsimmunität:
Angriff:
  Waffen:
    - "[[Kurzschwert]]"
    - "[[Kurzbogen]]"
Attribute:
  Stärke: 14
  Geschicklichkeit: 16
  Konstitution: 14
  Intelligenz: 8
  Weisheit: 11
  Charisma: 10
Rettungswürfe:
  Stärke: 0
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
  Überlebenskunst: 0
  Überzeugen: 0
  Wahrnehmung: 0
Sprachen:
  - "[[Gemeinsprache]]"
  - "[[Orkisch]]"
Merkmale:
  - "[[Aggressiv]]"
  - "[[Überspannen]]"
Anzahl_Legendäre_Aktionen:
Legendäre_Aktionen:
---
# `=this.file.name`
> [!column | 2 flex | no-title]
>> ![[orc_archer.png | 350]]
>> ## `=this.file.name`
>> |  |  |
>> | ---- | ---- |
>> | [[Größenkategorie]] | `=this.Größenkategorie` |
>> | Typ | `=this.Typ` |
>> | Subtyp | `=this.Subtyp` |
>> | [[Gesinnung]] | `=this.Gesinnung` |
>> | [[Herausforderungsgrad]] | `=this.Herausforderungsgrad` |
>> | [[Übung\|Übungsbonus]] | (Übungsbonus:: `=(ceil(this.Herausforderungsgrad/4)+1)`) |
>> | [[Sprachen]] | `=this.Sprachen` |
>
>> ## Bewegung
>> ```dynamic-embed
>> [[embed Statblock Kreatur Bewegung]]
>> ```
>>
>> ```dynamic-embed
>> [[embed Statblock Kreatur Sinne]]
>>```
>>
>> ## Verteidigung
>> ```dynamic-embed
>> [[embed Statblock Kreatur Verteidigung]]
>>```
>>
>> ```dynamic-embed
>> [[embed Statblock Kreatur Resistenzen]]
>> ```
>
>> ## Attribute
>> ```dynamic-embed
>> [[embed Statblock Kreatur Attribute]]
>> ```
>>
>> ## Fertigkeiten
>> ```dynamic-embed
>> [[embed Statblock Kreatur Fertigkeiten]]
>> ```
>> 
>> [[Wahrnehmung#Passive Wahrnehmung]]: `=10+floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Wahrnehmung*(ceil(this.Herausforderungsgrad/4)+1))`
>>
>> ```dynamic-embed
>> [[embed Statblock Kreatur Merkmale]]
>> ```
>>
>> ```dynamic-embed
>> [[embed Statblock Kreatur Legendäre Aktionen]]
>> ```
>
>> ## Angriff
>> #### Nahkampfwaffen
>> ```dynamic-embed
>> [[embed Statblock Kreatur Waffen Nahkampf]]
>> ```
>> 
>> #### Schusswaffen 
>> ```dynamic-embed
>> [[embed Statblock Kreatur Waffen Fernkampf]]
>> ```
>> 
>> #### Wurfwaffen
>> ```dynamic-embed
>> [[embed Statblock Kreatur Waffen Wurf]]
>> ```