---
cssclass: dnd
Stufe: 5
Bewegung: 6
Verteidigung:
  Natürliche_Rüstung: 10
  Zusätzliche_Rüstung: 1
  Zusätzliche_SR: 1
  Rüstung: "[[Fellrüstung]]"
  Schild: "[[Holzschild]]"
Waffen:
  - "[[Stab des Sommerwalds]]"
  - "[[Krummsäbel]]"
  - "[[Schleuder]]"
Gesundheit:
  MaxTP: 38
  TP: 38
  TW: 5
  TempTP: 0
Attribute:
  Stärke: 8
  Geschicklichkeit: 14
  Konstitution: 14
  Intelligenz: 12
  Weisheit: 19
  Charisma: 11
Rettungswürfe:
  Stärke: 0
  Geschicklichkeit: 0
  Konstitution: 0
  Intelligenz: 1
  Weisheit: 1
  Charisma: 0
Fertigkeiten:
  Akrobatik: 0
  Arkane_Kunde: 1
  Athletik: 0
  Auftreten: 0
  Einschüchtern: 0
  Fingerfertigkeit: 0
  Geschichte: 0
  Heilkunde: 1
  Heimlichkeit: 0
  Mit_Tieren_umgehen: 1
  Motiv_erkennen: 0
  Nachforschungen: 0
  Naturkunde: 1
  Religion: 1
  Täuschen: 0
  Überlebenskunst: 1
  Überzeugen: 0
  Wahrnehmung: 0
Übung:
  Sprachen:
    - "[[Gemeinsprache]]"
    - "[[Elfisch]]"
    - "[[Sylvanisch]]"
    - "[[Urtümlich]]"
    - "[[Druidisch]]"
  Werkzeuge:
    - "[[Kräuterkunde-Ausrüstung]]"
    - "[[Giftmischerausrüstung]]"
  Rüstungen:
    - "[[Leichte Rüstung]]"
    - "[[Mittelschwere Rüstung]]"
  Waffen:
    - "[[Knüppel]]"
    - "[[Dolch]]"
    - "[[Wurfmesser]]"
    - "[[Wurfspeer]]"
    - "[[Streitkolben]]"
    - "[[Kampfstab]]"
    - "[[Krummsäbel]]"
    - "[[Sichel]]"
    - "[[Schleuder]]"
    - "[[Speer]]"
Aussehen:
  Geschlecht: männlich
  Alter: 45 Jahre
  Größenkategorie: "[[Mittelgroß]]"
  Größe: 180 cm
  Gewicht: 150 Pfund
  Augenfarbe: Grau
  Haarfarbe: Dunkelbraun
  Hautfarbe: Sandfarben
Merkmale:
  - "[[Dunkelsicht]]"
  - "[[Feenblut]]"
  - "[[Die Sprache des Waldes]]"
  - "[[Druidisch]]"
  - "[[Verbesserte Tiergestalt]]"
  - "[[Geistertotem]]"
  - "[[Druidisches Zauberwirken]]"
  - "[[Tiergestalt]]"
Talente:
  - "[[Von Feen berührt]]"
Hintergrund:
  Name: Aranon Grauwald
  Volk: "[[Halbelfen|Halbelf]]"
  Klasse: "[[Druide]]"
  Subklasse: "[[Zirkel des Hirten]]"
  Gesinnung: "[[Rechtschaffen Gut]]"
  Hintergrund: "[[Einsiedler]]"
Persönlichkeit:
  Persönlichkeitsmerkmale:
    - Große Empathie für alle jene die großes Leid erfahren
    - Erlangt durch Meditation innere Ruhe und Frieden
    - Gesellig und trinkfest
  Ideale: Alles Böse zu vernichten!
  Bindungen: Rache für den ausgelöschten Stamm.
  Makel:
    - Visionen, Alpträume und unkontrollierte Teleportation
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
  - "[[Tiere beschwören]]"
  - "[[Mit Pflanzen sprechen]]"
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
  TiergestaltLadung1: false
  TiergestaltLadung2: false
  GeistertotemLadung: false
  NebelschrittLadung: false
  IdentifizierenLadung: false
  Stresslevel1: false
  Stresslevel2: false
  Stresslevel3: false
  Stresslevel4: false
  Stresslevel5: false
  Zauberplätze:
    Grad_1: 4
    Grad_2: 3
    Grad_3: 2
    Grad_4: 0
    Grad_5: 0
    Grad_6: 0
    Grad_7: 0
    Grad_8: 0
    Grad_9: 0
