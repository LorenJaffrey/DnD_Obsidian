---
tags:
  - Kreatur/Pflanze
aliases: 
Größenkategorie: "[[Klein]]"
Typ: "[[Pflanzen|Pflanze]]"
Subtyp: "[[Plagen|Plage]]"
Gesinnung: "[[Neutral Böse]]"
Herausforderungsgrad: 0.125
Stufe: 1
Trefferwürfel: d6
Bewegung:
  Boden: 6
  Fliegen: 0
  Schwimmen: 0
  Klettern: 0
  Graben: 0
Sinne:
  - "[[Blindsicht]] 18m (12 Kästchen)"
Verteidigung:
  Rüstung: 
  Schild: 
  Natürliche_Rüstung: 12
  Natürliche_SR: 0
  Resistenzen:
    Schadensresistenz:
    Schadensimmunität: 
    Zustandsimmunität:
      - "[[Blind]]"
      - "[[Taub]]"
Angriff:
  Waffen: 
  Angriffe:
    - "[[Winziger Klauenhieb]]"
Attribute:
  Stärke: 6
  Geschicklichkeit: 13
  Konstitution: 12
  Intelligenz: 4
  Weisheit: 8
  Charisma: 3
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
  Heimlichkeit: 1
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
  - "versteht [[Gemeinsprache]]"
Merkmale:
  - "[[Falsches Erscheinungsbild]]"
Anzahl_Legendäre_Aktionen:
Legendäre_Aktionen:
---
# `=this.file.name`
> [!column | 2 flex | no-title]
>> ![[twig_blight.png|250]]
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