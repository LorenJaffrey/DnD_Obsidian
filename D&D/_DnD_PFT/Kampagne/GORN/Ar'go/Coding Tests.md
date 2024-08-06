---
valueA: 1
valueB: true
valueC: false
---

```js-engine
// Grab the Meta Bind API and extract metadata fields
const mb = engine.getPlugin('obsidian-meta-bind-plugin').api;
const valueA = mb.parseBindTarget('valueA', context.file.path);
const valueB = mb.parseBindTarget('valueB', context.file.path);
const valueC = mb.parseBindTarget('valueC', context.file.path);

function updateValueBIfNeeded(newValueA) {
	switch(newValueA) {
		case 0:
		mb.setMetadata(valueB, false);
        mb.setMetadata(valueC, false);
		break;
		case 1:
		mb.setMetadata(valueB, true);
        mb.setMetadata(valueC, false);
		break;
		case 2:
		mb.setMetadata(valueB, true);
        mb.setMetadata(valueC, true);
		break;
	}
}

function onUpdate(value) {
    // Handle the update
    updateValueBIfNeeded(value);
}

// Set up reactive subscriptions
const reactiveA = engine.reactive(onUpdate, mb.getMetadata(valueA)); 
const reactiveB = engine.reactive(() => {}, mb.getMetadata(valueB)); 
const reactiveC = engine.reactive(() => {}, mb.getMetadata(valueC));

// Subscribe to changes in valueA 
mb.subscribeToMetadata(valueA, component, (value) => { reactiveA.refresh(value); }); 

// Subscribe to changes in valueB 
mb.subscribeToMetadata(valueB, component, (value) => { reactiveB.refresh(value); }); 

// Subscribe to changes in valueC 
mb.subscribeToMetadata(valueC, component, (value) => { reactiveC.refresh(value); });

return { reactiveA, reactiveB, reactiveC };
```


`=this.valueA`
`=this.valueB`
`=this.valueC`

`INPUT[toggle:valueB]`
`INPUT[toggle:valueC]`

`INPUT[number:valueA]`