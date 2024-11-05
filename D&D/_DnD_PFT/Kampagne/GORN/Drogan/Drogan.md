---
Stufe: 5
Bewegung: 7
Verteidigung:
  Natürliche_Rüstung: 10
  Zusätzliche_Rüstung: 0
  Zusätzliche_SR: 0
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
  TP: 59
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
  Name: "Drogan"
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
# `=this.Hintergrund.Name`

> [!infobox]
> ## `=this.Hintergrund.Name`
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

## Allgemein
> [!column | 3 no-title] 
>> ```dynamic-embed
>> [[embed Character Sheet Allgemein]]
>> ```
>
>> ### Cooldowns
>> |                                                                                                                              |                                                                                                    |
>> | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
>> | Nutzungen [[Kampfrausch]] (max. `$=dv.page(dv.current().Hintergrund.Klasse).Kampfrausch["Stufe"+dv.current().Stufe].Anzahl`) | `INPUT[toggle:InputData.Rage1]` `INPUT[toggle:InputData.Rage2]` `INPUT[toggle:InputData.Rage3]`    |
>> | Bonuschaden [[Kampfrausch]]                                                                                                  | +`$=dv.page(dv.current().Hintergrund.Klasse).Kampfrausch["Stufe"+dv.current().Stufe].Bonusschaden` |
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
>> [[embed Character Sheet Rüstung Barbar]]
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
TBD

## Versteckte Logiken & Button Konfigurationen

```meta-bind-button
label: Kurze Rast
icon: switch
hidden: true
class: ""
tooltip: ""
id: "kurzeRast"
style: primary
actions:
  - type: inlineJS
    code: "console.log('Hello World!');"
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

 ```dynamic-embed
[[embed Character Sheet Erschöpfung Code]]
```