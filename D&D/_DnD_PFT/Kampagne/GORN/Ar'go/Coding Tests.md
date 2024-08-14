---
cssclass: nord
Name: Ar'go
Stufe: 4
Bewegung: 6
Rüstung: 
Schild: 
Waffen:
  - "[[Kampfstab]]"
  - "[[Dolch]]"
Gesundheit:
  MaxTP: 33
  TP: 33
  TW: 4
  TempTP: 0
Attribute:
  Stärke: 8
  Geschicklichkeit: 13
  Konstitution: 16
  Intelligenz: 12
  Weisheit: 10
  Charisma: 18
Rettungswürfe:
  Stärke: 0
  Geschicklichkeit: 0
  Konstitution: 1
  Intelligenz: 0
  Weisheit: 0
  Charisma: 1
Fertigkeiten:
  Akrobatik: 0
  Arkane_Kunde: 1
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
  Naturkunde: 1
  Religion: 1
  Täuschen: 0
  Überlebenskunst: 0
  Überzeugen: 1
  Wahrnehmung: 0
Übung:
  Sprachen:
    - "[[Gemeinsprache]]"
    - "[[Urtümlich]]"
    - "[[Drakonisch]]"
    - "[[Celestisch]]"
  Werkzeuge:
    - "[[Navigationswerkzeug]]"
  Rüstungen: 
  Waffen:
    - "[[Dolch]]"
    - "[[Wurfmesser]]"
    - "[[Kampfstab]]"
    - "[[Leichte Armbrust]]"
Aussehen:
  Geschlecht: männlich
  Alter: 19 Jahre
  Größenkategorie: "[[Mittelgroß]]"
  Größe: 200 cm
  Gewicht: 120 Kilo
  Augenfarbe: Blau
  Haarfarbe: Dunkel Blau
  Hautfarbe: Blau
Merkmale:
  Volk:
    - "[[Odemwaffe]]"
    - "[[Drakonische Resistenz]]"
  Klasse:
    - "[[Quelle der Magie]]"
    - "[[Windsprecher]]"
    - "[[Stürmische Magie]]"
    - "[[Zauberwirken Zauberer]]"
  Talente:
    - "[[Kampferprobter Zauberwirker]]"
Hintergrund:
  Volk: "[[Drachenblütige|Drachenblütiger]]"
  Klasse: "[[Zauberer]]"
  Subklasse: "[[Sturmzauberei]]"
  Gesinnung: "[[Rechtschaffen Neutral]]"
  Hintergrund: "[[Einsiedler]]"
InputData:
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
random_number: 
---
## Statblocks

### Version 1

> [!statblocks]
> ![[Argo.jpeg|cover right circle htiny wtiny lp]]
> 
> # `=this.Name`
> > Description
> *Basics*
> *Basics*
> 
> ---
> ```dataviewjs 
> const Gesundheit = dv.current().Gesundheit; 
> const percentage = Math.round((Gesundheit.TP / Gesundheit.MaxTP) * 100);
> const metaBindCode = `<div style="display: flex; align-items: center; width: 100%; position: relative;">        <div style="width: 30px; text-align: center;">0</div>        <div style="flex: 1; position: relative;">            <progress id="health" max="${Gesundheit.MaxTP}" value="${Gesundheit.TP}" style="width: 100%; height: 20px; --progress: rgb(136, 192, 208) !important;"></progress>            <span id="percentage" style="position: absolute; left: 50%; top: 50%; transform: translate(-50%, -70%); color: white; font-weight: bold;">${percentage}%</span>        </div>        <div style="width: 30px; text-align: center;">${Gesundheit.MaxTP}</div>    </div>`; 
> dv.el('div', metaBindCode); 
> ```
| LP | RK | Initiative |
|:---:|:---:|:---:|
| `INPUT[number():Gesundheit.TP]` |  `=this.Rüstung` `=choice(this.Schild, ", ", "")` `=choice(this.Schild, this.Schild, "")`  | `=10+floor(((this.Attribute.Geschicklichkeit)-10)/2)+choice(this.Rüstung.RP, this.Rüstung.RP, 0)` + `=choice(this.Schild, this.Schild.RP, 0)`  | `=choice(this.Rüstung.SR, this.Rüstung.SR, 0)` + `=choice(this.Schild.SR, this.Schild.SR, 0)` |  `=floor(((this.Attribute.Geschicklichkeit)-10)/2)` |
>
> 
| [[Attribute\|Attribut]] |           Wert            |        Mod.         |                                            RW-Mod.                                       |
| ----------------------- |:----------------------------------:|:--------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------:|
| [[Stärke]]              |      `=this.Attribute.Stärke`      |      `=floor(((this.Attribute.Stärke)-10)/2)`      |           `=floor(((this.Attribute.Stärke)-10)/2)+(this.Rettungswürfe.Stärke*(ceil(this.Stufe/4)+1))`           |
| [[Geschicklichkeit]]    | `=this.Attribute.Geschicklichkeit` | `=min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)` | `=min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)+(this.Rettungswürfe.Geschicklichkeit*(ceil(this.Stufe/4)+1))` |
| [[Konstitution]]        |   `=this.Attribute.Konstitution`   |   `=floor(((this.Attribute.Konstitution)-10)/2)`   |     `=floor(((this.Attribute.Konstitution)-10)/2)+(this.Rettungswürfe.Konstitution*(ceil(this.Stufe/4)+1))`     |
| [[Intelligenz]]         |   `=this.Attribute.Intelligenz`    |   `=floor(((this.Attribute.Intelligenz)-10)/2)`    |      `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Rettungswürfe.Intelligenz*(ceil(this.Stufe/4)+1))`      |
| [[Weisheit]]            |     `=this.Attribute.Weisheit`     |     `=floor(((this.Attribute.Weisheit)-10)/2)`     |         `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Rettungswürfe.Weisheit*(ceil(this.Stufe/4)+1))`         |
| [[Charisma]]            |     `=this.Attribute.Charisma`     |     `=floor(((this.Attribute.Charisma)-10)/2)`     |         `=floor(((this.Attribute.Charisma)-10)/2)+(this.Rettungswürfe.Charisma*(ceil(this.Stufe/4)+1))`         |
> 
|  |  |
| ---:|:--- |
| **Bewegung** | 9 Meter |
| **Passive Wahrnehmung (WIS)** | `=10+floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Wahrnehmung*(ceil(this.Stufe/4)+1))`   |
| **Übungsbonus** | `=ceil(this.Stufe/4)+1`|
| **Dunkelsicht** |  Nein |
>
> ---
>> [!checks|no-t] 
>> - **Death Saves**
>>	- ❌
>>	- [ ] 
>>	- [ ] 
>>	- [ ] 
>>	- ✔
>>	- [ ] 
>>	- [ ] 
>>	- [ ] 
>
> ###### Traits
| | |
| --- | --- |
| **Class** | |
| **.** | |
| **Racial Traits** | |
| **Feats** | |

