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
Trefferwürfel: W12
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
  Resistenzen:
    Schadensresistenz: 
    Schadensimmunität: 
      - "[[Kälteschaden]]"
    Zustandsimmunität: 
Angriff:
  Waffen:
    - "[[Kältebiss]]"
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
>> 	if(skills[key] > 0) {
>> 		if (string.length > 0) {
>> 			string += "\n";
>> 		}
>> 		string += "- [[" + key + "]]: +" + skills[key]*(Math.ceil(dv.current().Herausforderungsgrad/4)+1);
>> 	}
>> }
>> dv.paragraph(string);
>> ```
>> 
>> [[Wahrnehmung#Passive Wahrnehmung]]: `=10+floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Wahrnehmung*(ceil(this.Herausforderungsgrad/4)+1))`
>>
>> ``` dataviewjs
>> var merkmale = dv.current().Merkmale;
>> var aktionen = [];
>> var bonusaktionen = [];
>> var reaktionen = [];
>> var passiv = [];
>> 
>> var merkmaleString = "";
>> var aktionenString = "";
>> var bonusaktionenString = "";
>> var reaktionenString = "";
>> var passivString = "";
>> 
>> var aktuellesMerkmal;
>> 
>> for (var i = 0, j = merkmale.length; i<j; i++) {
>> 	aktuellesMerkmal = dv.page(merkmale[i]);
>> 
>> 	if (typeof(aktuellesMerkmal.Einsatz) == "object") {
>> 		if (dv.page(aktuellesMerkmal.Einsatz).file.name == dv.parse("[[Aktion]]").path)  {
>> 			aktionen.push(merkmale[i]);
>> 		}
>> 		if (dv.page(aktuellesMerkmal.Einsatz).file.name == dv.parse("[[Bonusaktion]]").path)  {
>> 			bonusaktionen.push(merkmale[i]);
>> 		}
>> 		if (dv.page(aktuellesMerkmal.Einsatz).file.name == dv.parse("[[Reaktion]]").path)  {
>> 			reaktionen.push(merkmale[i]);
>> 		}
>> 	}
>> 	else {
>> 		passiv.push(merkmale[i]);
>> 	}
>> }
>> 
>> if (aktionen.length > 0) {
>> 	aktionenString += "#### Aktionen";
>> 	for (var i = 0, j = aktionen.length; i<j; i++) {
>> 		aktionenString += "\n - " + aktionen[i];
>> 	}
>> }
>> 
>> if (bonusaktionen.length > 0) {
>> 	bonusaktionenString += "#### Bonusaktionen";
>> 	for (var i = 0, j = bonusaktionen.length; i<j; i++) {
>> 		bonusaktionenString +=  "\n - " + bonusaktionen[i];
>> 	}
>> }
>> 
>> if (reaktionen.length > 0) {
>> 	reaktionenString += "#### Reaktionen";
>> 	for (var i = 0, j = reaktionen.length; i<j; i++) {
>> 		reaktionenString +=  "\n - " + reaktionen[i];
>> 	}
>> }
>> 
>> if (passiv.length > 0) {
>> 	passivString += "#### Passive Merkmale";
>> 	for (var i = 0, j = passiv.length; i<j; i++) {
>> 		passivString +=  "\n - " + passiv[i];
>> 	}
>> }
>> 
>> if (aktionenString) {
>> 	merkmaleString += aktionenString;
>> }
>> if (bonusaktionenString) {
>> 	if (merkmaleString) {
>> 		merkmaleString += "\n"
>> 	}
>> 	merkmaleString += bonusaktionenString;
>> }
>> if (reaktionenString) {
>> 	if (merkmaleString) {
>> 		merkmaleString += "\n"
>> 	}
>> 	merkmaleString += reaktionenString;
>> }
>> if (passivString) {
>> 	if (merkmaleString) {
>> 		merkmaleString += "\n"
>> 	}
>> 	merkmaleString += passivString;
>> }
>> if (merkmaleString) {
>> 	merkmaleString = "### Merkmale\n" + merkmaleString;
>> 	dv.span(merkmaleString);
>> }
>> ```
>>
>> ``` dataviewjs
>> var legendäreAktionen = dv.current().Legendäre_Aktionen;
>> var anzahlLegendäreAktionen = dv.current().Anzahl_Legendäre_Aktionen;
>>
>> var legendäreAktionenString = "";
>> if (legendäreAktionen) {
>> for (var i = 0, j = legendäreAktionen.length; i<j; i++) {
>> 	legendäreAktionenString += "\n- "
>> 	legendäreAktionenString += legendäreAktionen[i];
>> }
>>
>> legendäreAktionenString = "### Legendäre Aktionen\n" + "Anzahl: " + anzahlLegendäreAktionen + "\n" + legendäreAktionenString;
>> dv.span(legendäreAktionenString);
>> }
>> ```
>
>> ## Angriff
>> ```dataview
>> TABLE WITHOUT ID 
>> file.link AS "Angriff",
>> Reichweite,
>> floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)+ceil(this.Herausforderungsgrad/4)+1 AS "Bonus",
>> (floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)) AS "Schaden",
>> Schadensarten,
>> Eigenschaften
>> FROM #Angriff
>> WHERE contains(this.Angriff.Waffen, file.link)
>> SORT file.name
>> ```