tags:
  - Charakter/GORN
---
# `=this.Hintergrund.Name`
> [!infobox]
> ## `=this.Hintergrund.Name`
> ![[Aranon.jpg]]
> ```dynamic-embed
> [[embed Character Sheet Healthbar]]
> ```
> 
> ```dataviewjs 
> const maxGrad1 = dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad1;
> const maxGrad2 = dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad2;
> const maxGrad3 = dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad3;
> const maxGrad4 = dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad4;
> const maxGrad5 = dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad5;
> const maxGrad6 = dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad6;
> const maxGrad7 = dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad7;
> const maxGrad8 = dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad8;
> const maxGrad9 = dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad9;
> 
> const maxSpellSlots =  (maxGrad1*1)+(maxGrad2*4)+(maxGrad3*9)+(maxGrad4*16)+(maxGrad5*25)+(maxGrad6*36)+(maxGrad7*49)+(maxGrad8*64)+(maxGrad9*81);
>  
> const grad1 = dv.current().InputData.Zauberplätze.Grad_1;
> const grad2 = dv.current().InputData.Zauberplätze.Grad_2;
> const grad3 = dv.current().InputData.Zauberplätze.Grad_3;
> const grad4 = dv.current().InputData.Zauberplätze.Grad_4;
> const grad5 = dv.current().InputData.Zauberplätze.Grad_5;
> const grad6 = dv.current().InputData.Zauberplätze.Grad_6;
> const grad7 = dv.current().InputData.Zauberplätze.Grad_7;
> const grad8 = dv.current().InputData.Zauberplätze.Grad_8;
> const grad9 = dv.current().InputData.Zauberplätze.Grad_9;
>  
> const currentSpellSlots = (grad1*1)+(grad2*4)+(grad3*9)+(grad4*16)+(grad5*25)+(grad6*36)+(grad7*49)+(grad8*64)+(grad9*81);
> const percentValue = Math.round(currentSpellSlots / (maxSpellSlots / 100));
> 
> const metaBindCode = `<div style="display: flex; align-items: center; width: 100%; position: relative;"><div style="flex: 1; position: relative;"><progress id="magic" max="${maxSpellSlots}" value="${currentSpellSlots}" style="width: 100%; height: 20px; --progress: #45b480 !important;"></progress><span id="percentage2" style="position: absolute; left: 50%; top: 50%; transform: translate(-50%, -70%); color: white; font-weight: bold;">Magie</span></div><div style="width: 60px; text-align: center;">${percentValue}%</div></div>`; 
> dv.el('div', metaBindCode); 
> ```
> 
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
> | [[Größenkategorie]] | `=this.Aussehen.Größenkategorie` |
> | Größe | `=this.Aussehen.Größe` |
> | Gewicht | `=this.Aussehen.Gewicht` |
> | Augenfarbe | `=this.Aussehen.Augenfarbe` |
> | Haarfarbe | `=this.Aussehen.Haarfarbe` |
> | Hautfarbe | `=this.Aussehen.Hautfarbe` |
>
> ## Persönlichkeit
> ---
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

## Allgemein
> [!column | 3 no-title]
>> ```dynamic-embed
>> [[embed Character Sheet Allgemein]]
>> ```
>
>> ### Cooldowns
>> |                    | Maximal                                                                                   | Aufladung      |
>> | ------------------ | ----------------------------------------------------------------------------------------- | -------------- |
>> | [[Tiergestalt]]    | `INPUT[toggle:InputData.TiergestaltLadung1]` `INPUT[toggle:InputData.TiergestaltLadung2]` | [[Kurze Rast]] |
>> | [[Geistertotem]]   | `INPUT[toggle:InputData.GeistertotemLadung]`                                              | [[Kurze Rast]] |
>> | [[Nebelschritt]]   | `INPUT[toggle:InputData.NebelschrittLadung]`                                              | [[Lange Rast]] |
>> | [[Identifizieren]] | `INPUT[toggle:InputData.IdentifizierenLadung]`                                            | [[Lange Rast]] |
>>
>> ### Tiergestalten
>> 
>> ```dataview
>> TABLE WITHOUT ID
>> file.link AS "Tier",
>> HG
>> FROM #Kreatur/Tier 
>> SORT HG DESC
>> WHERE HG = "1/4" OR HG = "1/8" OR HG = 0
>> ```
>
>> ### Bewegung
>> ```dynamic-embed
>> [[embed Character Sheet Bewegung]]
>> ```

