---
tags:
  - Kreatur
aliases: 
Größenkategorie: "[[Mittelgroß]]"
Typ: "[[Humanoide]]"
Subtyp: "[[Menschen|Mensch]]"
Gesinnung: "[[Neutral Gut]]"
Geschlecht: männlich
Alter:
Beruf: Jäger
Fraktion:
Herausforderungsgrad: 4
Stufe: 15
Trefferwürfel: d8
Bewegung:
  Boden: 9
  Fliegen:
  Schwimmen:
  Klettern:
  Graben:
Sinne:
Verteidigung:
  Rüstung: "[[Beschlagene Lederrüstung]]"
  Schild:
  Natürliche_Rüstung: 10
  Natürliche_SR: 0
  Resistenzen:
    Schadensresistenz:
    Schadensimmunität: 
    Zustandsimmunität:
Angriff:
  Waffen:
    - "[[Langbogen]]"
    - "[[Langschwert]]"
  Angriffe:
Attribute:
  Stärke: 14
  Geschicklichkeit: 15
  Konstitution: 16
  Intelligenz: 11
  Weisheit: 16
  Charisma: 15
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
  Athletik: 1
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
  Überlebenskunst: 1
  Überzeugen: 0
  Wahrnehmung: 1
Sprachen:
  - "[[Gemeinsprache]]"
Merkmale:

Anzahl_Legendäre_Aktionen:
Legendäre_Aktionen:
---
# `=this.file.name`
> [!column | 2 flex | no-title]
>> ![[falcon_the_hunter.webp | 350]]
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
>> | Geschlecht | `=this.Geschlecht` |
>> | Alter      | `=this.Alter`      |
>> | Funktion      | `=this.Beruf`      |
>> | Fraktion/en   | `=this.Fraktion`   |
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
>> [[Trefferpunkte]]: `$="```dice:" + dv.current().Stufe + dv.current().Trefferwürfel + "+" + dv.current().Stufe*Math.floor((dv.current().Attribute.Konstitution-10)/2) + "|none|noform```"`
>>
>> |                |                                                                                                                                                 |
>> | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
>> | Rüstung               | `=this.Verteidigung.Rüstung` `=choice(this.Verteidigung.Schild, ", ", "")` `=choice(this.Verteidigung.Schild, this.Verteidigung.Schild, "")`                                                                           |
>> | [[Rüstungsklasse]]    | `=this.Verteidigung.Natürliche_Rüstung+floor(((this.Attribute.Geschicklichkeit)-10)/2)+choice(this.Verteidigung.Rüstung.RP, this.Verteidigung.Rüstung.RP, 0)` + `=choice(this.Verteidigung.Schild, this.Verteidigung.Schild.RP, 0)` |
>> | [[Schadensreduktion]] | `=this.Verteidigung.Natürliche_SR+choice(this.Verteidigung.Rüstung.SR, this.Verteidigung.Rüstung.SR, 0)` + `=choice(this.Verteidigung.Schild.SR, this.Verteidigung.Schild.SR, 0)`       
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

## Aussehen
[[Falke der Jäger]]  trägt eine [[beschlagene Lederrüstung]] und darüber einen pelzgefütterten Umhang. 
Er ist knapp zwei Meter groß, hat schwarzes Haar und breite Schultern. 
Er trägt einen gepflegten Bart. 
Seine scharfen Augen sind blau und kalt wie Eis. 
Falke bewegt sich mit der Sicherheit dessen, der nichts fürchtet, und begegnet allen Problemen mit verblüffender Gleichgültigkeit. 

## Persönlichkeit
Er liebt guten Wein und behandelt andere, wie er selbst behandelt werden will: aufrichtig und geduldig.

## Eigenarten

## Ziele
Wenn die Charaktere die Quest „Das alte Haus im Wald" schon in Angriff nehmen dürfen, bietet Falke ihnen ein Paar Stiefel der Elfen als Belohnung an. 
Falke lehnt es höflich, aber bestimmt ab, die Charaktere auf einer Quest zu begleiten, da er sich im Jagdhaus aufhalten muss, falls Adlige aus Niewinter kommen.

## Beschreibung
Falkes echter Name ist Gustaf Stellern, aber er hat ihn schon lange abgelegt. 
Seine Jagdkünste haben ihm seinen heutigen Namen eingebracht. 
Wenn er die Gelegenheit bekommt, teilt er den Charakteren folgende nützliche Informationen mit:

- "Ich sehe immer mehr Orks in den Wäldern. 
   Hässliche Bastarde."
- ﻿﻿"Die Orks scheinen sich mit den bösen Halborks verbündet zu haben, die südöstlich von hier hausen. 
   Diese Halborks sind häufig mit kleinen Waldkreaturen unterwegs, die wie Stöcke aussehen.
   Grässliche  Biester allesamt."
- "Die Halborks hausen in einem verfallenen, überwucherten Steinbau etwa zehn Meilen von hier. 
   Das Haus wurde angeblich von einem Gelehrten errichtet, der die Elfenruinen in diesen Wäldern studiert hat."