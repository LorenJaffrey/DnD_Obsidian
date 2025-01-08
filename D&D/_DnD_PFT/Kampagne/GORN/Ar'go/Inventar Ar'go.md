---
Name: Inventar
Charakter: "[[Ar'go]]"
cssclass: slrvb-b, dvl-o, hc, h-line, table, k-o, t-c, t-w, tbl-nalt, tag-notion, tag-bubble, tag-outline, tag-text
Summen:
  Rucksack: 53.1
  Behälter: 0
  Körper: 11.6
Inventar:
  Körper:
    count1: 2
    gewicht1: 1
    count2: 1
    gewicht2: 4
    count3: 1
    gewicht3: 1
    count4: 1
    gewicht4: 3
    count5: 1
    gewicht5: 0
    count6: 1
    gewicht6: 1
    count7: 12
    gewicht7: 0.05
    count8: 1
    gewicht8: 0
    count9: 0
    gewicht9: 0
    count10: 0
    gewicht10: 0
    count11: 0
    gewicht11: 0
    count12: 0
    gewicht12: 0
    count13: 0
    gewicht13: 0
    count14: 0
    gewicht14: 0
    count15: 0
    gewicht15: 0
  Behälter:
    count1: 1
    gewicht1: 0
    count2: 0
    gewicht2: 0
    count3: 0
    gewicht3: 0
    count4: 0
    gewicht4: 0
    count5: 0
    gewicht5: 0
    count6: 0
    gewicht6: 0
    count7: 0
    gewicht7: 0
    count8: 0
    gewicht8: 0
    count9: 0
    gewicht9: 0
    count10: 0
    gewicht10: 0
    count11: 0
    gewicht11: 0
    count12: 0
    gewicht12: 0
    count13: 0
    gewicht13: 0
    count14: 0
    gewicht14: 0
    count15: 0
    gewicht15: 0
  Rucksack:
    count1: 1
    gewicht1: 5
    count2: 1
    gewicht2: 3
    count3: 10
    gewicht3: 0.25
    count4: 9
    gewicht4: 1
    count5: 1
    gewicht5: 1
    count6: 22
    gewicht6: 1
    count7: 1
    gewicht7: 0
    count8: 15
    gewicht8: 0.6
    count9: 1
    gewicht9: 0.6
    count10: 1
    gewicht10: 0
    count11: 1
    gewicht11: 0.5
    count12: 1
    gewicht12: 0
    count13: 50
    gewicht13: 0.01
    count14: 0
    gewicht14: 0
    count15: 0
    gewicht15: 0
    count16: 0
    gewicht16: 0
    count17: 0
    gewicht17: 0
Geld:
  PM: 0
  GM: 35
  EM: 0
  SM: 8
  KM: 23
---

# `=this.Name`
> [!infobox]
> ###### Geld
> | Währung | Anzahl |
> | ---- | ---- |
> | PM (10 GM)| `INPUT[number:Geld.PM]` |
> | GM  (10 SM)| `INPUT[number:Geld.GM]`  |
> | EM  (5 SM) | `INPUT[number:Geld.EM]`  |
> | SM (10 KM) | `INPUT[number:Geld.SM]`  |
> | KM | `INPUT[number:Geld.KM]` |
> 
> ##### Last
> | Type | Stat |
> | ---- | ---- |
> | Belastet | `=(this.Charakter.Attribute.Stärke*5)+1` - `=(this.Charakter.Attribute.Stärke*10)` Pfund |
> | Stark Belastet | `=(this.Charakter.Attribute.Stärke*10)+1` - `=(this.Charakter.Attribute.Stärke*15)` Pfund |
> | Maximale Traglast | `=(this.Charakter.Attribute.Stärke*15)` Pfund |
> | Maximalbelastung | `=(this.Charakter.Attribute.Stärke*30)` Pfund |
> 
> ##### Aktuelle Traglast: `=round(this.Summen.Rucksack+this.Summen.Behälter+this.Summen.Körper, 2)`