## Verteidigung
> [!column | 2 no-title] 
>> ### Gesundheit
>> ```dynamic-embed
>> [[embed Character Sheet Gesundheit]]
>> ```
>
>> ### Rüstung
>> ```dynamic-embed
>> [[embed Character Sheet Rüstung]]
>> ```

## Attribute und Fertigkeiten
> [!column  | 3 no-title]
>> ### Stärke
>> ```dynamic-embed
>> [[embed Character Sheet Attribute Stärke]]
>> ```
>
>> ### Geschicklichkeit
>> ```dynamic-embed
>> [[embed Character Sheet Attribute Geschicklichkeit]]
>> ```
>
>> ### Konstitution
>> ```dynamic-embed
>> [[embed Character Sheet Attribute Konstitution]]
>> ```
>
>> ### Intelligenz
>> ```dynamic-embed
>> [[embed Character Sheet Attribute Intelligenz]]
>> ```
>
>> ### Weisheit
>> ```dynamic-embed
>> [[embed Character Sheet Attribute Weisheit]]
>> ```
>
>> ### Charisma
>> ```dynamic-embed
>> [[embed Character Sheet Attribute Charisma]]
>> ```

## Angriff
> [!column | 2 no-title]
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

## Magie
>[!column | 2 no-title]
>> #### Zauberparameter
>>| | |
>>| --- | --- |
>> | Zauberattribut | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberattribut` |
>> | Zauberangriffsbonus   | `$=Math.ceil((dv.current().Stufe/4)+1)+Math.floor(((dv.current().Attribute[dv.page(dv.page(dv.current().Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)`   |
>> | Zauberrettungswurf-SG | `$=8+Math.ceil((dv.current().Stufe/4)+1)+Math.floor(((dv.current().Attribute[dv.page(dv.page(dv.current().Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)` |
>> | Zaubertricks | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad0` |
>> | Bekannte Zauber | `$=dv.current().Stufe+Math.floor(((dv.current().Attribute[dv.page(dv.page(dv.current().Hintergrund.Klasse).Zauberattribut).file.name])-10)/2)`  |
>>
>>  #### Zauberplätze
>> | Grad |    [[Zauberplätze]] Maximal     |      [[Zauberplätze]] aktuell       |
>> |:----:|:-------------------------------:|:-----------------------------------:|
>> |  1   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad1` | `INPUT[number():InputData.Zauberplätze.Grad_1]` |
>> |  2   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad2` | `INPUT[number():InputData.Zauberplätze.Grad_2]` |
>> |  3   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad3` | `INPUT[number():InputData.Zauberplätze.Grad_3]` |
>> |  4   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad4` | `INPUT[number():InputData.Zauberplätze.Grad_4]` |
>> |  5   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad5` | `INPUT[number():InputData.Zauberplätze.Grad_5]` |
>> |  6   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad6` | `INPUT[number():InputData.Zauberplätze.Grad_6]` |
>> |  7   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad7` | `INPUT[number():InputData.Zauberplätze.Grad_7]` |
>> |  8   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad8` | `INPUT[number():InputData.Zauberplätze.Grad_8]` |
>> |  9   | `$=dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad9` | `INPUT[number():InputData.Zauberplätze.Grad_9]` |
>
>> #### Zaubertricks
>> ```dataview
>> TABLE WITHOUT ID
>> file.link AS "Zauber",
>> Schule,
>> Zeitaufwand, 
>> Schadensart,
>> Schaden AS "Schaden ab Lv. 1",
>> SchadenLv5 AS "Schaden ab Lv. 5",
>> Ziel,
>> Reichweite, 
>> choice(Verbal,"X","") AS "Verbal", 
>> choice(Geste,"X","") AS "Geste", 
>> Dauer, 
>> choice(Konzentration,"X","") AS "Konzentration", 
>> choice(Ritual,"X","") AS "Ritual"
>> FROM #Zauber
>> WHERE contains(this.Zauber, file.link) AND Grad=0
>> SORT file.name
>> ```
>> 
>> #### Grad 1
>> ```dataview
>> TABLE WITHOUT ID
>> file.link AS "Zauber",
>> Schule,
>> Zeitaufwand, 
>> Schadensart,
>> Schaden,
>> Ziel,
>> Reichweite, 
>> choice(Verbal,"X","") AS "Verbal", 
>> choice(Geste,"X","") AS "Geste", 
>> Dauer, 
>> choice(Konzentration,"X","") AS "Konzentration", 
>> choice(Ritual,"X","") AS "Ritual", 
>> choice(Skalierbar,"X","") AS "Skalierbar" 
>> FROM #Zauber
>> WHERE contains(this.Zauber, file.link) AND Grad=1
>> SORT file.name
>> ```
>> 
>> #### Grad 2
>> ```dataview
>> TABLE WITHOUT ID
>> file.link AS "Zauber",
>> Schule,
>> Zeitaufwand, 
>> Schadensart,
>> Schaden,
>> Ziel,
>> Reichweite, 
>> choice(Verbal,"X","") AS "Verbal", 
>> choice(Geste,"X","") AS "Geste", 
>> Dauer, 
>> choice(Konzentration,"X","") AS "Konzentration", 
>> choice(Ritual,"X","") AS "Ritual", 
>> choice(Skalierbar,"X","") AS "Skalierbar" 
>> FROM #Zauber
>> WHERE contains(this.Zauber, file.link) AND Grad=2
>> SORT file.name
>> ```
>> 
>> #### Grad 3
>> ```dataview
>> TABLE WITHOUT ID
>> file.link AS "Zauber",
>> Schule,
>> Zeitaufwand, 
>> Schadensart,
>> Schaden,
>> Ziel,
>> Reichweite, 
>> choice(Verbal,"X","") AS "Verbal", 
>> choice(Geste,"X","") AS "Geste", 
>> Dauer, 
>> choice(Konzentration,"X","") AS "Konzentration", 
>> choice(Ritual,"X","") AS "Ritual", 
>> choice(Skalierbar,"X","") AS "Skalierbar" 
>> FROM #Zauber
>> WHERE contains(this.Zauber, file.link) AND Grad=3
>> SORT file.name
>> ```
>

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

## Übung
> [!column | 4 no-title]
>> ### Rüstung
>> ```dynamic-embed
>> [[embed Character Sheet Übung Rüstung]]
>> ```
> 
>> ### Waffen
>> ```dynamic-embed
>> [[embed Character Sheet Übung Waffen]]
>> ```
>
>> ### Sprachen
>> ```dynamic-embed
>> [[embed Character Sheet Übung Sprachen]]
>> ```
>
>> ### Werkzeuge
>> ```dynamic-embed
>> [[embed Character Sheet Übung Werkzeuge]]
>> ```

## Hintergrundgeschichte
* Vater Waldelf 
* Mutter Mensch (lebt in der Stadt)
* aufgewachsen im Stamm des Vaters
* Der Stamm lebte im Wald in besonderer Beziehung zu einem Einhorn
* Stamm wurde von einem bösen Wesen ausgelöscht
* Während des Angriffs schnell ausgeschaltet / getötet
* Das Einhorn wurde ebenfalls getötet und fiel auf den Halbelfen
* Durch die Berührung des Hornes überlebte der Halbelf
* Sagte durch das traumatische Erlebnis den dämonischen Mächten den Kampf an
* Leidet seit dem Angriff gelegentlich unter angsteinflössenden Visionen und Alpträumen, die er mit diversen Mitteln betäubt
* Trägt das abgetrennte Einhorn als Totem


## Meta

```meta-bind-button
label: Kurze Rast
icon: switch
hidden: true
class: ""
tooltip: ""
id: "kurzeRast"
style: primary
actions:
  - type: updateMetadata
    bindTarget: InputData.TiergestaltLadung1
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.TiergestaltLadung2
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.GeistertotemLadung
    evaluate: false
    value: "false"
```

```meta-bind-button
label: Lange Rast
icon: reset
hidden: true
class: ""
tooltip: ""
id: "langeRast"
style: primary
actions:
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const tw = mb.parseBindTarget('Gesundheit.TW', context.file.path); const stufe = mb.getMetadata(mb.parseBindTarget('Stufe', context.file.path)); mb.setMetadata(tw, stufe);"
  - type: updateMetadata
    bindTarget: InputData.TiergestaltLadung1
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.TiergestaltLadung2
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.GeistertotemLadung
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.NebelschrittLadung
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.IdentifizierenLadung
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.Stresslevel1
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.Stresslevel2
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.Stresslevel3
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.Stresslevel4
    evaluate: false
    value: "false"
  - type: updateMetadata
    bindTarget: InputData.Stresslevel5
    evaluate: false
    value: "false"
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const grad = mb.parseBindTarget('InputData.Zauberplätze.Grad_1', context.file.path); const stufe = mb.getMetadata(mb.parseBindTarget('Stufe', context.file.path)); const value = mb.getMetadata(mb.parseBindTarget('Zauberplätze.Stufe' + stufe + '.Grad1', 'Charaktere/Klassen/Druide/Druide.md'));  mb.setMetadata(grad, value);"
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const grad = mb.parseBindTarget('InputData.Zauberplätze.Grad_2', context.file.path); const stufe = mb.getMetadata(mb.parseBindTarget('Stufe', context.file.path)); const value = mb.getMetadata(mb.parseBindTarget('Zauberplätze.Stufe' + stufe + '.Grad2', 'Charaktere/Klassen/Druide/Druide.md'));  mb.setMetadata(grad, value);"
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const grad = mb.parseBindTarget('InputData.Zauberplätze.Grad_3', context.file.path); const stufe = mb.getMetadata(mb.parseBindTarget('Stufe', context.file.path)); const value = mb.getMetadata(mb.parseBindTarget('Zauberplätze.Stufe' + stufe + '.Grad3', 'Charaktere/Klassen/Druide/Druide.md'));  mb.setMetadata(grad, value);"
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const grad = mb.parseBindTarget('InputData.Zauberplätze.Grad_4', context.file.path); const stufe = mb.getMetadata(mb.parseBindTarget('Stufe', context.file.path)); const value = mb.getMetadata(mb.parseBindTarget('Zauberplätze.Stufe' + stufe + '.Grad4', 'Charaktere/Klassen/Druide/Druide.md'));  mb.setMetadata(grad, value);"
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const grad = mb.parseBindTarget('InputData.Zauberplätze.Grad_5', context.file.path); const stufe = mb.getMetadata(mb.parseBindTarget('Stufe', context.file.path)); const value = mb.getMetadata(mb.parseBindTarget('Zauberplätze.Stufe' + stufe + '.Grad5', 'Charaktere/Klassen/Druide/Druide.md'));  mb.setMetadata(grad, value);"
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const grad = mb.parseBindTarget('InputData.Zauberplätze.Grad_6', context.file.path); const stufe = mb.getMetadata(mb.parseBindTarget('Stufe', context.file.path)); const value = mb.getMetadata(mb.parseBindTarget('Zauberplätze.Stufe' + stufe + '.Grad6', 'Charaktere/Klassen/Druide/Druide.md'));  mb.setMetadata(grad, value);"
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const grad = mb.parseBindTarget('InputData.Zauberplätze.Grad_7', context.file.path); const stufe = mb.getMetadata(mb.parseBindTarget('Stufe', context.file.path)); const value = mb.getMetadata(mb.parseBindTarget('Zauberplätze.Stufe' + stufe + '.Grad7', 'Charaktere/Klassen/Druide/Druide.md'));  mb.setMetadata(grad, value);"
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const grad = mb.parseBindTarget('InputData.Zauberplätze.Grad_8', context.file.path); const stufe = mb.getMetadata(mb.parseBindTarget('Stufe', context.file.path)); const value = mb.getMetadata(mb.parseBindTarget('Zauberplätze.Stufe' + stufe + '.Grad8', 'Charaktere/Klassen/Druide/Druide.md'));  mb.setMetadata(grad, value);"
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const grad = mb.parseBindTarget('InputData.Zauberplätze.Grad_9', context.file.path); const stufe = mb.getMetadata(mb.parseBindTarget('Stufe', context.file.path)); const value = mb.getMetadata(mb.parseBindTarget('Zauberplätze.Stufe' + stufe + '.Grad9', 'Charaktere/Klassen/Druide/Druide.md'));  mb.setMetadata(grad, value);"
  - type: updateMetadata
    bindTarget: InputData.ErschöpfungsPunkte
    evaluate: true
    value: x - 1
  - type: inlineJS
    code: "const mb = engine.getPlugin('obsidian-meta-bind-plugin').api; const TP = mb.parseBindTarget('Gesundheit.TP', context.file.path); const maxTP = mb.getMetadata(mb.parseBindTarget('Gesundheit.MaxTP', context.file.path));  mb.setMetadata(TP, maxTP);"
```

```dynamic-embed
[[embed Character Sheet Erschöpfung Code]]
```