### Version 2

> [!statblocks|columns]
> 
>> [!blank]  
>> ![Char Image|right cover htiny wtiny circle lp]()
>> # Name
>> > Description
>> 
>> *Basics*
>> 
>> ---
| HP | AC | Initiative |
|:---:|:---:|:---:|
| | | |
>>
| STR | DEX | CON | INT | WIS | CHA |  |
|:---:|:---:|:---:|:---:|:---:|:---:|:--- |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  | **Mod** |
|  |  |  |  |  |  | **Sav** |
>>
|  |  |
| ---:|:--- |
| **Speed** |  |
| **Passive Perception (WIS)** |  |
| **Proficiency Bonus** |  |
| **Darkvision** |  |
>> 
>> ---
>> 
>>> [!checks|no-t] 
>>> - 
>>>	- **Spell Slots**
>>>	- [ ] 
>>>	- [ ] 
>>> - **Death Saves**
>>>	- ❌
>>>	- [ ] 
>>>	- [ ] 
>>>	- [ ] 
>>>	- ✔
>>>	- [ ] 
>>>	- [ ] 
>>>	- [ ] 
>> 
> 
> 
>> [!blank]
>> ## Traits
| | |
| --- | --- |
>> 
>> ## Feats
>> 
>> **Feat**
>> Description
>> 
>> **Feat**
>> Description

##  Dice Plugin

`dice: 1d6`
 
```js-engine

// Roll a 1d6 die using the Dice Roller plugin
//const diceRoll = await engine.getPlugin['obsidian-dice-roller'];

// Update the front matter metadata with the dice roll result
/*const currentFile = app.workspace.getActiveFile();
const metadata = app.metadataCache.getFileCache(currentFile)?.frontmatter || {};

// Merge the new metadata
metadata.random_number = diceRoll.result;

// Write the updated metadata back to the file
await app.vault.modify(
    currentFile, 
    `---
random_number: ${metadata.random_number}
---\n\n` + app.vault.read(currentFile)
);*/

```


## Erschöpfungspunkte Logik

`INPUT[number:InputData.ErschöpfungsPunkte]`

Erschöpfungspunkte: `=this.InputData.ErschöpfungsPunkte`

```meta-bind-button
label: Lange Rast
icon: reset
hidden: false
class: ""
tooltip: ""
id: ""
style: primary
actions:
  - type: updateMetadata
    bindTarget: InputData.ErschöpfungsPunkte
    evaluate: true
    value: x - 1

```


|        Eigenschaft         |                   1                    |                   2                    |                   3                    |                   4                    |                   5                    |                   6                    |                   7                    |                   8                    |                   9                    |
|:--------------------------:|:--------------------------------------:|:--------------------------------------:|:--------------------------------------:|:--------------------------------------:|:--------------------------------------:|:--------------------------------------:|:--------------------------------------:|:--------------------------------------:|:--------------------------------------:|
| [[Erschöpft\|Erschöpfung]] | `INPUT[toggle:InputData.Erschöpfung1]` | `INPUT[toggle:InputData.Erschöpfung2]` | `INPUT[toggle:InputData.Erschöpfung3]` | `INPUT[toggle:InputData.Erschöpfung4]` | `INPUT[toggle:InputData.Erschöpfung5]` | `INPUT[toggle:InputData.Erschöpfung6]` | `INPUT[toggle:InputData.Erschöpfung7]` | `INPUT[toggle:InputData.Erschöpfung8]` | `INPUT[toggle:InputData.Erschöpfung9]` |


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

