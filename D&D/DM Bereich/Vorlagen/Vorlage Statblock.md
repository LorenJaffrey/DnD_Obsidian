---
tags:
  - Kreatur
aliases:
  - Monster Statblock Vorlage
Größenkategorie: "[[Mittelgroß]]"
Typ: "[[Humanoide]]"
Subtyp: "[[Orks|Ork]]"
Gesinnung: "[[Chaotisch Böse]]"
Herausforderungsgrad: 20
Stufe: 3
Trefferwürfel: W10
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
  Resistenzen:
    Schadensresistenz:
      - "[[Hiebschaden]]"
      - "[[Giftschaden]]"
      - "[[Stichschaden]]"
      - "[[Wuchtschaden]]"
      - "[[Energieschaden]]"
      - "[[Nekrotischer Schaden]]"
      - "[[Feuerschaden]]"
    Schadensimmunität:
    Zustandsimmunität:
      - "[[Blind]]"
      - "[[Gepackt]]"
Angriff:
  Waffen:
    - "[[Axt]]"
    - "[[Axt]]"
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
---
# `=this.file.name`
> [!column | 2 flex | no-title]
>> ![[orc.jpg |  350]]
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
>> ```dataviewjs
>> const movement = dv.current().Bewegung;
>> var string = "|  |  | \n | ---- | ---- |";
>> for (var key in movement) {
>> if(movement[key] > 0) {
>> if (string.length > 0) {
>> string += "\n"
>> }
>> string += ("|  [[" + key + "]] | " + movement[key] + "m (" + movement[key]/1.5 + " Kästchen) |");
>> }
>> }
>> dv.paragraph(string);
>> ```
>>
>> ## Verteidigung
>>  
>> [[Trefferpunkte]]: `=this.Stufe + "" + this.Trefferwürfel + choice(floor(((this.Attribute.Konstitution)-10)/2)!=0, (" + " + this.Stufe*floor(((this.Attribute.Konstitution)-10)/2)), "")`
>> 
>> |                |                                                                                                                                                 |
>> | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
>> | Rüstung               | `=this.Verteidigung.Rüstung` `=choice(this.Verteidigung.Schild, ", ", "")` `=choice(this.Verteidigung.Schild, this.Verteidigung.Schild, "")`                                                                           |
>> | [[Rüstungsklasse]]    | `=this.Verteidigung.Natürliche_Rüstung+floor(((this.Attribute.Geschicklichkeit)-10)/2)+choice(this.Verteidigung.Rüstung.RP, this.Verteidigung.Rüstung.RP, 0)` + `=choice(this.Verteidigung.Schild, this.Verteidigung.Schild.RP, 0)` |
>> | [[Schadensreduktion]] | `=choice(this.Verteidigung.Verteidigung.Rüstung.SR, this.Verteidigung.Rüstung.SR, 0)` + `=choice(this.Verteidigung.Schild.SR, this.Verteidigung.Schild.SR, 0)`       
>>
>> ``` dataviewjs
>> var schadensresistenzen = dv.current().Verteidigung.Resistenzen.Schadensresistenz;
>> var schadensimmunitäten = dv.current().Verteidigung.Resistenzen.Schadensimmunität;
>> var zustandsimmunitäten = dv.current().Verteidigung.Resistenzen.Zustandsimmunität;
>> 
>> var schadensresistenzenString = "";
>> var schadensimmunitätenString = "";
>> var zustandsimmunitätenString = "";
>> var resistenzenString = "";
>> 
>> if (schadensresistenzen) {
>> 	schadensresistenzenString += "#### Schadensresistenzen";
>> 	for (var i = 0, j = schadensresistenzen.length; i<j; i++) {
>> 		schadensresistenzenString += "\n - " + schadensresistenzen[i];
>> 	}
>> }
>> 
>> if (schadensimmunitäten) {
>> 	schadensimmunitätenString += "#### Schadensimmunitäten";
>> 	for (var i = 0, j = schadensimmunitäten.length; i<j; i++) {
>> 		schadensimmunitätenString +=  "\n - " + schadensimmunitäten[i];
>> 	}
>> }
>> 
>> if (zustandsimmunitäten) {
>> 	zustandsimmunitätenString += "#### Zustandsimmunitäten";
>> 	for (var i = 0, j = zustandsimmunitäten.length; i<j; i++) {
>> 		zustandsimmunitätenString +=  "\n - " + zustandsimmunitäten[i];
>> 	}
>> }
>> 
>> if (schadensresistenzenString) {
>> 	resistenzenString += schadensresistenzenString;
>> }
>> if (schadensimmunitätenString) {
>> 	if (resistenzenString) {
>> 		resistenzenString += "\n"
>> 	}
>> 	resistenzenString += schadensimmunitätenString;
>> }
>> if (zustandsimmunitätenString) {
>> 	if (resistenzenString) {
>> 		resistenzenString += "\n"
>> 	}
>> 	resistenzenString += zustandsimmunitätenString;
>> }
>> if (resistenzenString) {
>> 	resistenzenString = "### Resistenzen\n" + resistenzenString;
>> 	dv.span(resistenzenString);
>> }
>> ```
>>
>> ``` dataviewjs
>> var sinne = dv.current().Sinne;
>> var sinneString = "";
>> 
>> if (sinne) {
>> 	sinneString += "## Sinne";
>> 	for (var i = 0, j = sinne.length; i<j; i++) {
>> 		sinneString +=   "\n - " + sinne[i];
>> 	}
>> 	dv.span(sinneString);
>> }
>>```
>
>> ## Attribute
>> |         |                                       [[Stärke\|ST]]                                        |                                                         [[Geschicklichkeit\|GE]]                                                          |                                          [[Konstitution\|KO]]                                           |                                          [[Intelligenz\|IN]]                                          |                                        [[Weisheit\|WE]]                                         |                                        [[Charisma\|CH]]                                         |
>> | ------- |:-------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------:|
>> | **Attributswert**        |                                  `=this.Attribute.Stärke`                                   |                                                    `=this.Attribute.Geschicklichkeit`                                                     |                                     `=this.Attribute.Konstitution`                                      |                                     `=this.Attribute.Intelligenz`                                     |                                   `=this.Attribute.Weisheit`                                    |                                   `=this.Attribute.Charisma`                                    |
>> | **Modifikator** |                          `=floor(((this.Attribute.Stärke)-10)/2)`                           |                               `=min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)`                                |                             `=floor(((this.Attribute.Konstitution)-10)/2)`                              |                             `=floor(((this.Attribute.Intelligenz)-10)/2)`                             |                           `=floor(((this.Attribute.Weisheit)-10)/2)`                            |                           `=floor(((this.Attribute.Charisma)-10)/2)`                            |
>> | **Rettungswurf**  | `=floor(((this.Attribute.Stärke)-10)/2)+(this.Rettungswürfe.Stärke*(ceil(this.Herausforderungsgrad/4)+1))` | `=min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)+(this.Rettungswürfe.Geschicklichkeit*(ceil(this.Herausforderungsgrad/4)+1))` | `=floor(((this.Attribute.Konstitution)-10)/2)+(this.Rettungswürfe.Konstitution*(ceil(this.Herausforderungsgrad/4)+1))` | `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Rettungswürfe.Intelligenz*(ceil(this.Herausforderungsgrad/4)+1))` | `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Rettungswürfe.Weisheit*(ceil(this.Herausforderungsgrad/4)+1))` | `=floor(((this.Attribute.Charisma)-10)/2)+(this.Rettungswürfe.Charisma*(ceil(this.Herausforderungsgrad/4)+1))` |
>>
>> ## Fertigkeiten
>> ```dataviewjs
>> const skills = dv.current().Fertigkeiten;
>> var string = ""; 
>> for (var key in skills) {
>> if(skills[key] > 0) {
>> if (string.length > 0) {
>> string += "\n";
>> }
>> string += "- [[" + key + "]]: +" + skills[key]*(Math.ceil(dv.current().Herausforderungsgrad/4)+1);
>> }
>> }
>> dv.paragraph(string);
>> ```
>> 
>> [[Wahrnehmung#Passive Wahrnehmung]]: `=10+floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Wahrnehmung*(ceil(this.Herausforderungsgrad/4)+1))`
>> 
>> ## Merkmale
>> `$=dv.list(dv.current().Merkmale)`
>
>> ## Angriff
>> `=choice(this.Angriff.Angriffe, "###### Mehrfachangriff " + "</br>" + this.Angriff.Angriffe, "")`
>>
>> #### Nahkampfwaffen
>> ```dataview
>> TABLE WITHOUT ID 
>> file.link AS "Waffe",
>> Reichweite,
>> floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)+ceil(this.Herausforderungsgrad/4)+1 AS "Bonus",
>> Schaden+"+"+(floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)) AS "Schaden",
>> Schadensart,
>> Eigenschaften
>> FROM #Gegenstand/Waffe/Klasse/Nahkampfwaffe 
>> WHERE contains(this.Angriff.Waffen, file.link)
>> SORT file.name
>> ```
>> 
>> #### Schusswaffen 
>> ```dataview
>> TABLE WITHOUT ID 
>> file.link AS "Waffe",
>> Range1 AS "Min RW",
>> Range2 AS "Gnd RW",
>> Range3 AS "Max RW",
>> floor(((this.Attribute.Geschicklichkeit)-10)/2)+ceil(this.Herausforderungsgrad/4)+1 AS "Bonus",
>> SchadenFern+"+"+floor((((this.Attribute.Geschicklichkeit)-10)/2)) AS "Schaden",
>> SchadensartFern AS "Schadensart",
>> EigenschaftenFern AS "Eigenschaften"
>> FROM #Gegenstand/Waffe/Klasse/Fernkampfwaffe/Schusswaffe 
>> WHERE contains(this.Angriff.Waffen, file.link)
>> SORT file.name
>> ```
>> 
>> #### Wurfwaffen
>> ```dataview
>> TABLE WITHOUT ID 
>> file.link AS "Waffe",
>> Range1 AS "Min RW",
>> Range2 AS "Gnd RW",
>> Range3 AS "Max RW",
>> floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)+ceil(this.Herausforderungsgrad/4)+1 AS "Bonus",
>> SchadenFern+"+"+(floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)) AS "Schaden",
>> SchadensartFern AS "Schadensart",
>> EigenschaftenFern AS "Eigenschaften"
>> FROM #Gegenstand/Waffe/Klasse/Fernkampfwaffe/Wurfwaffe  
>> WHERE contains(this.Angriff.Waffen, file.link)
>> SORT file.name
>> ```

- [ ] #task Template finalisieren [priority:: highest]