> [!column | 3 flex no-title]
>> ## Am Körper
>> | Gegenstand                                  |                 Anzahl                 |                 Gewicht                  |                             Gesamt                             |
>> | ------------------------------------------- |:--------------------------------------:|:----------------------------------------:|:--------------------------------------------------------------:|
>> | [[Dolch]]                                   | `INPUT[number:Inventar.Körper.count1]` | `INPUT[number:Inventar.Körper.gewicht1]` | `=round(this.Inventar.Körper.count1 * this.Inventar.Körper.gewicht1, 2)` |
>> | [[Kampfstab]]                               | `INPUT[number:Inventar.Körper.count2]` | `INPUT[number:Inventar.Körper.gewicht2]` | `=round(this.Inventar.Körper.count2 * this.Inventar.Körper.gewicht2, 2)` |
>> | [[Arkaner Fokus]] - Kristall                | `INPUT[number:Inventar.Körper.count3]` | `INPUT[number:Inventar.Körper.gewicht3]` | `=round(this.Inventar.Körper.count3 * this.Inventar.Körper.gewicht3, 2)` |
>> | Gewöhnliche Kleidung                        | `INPUT[number:Inventar.Körper.count4]` | `INPUT[number:Inventar.Körper.gewicht4]` | `=round(this.Inventar.Körper.count4 * this.Inventar.Körper.gewicht4, 2)` |
>> | Kultisten-Amulett <br/>(Symbol des Sturmdrachen) | `INPUT[number:Inventar.Körper.count5]` | `INPUT[number:Inventar.Körper.gewicht5]` | `=round(this.Inventar.Körper.count5 * this.Inventar.Körper.gewicht5, 2)` |
>> | [[Leichte Armbrust]]                        | `INPUT[number:Inventar.Körper.count6]` | `INPUT[number:Inventar.Körper.gewicht6]` | `=round(this.Inventar.Körper.count6 * this.Inventar.Körper.gewicht6, 2)` |
>> | Köcher mit Bolzen                           | `INPUT[number:Inventar.Körper.count7]` | `INPUT[number:Inventar.Körper.gewicht7]` | `=round(this.Inventar.Körper.count7 * this.Inventar.Körper.gewicht7, 2)` |
>> |            Tagebuch des Akolythen   / Ritual Dolch des Talos            | `INPUT[number:Inventar.Körper.count8]` | `INPUT[number:Inventar.Körper.gewicht8]` | `=round(this.Inventar.Körper.count8 * this.Inventar.Körper.gewicht8, 2)` |
>> |                                                                    | `INPUT[number:Inventar.Körper.count9]` | `INPUT[number:Inventar.Körper.gewicht9]` | `=round(this.Inventar.Körper.count9 * this.Inventar.Körper.gewicht9, 2)` |
>> |                                                                    | `INPUT[number:Inventar.Körper.count10]` | `INPUT[number:Inventar.Körper.gewicht10]` | `=round(this.Inventar.Körper.count10 * this.Inventar.Körper.gewicht10, 2)` |
>> |                                                                    | `INPUT[number:Inventar.Körper.count11]` | `INPUT[number:Inventar.Körper.gewicht11]` | `=round(this.Inventar.Körper.count11 * this.Inventar.Körper.gewicht11, 2)` |
>> | **GESAMT**                                  |                                        |                                          |                     `=this.Summen.Körper`                      |
>
>> ## Schriftrollenbehälter
>> | Gegenstand                                                |                  Anzahl                  |                  Gewicht                   |                               Gesamt                               |
>> | --------------------------------------------------------- |:----------------------------------------:|:------------------------------------------:|:------------------------------------------------------------------:|
>> | Karte der Insel (Drachenkult) <br/>und der umliegenden Gebiete | `INPUT[number:Inventar.Behälter.count1]` | `INPUT[number:Inventar.Behälter.gewicht1]` | `=round(this.Inventar.Behälter.count1 * this.Inventar.Behälter.gewicht1, 2)` |
>> |                                                                             | `INPUT[number:Inventar.Behälter.count2]` | `INPUT[number:Inventar.Behälter.gewicht2]` | `=round(this.Inventar.Behälter.count2 * this.Inventar.Behälter.gewicht2, 2)` |
>> |                                                                             | `INPUT[number:Inventar.Behälter.count3]` | `INPUT[number:Inventar.Behälter.gewicht3]` | `=round(this.Inventar.Behälter.count3 * this.Inventar.Behälter.gewicht3, 2)` |
>> |                                                                             | `INPUT[number:Inventar.Behälter.count4]` | `INPUT[number:Inventar.Behälter.gewicht4]` | `=round(this.Inventar.Behälter.count4 * this.Inventar.Behälter.gewicht4, 2)` |
>> |                                                                             | `INPUT[number:Inventar.Behälter.count5]` | `INPUT[number:Inventar.Behälter.gewicht5]` | `=round(this.Inventar.Behälter.count5 * this.Inventar.Behälter.gewicht5, 2)` |
>> | **GESAMT**                                                |                                          |                                            |                      `=this.Summen.Behälter`                       | 
>
>> ## Rucksack
>> | Gegenstand                                |                  Anzahl                   |                   Gewicht                   |                                Gesamt                                |
>> | ----------------------------------------- |:-----------------------------------------:|:-------------------------------------------:|:--------------------------------------------------------------------:|
>> | [[Brechstange]]                           | `INPUT[number:Inventar.Rucksack.count1]`  | `INPUT[number:Inventar.Rucksack.gewicht1]`  |  `=round(this.Inventar.Rucksack.count1 * this.Inventar.Rucksack.gewicht1, 2)`  |
>> | [[Hammer]]                                | `INPUT[number:Inventar.Rucksack.count2]`  | `INPUT[number:Inventar.Rucksack.gewicht2]`  |  `=round(this.Inventar.Rucksack.count2 * this.Inventar.Rucksack.gewicht2, 2)`  |
>> | [[Kletterhaken]]                          | `INPUT[number:Inventar.Rucksack.count3]`  | `INPUT[number:Inventar.Rucksack.gewicht3]`  |  `=round(this.Inventar.Rucksack.count3 * this.Inventar.Rucksack.gewicht3, 2)`  |
>> | [[Fackel]]                                | `INPUT[number:Inventar.Rucksack.count4]`  | `INPUT[number:Inventar.Rucksack.gewicht4]`  |  `=round(this.Inventar.Rucksack.count4 * this.Inventar.Rucksack.gewicht4, 2)`  |
>> | [[Zunderkästchen]]                        | `INPUT[number:Inventar.Rucksack.count5]`  | `INPUT[number:Inventar.Rucksack.gewicht5]`  |  `=round(this.Inventar.Rucksack.count5 * this.Inventar.Rucksack.gewicht5, 2)`  |
>> | [[Ration]]                                | `INPUT[number:Inventar.Rucksack.count6]`  | `INPUT[number:Inventar.Rucksack.gewicht6]`  |  `=round(this.Inventar.Rucksack.count6 * this.Inventar.Rucksack.gewicht6, 2)`  |
>> | [[Trinkschlauch]]                         | `INPUT[number:Inventar.Rucksack.count7]`  | `INPUT[number:Inventar.Rucksack.gewicht7]`  |  `=round(this.Inventar.Rucksack.count7 * this.Inventar.Rucksack.gewicht7, 2)`  |
>> | [[Seil aus Hanf]]  (Meter)                | `INPUT[number:Inventar.Rucksack.count8]`  | `INPUT[number:Inventar.Rucksack.gewicht8]`  |  `=round(this.Inventar.Rucksack.count8 * this.Inventar.Rucksack.gewicht8, 2)`  |
>> | Kompass                                   | `INPUT[number:Inventar.Rucksack.count9]`  | `INPUT[number:Inventar.Rucksack.gewicht9]`  |  `=round(this.Inventar.Rucksack.count9 * this.Inventar.Rucksack.gewicht9, 2)`  |
>> | Winterdecke                               | `INPUT[number:Inventar.Rucksack.count10]` | `INPUT[number:Inventar.Rucksack.gewicht10]` | `=round(this.Inventar.Rucksack.count10 * this.Inventar.Rucksack.gewicht10, 2)` |
>> | Ritualbuch <br/>(Drachenkult des Sturmdrachen) | `INPUT[number:Inventar.Rucksack.count11]` | `INPUT[number:Inventar.Rucksack.gewicht11]` | `=round(this.Inventar.Rucksack.count11 * this.Inventar.Rucksack.gewicht11, 2)` |
>> | [[Gildenabzeichen]]                       | `INPUT[number:Inventar.Rucksack.count12]` | `INPUT[number:Inventar.Rucksack.gewicht12]` | `=round(this.Inventar.Rucksack.count12 * this.Inventar.Rucksack.gewicht12, 2)` |
>> | Spule Draht (Meter)                       | `INPUT[number:Inventar.Rucksack.count13]` | `INPUT[number:Inventar.Rucksack.gewicht13]` | `=round(this.Inventar.Rucksack.count13 * this.Inventar.Rucksack.gewicht13, 2)` |
>> |                                                                   | `INPUT[number:Inventar.Rucksack.count14]` | `INPUT[number:Inventar.Rucksack.gewicht14]` | `=round(this.Inventar.Rucksack.count14 * this.Inventar.Rucksack.gewicht14, 2)` |
>> |                                                                   | `INPUT[number:Inventar.Rucksack.count15]` | `INPUT[number:Inventar.Rucksack.gewicht15]` | `=round(this.Inventar.Rucksack.count15 * this.Inventar.Rucksack.gewicht15, 2)` |
>> |                                                                   | `INPUT[number:Inventar.Rucksack.count16]` | `INPUT[number:Inventar.Rucksack.gewicht16]` | `=round(this.Inventar.Rucksack.count16 * this.Inventar.Rucksack.gewicht16, 2)` |
>> |                                                                   | `INPUT[number:Inventar.Rucksack.count17]` | `INPUT[number:Inventar.Rucksack.gewicht17]` | `=round(this.Inventar.Rucksack.count17 * this.Inventar.Rucksack.gewicht17, 2)` |
>> | **GESAMT**                                |                                           |                                             |                       `=this.Summen.Rucksack`                        |


```js-engine
const mb = engine.getPlugin('obsidian-meta-bind-plugin').api;
const groupList = ['Rucksack', 'Behälter', 'Körper'];
const valueList = ['count', 'gewicht'];

groupList.forEach((groupName) => {
	const sumBinding = mb.parseBindTarget(`Summen.${groupName}`, context.file.path);
	const metaDataList = context.metadata.frontmatter.Inventar[groupName];
	const metaDataCount = Object.keys(metaDataList).length / (valueList.length)
	let sumValue = 0;

	for(let i = 0; i < metaDataCount; i++){
		const countValue = mb.getMetadata(mb.parseBindTarget(`Inventar.${groupName}.count${i+1}`, context.file.path));
		const gewichtValue = mb.getMetadata(mb.parseBindTarget(`Inventar.${groupName}.gewicht${i+1}`, context.file.path));
		sumValue += (countValue * gewichtValue)
	}

	mb.setMetadata(sumBinding, sumValue);
});

```

```js-engine
if(document.head) {
	const style = document.createElement('style');
	style.type = 'text/css';
	
	style.innerHTML = `
		.callout-content {
			justify-content: Center;
		}
	`;
	
	document.head.appendChild(style);
}
```