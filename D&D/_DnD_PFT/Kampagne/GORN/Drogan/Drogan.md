---
Stufe: 5
Bewegung: 7
Verteidigung:
  Natürliche_Rüstung: 10
  Zusätzliche_Rüstung: 0
  Rüstung: 
  Schild: 
Waffen:
  - "[[Zweihandaxt]]"
  - "[[Axt]]"
  - "[[Wurfspeer]]"
  - "[[Leichte Armbrust]]"
  - "[[Streitaxt]]"
Gesundheit:
  MaxTP: 59
  TP: 32
  TW: 5
  TempTP: 0
Attribute:
  Stärke: 18
  Geschicklichkeit: 14
  Konstitution: 16
  Intelligenz: 10
  Weisheit: 12
  Charisma: 8
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
  Nachforschungen: 1
  Naturkunde: 0
  Religion: 0
  Täuschen: 0
  Überlebenskunst: 0
  Überzeugen: 0
  Wahrnehmung: 1
Übung:
  Sprachen:
    - "[[Gemeinsprache]]"
    - "[[Zwergisch]]"
    - "[[Riesisch]]"
    - "[[Abyssisch]]"
  Werkzeuge:
    - "[[Brauereivorräte]]"
  Rüstungen:
    - "[[Leichte Rüstung]]"
    - "[[Mittelschwere Rüstung]]"
    - "[[Schilde]]"
  Waffen:
    - "[[Einfache Waffen]]"
    - "[[Kriegswaffen]]"
Aussehen:
  Geschlecht: männlich
  Alter: 115 Jahre
  Größenkategorie: "[[Mittelgroß]]"
  Größe: 140 cm
  Gewicht: 150 Pfund
  Augenfarbe: Blau
  Haarfarbe: Orange
  Hautfarbe: Sandfarben
Merkmale:
  - "[[Dunkelsicht]]"
  - "[[Unempfindlichkeit]]"
  - "[[Steingespür]]"
  - "[[Kampfrausch]]"
  - "[[Ungerüstete Verteidigung]]"
  - "[[Rücksichtsloser Angriff]]"
  - "[[Gefahrengespür]]"
  - "[[Titanengriff]]"
  - "[[Tödlicher Hieb]]"
  - "[[Furchtlos]]"
  - "[[Schnelle Bewegung]]"
  - "[[Zusätzlicher Angriff]]"
Talente:
  - "[[Meisterschaft Kampf mit zwei Waffen]]"
Hintergrund:
  Volk: "[[Zwerge#Gerbirgszwerge|Gebirgszwerg]]"
  Klasse: "[[Barbar]]"
  Subklasse: "[[Pfad des Slayers]]"
  Gesinnung: "[[Neutral Gut]]"
  Hintergrund: "[[Heimgesuchter]]"
Persönlichkeit:
  Persönlichkeitsmerkmale:
    - Ich fliehe nicht vor dem Bösen, das Böse flieht vor mir.
    - Ich spreche nicht über das, was mich quält.
    - Ich möchte andere nicht mit meinem Fluch belasten.
  Ideale: Ich versuche denjenigen zu helfen die Hilfe benötigen, egal was es mich kosten mag.
  Bindungen: Eine furchtbare Schuld verzehrt mich. Ich hoffe durch meine Taten Erlösung zu finden.
  Makel: Ich habe eine (Alkohol-)Sucht.
InputData:
  GlücksPunkt1: false
  GlücksPunkt2: false
  GlücksPunkt3: false
  GlücksPunkt4: false
  GlücksPunkt5: false
  ErschöpfungsPunkte: 0
  Erschöpfung1: false
  Erschöpfung2: false
  Erschöpfung3: false
  Erschöpfung4: false
  Erschöpfung5: false
  Erschöpfung6: false
  Erschöpfung7: false
  Erschöpfung8: false
  Erschöpfung9: false
  Rage1: false
  Rage2: false
  Rage3: false
tags:
  - Charakter/GORN
---
# `=this.file.name`

