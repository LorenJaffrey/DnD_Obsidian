---
cssclass: nord
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
## Beispiele


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

