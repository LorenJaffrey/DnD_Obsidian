---
aliases:
- Orks
tags:
- Kreatur/Monstrosität/Ankheg
Größenkategorie: "[[Groß]]"
Typ: "[[Monstrositäten|Monstrosität]]"
Subtyp: "[[Ankhegs|Ankheg]]"
Gesinnung: Gesinnungslos
Herausforderungsgrad: 2
Stufe: 6
Trefferwürfel: d10
Bewegung:
  Boden: 9
  Fliegen:
  Schwimmen:
  Klettern: 
  Graben: 3
Sinne:
  - "[[Dunkelsicht]] 18m (12 Kästchen)"
  - "[[Erschütterungssinn]] 18m (12 Kästchen)"
Verteidigung:
  Rüstung:
  Schild:
  Natürliche_Rüstung: 13
  Natürliche_SR: 1
  Resistenzen:
    Schadensresistenz:
    Schadensimmunität: 
    Zustandsimmunität:
Angriff:
  Angriffe:
    - "[[Klauenhieb]]"
Attribute:
  Stärke: 17
  Geschicklichkeit: 11
  Konstitution: 13
  Intelligenz: 1
  Weisheit: 13
  Charisma: 6
Rettungswürfe:
  Stärke: 0
  Geschicklichkeit: 0
  Konstitution: 0
  Intelligenz: 0
  Weisheit: 0
  Charisma: 0
Fertigkeiten:
  Akrobatik: 0
  Arkane_Kunde: 0
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
  Naturkunde: 0
  Religion: 0
  Täuschen: 0
  Überlebenskunst: 0
  Überzeugen: 0
  Wahrnehmung: 0
Sprachen:
Merkmale:
  - "[[Säure versprühen]]"
  - "[[Umschlingender Angriff]]"
  - "[[Säureangriff]]"
Anzahl_Legendäre_Aktionen:
Legendäre_Aktionen:
---
# `=this.file.name`
> [!column | 2 flex | no-title]
>> ![[ankheg.avif]]
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