> [!infobox]
>  ![[Drogan.jpeg]]
> ```dynamic-embed
> [[embed Character Sheet Healthbar]]
> ```
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

> [!column | 3 no-title] 
>> ## Tracker
>> |                           | 
>> |:-------------------------:|
>> | `BUTTON[longBreakButton]` |
>> 
>> | Eigenschaft  |  1  |  2  |  3  |  4  |  5  |  6  |  7  |  8  |  9  |
>> | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
>> | [[Glück\|Glückspunkte]]  | `INPUT[toggle:InputData.GlücksPunkt1]` |  `INPUT[toggle:InputData.GlücksPunkt2]` | `INPUT[toggle:InputData.GlücksPunkt3]` | `INPUT[toggle:InputData.GlücksPunkt4]` | `INPUT[toggle:InputData.GlücksPunkt5]` |  -  |  -  |  -  |  -  |
>> | [[Erschöpft\|Erschöpfung]]       |  `INPUT[toggle:InputData.Erschöpfung1]`  | `INPUT[toggle:InputData.Erschöpfung2]` |  `INPUT[toggle:InputData.Erschöpfung3]`  |  `INPUT[toggle:InputData.Erschöpfung4]`  | `INPUT[toggle:InputData.Erschöpfung5]`  |  `INPUT[toggle:InputData.Erschöpfung6]`  |  `INPUT[toggle:InputData.Erschöpfung7]`  |  `INPUT[toggle:InputData.Erschöpfung8]`  |  `INPUT[toggle:InputData.Erschöpfung9]`  |
>
>> ## Klasse
>> |                                                                                                                              |                                                                                                    |
>> | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
>> | Nutzungen [[Kampfrausch]] (max. `$=dv.page(dv.current().Hintergrund.Klasse).Kampfrausch["Stufe"+dv.current().Stufe].Anzahl`) | `INPUT[toggle:InputData.Rage1]` `INPUT[toggle:InputData.Rage2]` `INPUT[toggle:InputData.Rage3]`    |
>> | Bonuschaden [[Kampfrausch]]                                                                                                  | +`$=dv.page(dv.current().Hintergrund.Klasse).Kampfrausch["Stufe"+dv.current().Stufe].Bonusschaden` |
>
>> ## Bewegung
>> ```dynamic-embed
>> [[embed Character Sheet Bewegung]]
>> ```

## Verteidigung
> [!column | no-title] 
>> ### Gesundheit
>> ```dynamic-embed
>> [[embed Character Sheet Gesundheit]]
>> ```
>
>> ### Rüstung
>> ```dynamic-embed
>> [[embed Character Sheet Rüstung]]
>> ```

## Angriff
> [!column | no-title]
>> ### Nahkampfwaffen
>> ```dynamic-embed
>> [[embed Character Sheet Waffen Nahkampf]]
>> ```
>
>> ### Schusswaffen 
>> ```dynamic-embed
>> [[embed Character Sheet Waffen Fernkampf]]
>> ```
>> 
>> ### Wurfwaffen
>> ```dynamic-embed
>> [[embed Character Sheet Waffen Wurf]]
>> ```

Disclaimer: Waffen haben immer Übungsbonus...

## Attribute und Fertigkeiten
> [!column  | 6 no-title]
>> ## Stärke
>> ```dynamic-embed
>> [[embed Character Sheet Attribute Stärke]]
>> ```
>
>> ## Geschicklichkeit
>> ```dynamic-embed
>> [[embed Character Sheet Attribute Geschicklichkeit]]
>> ```
>
>> ## Konstitution
>> ```dynamic-embed
>> [[embed Character Sheet Attribute Konstitution]]
>> ```
>
>> ## Intelligenz
>> ```dynamic-embed
>> [[embed Character Sheet Attribute Intelligenz]]
>> ```
>
>> ## Weisheit
>> ```dynamic-embed
>> [[embed Character Sheet Attribute Weisheit]]
>> ```
>
>> ## Charisma
>> ```dynamic-embed
>> [[embed Character Sheet Attribute Charisma]]
>> ```

## Übung

