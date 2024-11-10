---
tags:
  - Kreatur
aliases:
Größenkategorie: "[[Mittelgroß]]"
Typ: "[[Humanoide]]"
Subtyp: "[[Orks|Ork]]"
Gesinnung: "[[Chaotisch Böse]]"
Herausforderungsgrad: 20
Stufe: 3
Trefferwürfel: d10
Bewegung:
  Boden: 9
  Fliegen: 3
  Schwimmen: 6
  Klettern: 
  Graben: 6
Sinne:
  - "[[Blindsicht]] 18m (12 Kästchen)"
  - "[[Dunkelsicht]] 36m (24 Kästchen)"
Verteidigung:
  Rüstung: "[[Lederrüstung]]"
  Schild: "[[Holzschild]]"
  Natürliche_Rüstung: 10
  Natürliche_SR: 0
  Resistenzen:
    Schadensresistenz:
      - "[[Hiebschaden]]"
      - "[[Stichschaden]]"
      - "[[Wuchtschaden]]"
    Schadensimmunität: 
    Zustandsimmunität:
      - "[[Blind]]"
      - "[[Gepackt]]"
Angriff:
  Waffen:
    - "[[Kurzschwert]]"
    - "[[Kurzbogen]]"
  Angriffe: "Die Kreatur führt drei Angriffe aus: Zwei mit ihrem [[Langschwert]] und eine mit ihrem [[Biss]] oder zwei Angriffe mit ihrem [[Kurzbogen]]."
Attribute:
  Stärke: 12
  Geschicklichkeit: 10
  Konstitution: 14
  Intelligenz: 8
  Weisheit: 13
  Charisma: 10
Rettungswürfe:
  Stärke: 1
  Geschicklichkeit: 0
  Konstitution: 1
  Intelligenz: 0
  Weisheit: 2
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
  Heimlichkeit: 2
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
  - "[[Behändes Entkommen]]"
  - "[[Drakonische Abstammung]]"
Anzahl_Legendäre_Aktionen: 3
Legendäre_Aktionen:
  - "[[Augenstrahlen]]"
Zauberplätze:
  Grad_1: 4
  Grad_2: 0
  Grad_3: 0
  Grad_4: 0
  Grad_5: 0
  Grad_6: 0
  Grad_7: 0
  Grad_8: 0
  Grad_9: 0
Zauber:
  - "[[Gift versprühen]]"
  - "[[Druidenkunst]]"
  - "[[Shillelagh]]"
  - "[[Donnerwoge]]"
  - "[[Wunden heilen]]"
  - "[[Mit Tieren sprechen]]"
  - "[[Nebelschritt]]"
  - "[[Identifizieren]]"
  - "[[Heilendes Wort]]"
  - "[[Schwache Genesung]]"
  - "[[Fallen finden]]"
  - "[[Spurloses Gehen]]"
---
# `=this.file.name`
> [!column | 2 flex | no-title]
>> ![[orc.jpg | 350]]
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
>> #### Nahkampfwaffen
>> ``` dynamic-embed
>> [[embed Statblock Kreatur Waffen Nahkampf]]]
>> ```
>> 
>> #### Schusswaffen 
>> ``` dynamic-embed
>> [[embed Statblock Kreatur Waffen Fernkampf]]]
>> ```
>> 
>> #### Wurfwaffen
>> ``` dynamic-embed
>> [[embed Statblock Kreatur Waffen Wurf]]]
>> ```

- [x] #task Template finalisieren  [priority:: highest]

> [!column | 2 flex ]
>> ## Zauberplätze
>> | [[Zaubergrad\|Grad]] |              1              |              2              |              3              |              4              |              5              |              6              |              7              |              8              |              9              |
>> | -------------------- |:---------------------------:|:---------------------------:|:---------------------------:|:---------------------------:|:---------------------------:|:---------------------------:|:---------------------------:|:---------------------------:|:---------------------------:|
>> | Anzahl               | `=this.Zauberplätze.Grad_1` | `=this.Zauberplätze.Grad_2` | `=this.Zauberplätze.Grad_3` | `=this.Zauberplätze.Grad_4` | `=this.Zauberplätze.Grad_5` | `=this.Zauberplätze.Grad_6` | `=this.Zauberplätze.Grad_7` | `=this.Zauberplätze.Grad_8` | `=this.Zauberplätze.Grad_9` |
>>
>> ## Zauber
>> `$=dv.list(dv.current().Zauber)`