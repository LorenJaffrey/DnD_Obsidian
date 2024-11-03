---
aliases: 
tags:
  - Kreatur/Drache
Größenkategorie: "[[Riesig]]"
Typ: "[[Drachen|Drache]]"
Subtyp: "[[Chromatische Drachen]]"
Gesinnung: "[[Chaotisch Böse]]"
Herausforderungsgrad: 13
Stufe: 16
Trefferwürfel: d12
Bewegung:
  Boden: 12
  Fliegen: 24
  Schwimmen: 12
  Klettern: 
  Graben: 9
Sinne:
  - "[[Dunkelsicht]] 36m (24 Kästchen)"
  - "[[Blindsicht]] 18m (12 Kästchen)"
Verteidigung:
  Rüstung: 
  Schild: 
  Natürliche_Rüstung: 18
  Natürliche_SR: 2
  Resistenzen:
    Schadensresistenz: 
    Schadensimmunität:
      - "[[Kälteschaden]]"
    Zustandsimmunität: 
Angriff:
  Waffen:
  Angriffe:
    - "[[Mächtiger Biss]]"
    - "[[Klauenhieb]]"
    - "[[Schwanzhieb]]"
Attribute:
  Stärke: 22
  Geschicklichkeit: 10
  Konstitution: 22
  Intelligenz: 8
  Weisheit: 12
  Charisma: 12
Rettungswürfe:
  Stärke: 0
  Geschicklichkeit: 1
  Konstitution: 1
  Intelligenz: 0
  Weisheit: 1
  Charisma: 1
Fertigkeiten:
  Akrobatik: 0
  Arkane_Kunde: 0
  Athletik: 0
  Auftreten: 0
  Einschüchtern: 0
  Fingerfertigkeit: 0
  Geschichte: 0
  Heilkunde: 0
  Heimlichkeit: 1
  Mit_Tieren_umgehen: 0
  Motiv_erkennen: 0
  Nachforschungen: 0
  Naturkunde: 0
  Religion: 0
  Täuschen: 0
  Überlebenskunst: 0
  Überzeugen: 0
  Wahrnehmung: 2
Sprachen:
  - "[[Gemeinsprache]]"
  - "[[Drakonisch]]"
Merkmale:
  - "[[Eiswandeln]]"
  - "[[Legendäre Resistenz]]"
  - "[[Kälteodem]]"
  - "[[Schreckliche Präsenz]]"
  - "[[Mehrfachangriff Weißer Drache]]"
  - "[[Kälteaura]]"
Anzahl_Legendäre_Aktionen: 3
Legendäre_Aktionen:
  - "[[Aufspüren]]"
  - "[[Schwanzhieb]]"
  - "[[Flügelschlag]]"
---
# `=this.file.name`
> [!column | 2 flex | no-title]
>> ![[dragon_white.png | 350]]
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
>> ``` dynamic-embed
>> [[embed Statblock Kreatur Sinne]]
>>```
>>
>> ## Verteidigung
>> ``` dynamic-embed
>> [[embed Statblock Kreatur Verteidigung]]
>>```
>>
>> ``` dynamic-embed
>> [[embed Statblock Kreatur Resistenzen]]
>> ```
>
>> ## Attribute
>> ``` dynamic-embed
>> [[embed Statblock Kreatur Attribute]]]
>> ```
>>
>> ## Fertigkeiten
>> ```dynamic-embed
>> [[embed Statblock Kreatur Fertigkeiten]]
>> ```
>> 
>> [[Wahrnehmung#Passive Wahrnehmung]]: `=10+floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Wahrnehmung*(ceil(this.Herausforderungsgrad/4)+1))`
>>
>>```dynamic-embed
>>[[embed Statblock Kreatur Merkmale]]
>>```
>>
>> ``` dynamic-embed
>> [[embed Statblock Kreatur Legendäre Aktionen]]]
>> ```
>
>> ## Angriff
>> ```dynamic-embed
>> [[embed Statblock Kreatur Angriff Nahkampf]]
>> ```
>>
>> ```dynamic-embed
>> [[embed Statblock Kreatur Angriff Fernkampf]]
>> ```