> [!column | 4 no-title]
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
>> OR #Liste/Waffen 
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
> [!column | 4 no-title]
>> ```dynamic-embed
>> [[embed Character Sheet Merkmale Aktionen]]
>> ```
>
>> ```dynamic-embed
>> [[embed Character Sheet Merkmale Bonusaktionen]]
>> ```
>
>> ```dynamic-embed
>> [[embed Character Sheet Merkmale  Reaktionen]]
>> ```
>
>> ```dynamic-embed
>> [[embed Character Sheet Merkmale Passiv]]
>> ```

## Hintergrundgeschichte
TBD

## Versteckte Logiken & Button Konfigurationen

```meta-bind-button
label: Lange Rast
icon: reset
hidden: true
class: ""
tooltip: ""
id: longBreakButton
style: primary
actions:
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const tw = mb.parseBindTarget('Gesundheit.TW', context.file.path); const stufe = mb.getMetadata(mb.parseBindTarget('Stufe', context.file.path)); mb.setMetadata(tw, stufe);"
  - type: updateMetadata
    bindTarget: InputData.Rage1
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.Rage2
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.Rage3
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.ErschöpfungsPunkte
    evaluate: true
    value: x - 1
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const TP = mb.parseBindTarget('Gesundheit.TP', context.file.path); const maxTP = mb.getMetadata(mb.parseBindTarget('Gesundheit.MaxTP', context.file.path));  mb.setMetadata(TP, maxTP);"
```

 
 ```js-engine
// Grab the Meta Bind API and extract metadata fields
const mb = engine.getPlugin('obsidian-meta-bind-plugin').api;

const ErschöpfungsPunkte = mb.parseBindTarget('InputData.ErschöpfungsPunkte', context.file.path);
const reactiveErschöpfungsPunkte = engine.reactive(onErschöpfungsPunkteChange, mb.getMetadata(ErschöpfungsPunkte)); 
setTimeout(() => {
	mb.subscribeToMetadata(ErschöpfungsPunkte, component, (value) => { reactiveErschöpfungsPunkte.refresh(value); }); 
}, 50);

const Erschöpfung1 = mb.parseBindTarget('InputData.Erschöpfung1', context.file.path);
const reactiveErschöpfung1 = engine.reactive(onChange1, mb.getMetadata(Erschöpfung1)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung1, component, (value) => { reactiveErschöpfung1.refresh(value); }); 
}, 50);

const Erschöpfung2 = mb.parseBindTarget('InputData.Erschöpfung2', context.file.path);
const reactiveErschöpfung2 = engine.reactive(onChange2, mb.getMetadata(Erschöpfung2)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung2, component, (value) => { reactiveErschöpfung2.refresh(value); }); 
}, 50);

const Erschöpfung3 = mb.parseBindTarget('InputData.Erschöpfung3', context.file.path);
const reactiveErschöpfung3 = engine.reactive(onChange3, mb.getMetadata(Erschöpfung3)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung3, component, (value) => { reactiveErschöpfung3.refresh(value); }); 
}, 50);

const Erschöpfung4 = mb.parseBindTarget('InputData.Erschöpfung4', context.file.path);
const reactiveErschöpfung4 = engine.reactive(onChange4, mb.getMetadata(Erschöpfung4)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung4, component, (value) => { reactiveErschöpfung4.refresh(value); }); 
}, 50);

const Erschöpfung5 = mb.parseBindTarget('InputData.Erschöpfung5', context.file.path);
const reactiveErschöpfung5 = engine.reactive(onChange5, mb.getMetadata(Erschöpfung5)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung5, component, (value) => { reactiveErschöpfung5.refresh(value); }); 
}, 50);

const Erschöpfung6 = mb.parseBindTarget('InputData.Erschöpfung6', context.file.path);
const reactiveErschöpfung6 = engine.reactive(onChange6, mb.getMetadata(Erschöpfung6)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung6, component, (value) => { reactiveErschöpfung6.refresh(value); }); 
}, 50);

const Erschöpfung7 = mb.parseBindTarget('InputData.Erschöpfung7', context.file.path);
const reactiveErschöpfung7 = engine.reactive(onChange7, mb.getMetadata(Erschöpfung7)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung7, component, (value) => { reactiveErschöpfung7.refresh(value); }); 
}, 50);

const Erschöpfung8 = mb.parseBindTarget('InputData.Erschöpfung8', context.file.path);
const reactiveErschöpfung8 = engine.reactive(onChange8, mb.getMetadata(Erschöpfung8)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung8, component, (value) => { reactiveErschöpfung8.refresh(value); }); 
}, 50);

const Erschöpfung9 = mb.parseBindTarget('InputData.Erschöpfung9', context.file.path);
const reactiveErschöpfung9 = engine.reactive(onChange9, mb.getMetadata(Erschöpfung9)); 
setTimeout(() => {
	mb.subscribeToMetadata(Erschöpfung9, component, (value) => { reactiveErschöpfung9.refresh(value); }); 
}, 50);

//events
function onErschöpfungsPunkteChange(value) {

	if( value < 0 ) {
		mb.setMetadata(ErschöpfungsPunkte, 0);
		return;
	}

	const metadataBind = {
		'Erschöpfung1': Erschöpfung1,
		'Erschöpfung2': Erschöpfung2,
		'Erschöpfung3': Erschöpfung3,
		'Erschöpfung4': Erschöpfung4,
		'Erschöpfung5': Erschöpfung5,
		'Erschöpfung6': Erschöpfung6,
		'Erschöpfung7': Erschöpfung7,
		'Erschöpfung8': Erschöpfung8,
		'Erschöpfung9': Erschöpfung9
	}

    const oldStates = [
        mb.getMetadata(Erschöpfung1),
        mb.getMetadata(Erschöpfung2),
        mb.getMetadata(Erschöpfung3),
        mb.getMetadata(Erschöpfung4),
        mb.getMetadata(Erschöpfung5),
        mb.getMetadata(Erschöpfung6),
        mb.getMetadata(Erschöpfung7),
        mb.getMetadata(Erschöpfung8),
        mb.getMetadata(Erschöpfung9)
    ];

    const newStates = Array(9).fill(false).map((_, index) => index < value);

    newStates.forEach((newState, index) => {
        if (oldStates[index] !== newState) {
            mb.setMetadata(metadataBind[`Erschöpfung${index + 1}`], newState);
        }
    });
}


function onChange1(value){
	onErschöpfungChange(1, value, Erschöpfung1);
}

function onChange2(value){
	onErschöpfungChange(2, value, Erschöpfung2);
}

function onChange3(value){
	onErschöpfungChange(3, value, Erschöpfung3);
}

function onChange4(value){
	onErschöpfungChange(4, value, Erschöpfung4);
}

function onChange5(value){
	onErschöpfungChange(5, value, Erschöpfung5);
}

function onChange6(value){
	onErschöpfungChange(6, value, Erschöpfung6);
}

function onChange7(value){
	onErschöpfungChange(7, value, Erschöpfung7);
}

function onChange8(value){
	onErschöpfungChange(8, value, Erschöpfung8);
}

function onChange9(value){
	onErschöpfungChange(9, value, Erschöpfung9);
}

function onErschöpfungChange(ErschöpfungsValue, newValue, metadataBind){	
	const currentPoints = mb.getMetadata(ErschöpfungsPunkte);
	const lowerValue = parseInt(ErschöpfungsValue-1);

	if(currentPoints == lowerValue && !newValue){
		return;
	} else if (currentPoints == lowerValue && newValue) {
		mb.setMetadata(ErschöpfungsPunkte, ErschöpfungsValue);
	} else if (currentPoints == ErschöpfungsValue && !newValue) {
		mb.setMetadata(ErschöpfungsPunkte, lowerValue);
	} else if (currentPoints > ErschöpfungsValue) {
		if(newValue == false) mb.setMetadata(metadataBind, true);
	} else if (currentPoints < ErschöpfungsValue) {
		if(newValue == true) mb.setMetadata(metadataBind, false);
	}
}

```
