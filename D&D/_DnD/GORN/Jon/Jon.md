---
tags:
- Charakter/GORN/Jon
Name: Jon "Verisus" Longbow
Stufe: 4
Glück: 0
Erschöpfung: 0
Bewegung: 6
Rüstung: "[[Beschlagene Lederrüstung]]"
Schild: "[[Holzschild]]"
Waffen:
- "[[Langbogen]]"
- "[[Leichte Armbrust]]"
- "[[Kurzschwert]]"
- "[[Krummsäbel]]"
- "[[Dolch]]"
Feinde: "[[Orks]]"
Gesundheit:
  MaxTP: 39
  TP: 39
  TW: 4
  TempTP: 0
Attribute:
  Stärke: 12
  Geschicklichkeit: 18
  Konstitution: 14
  Intelligenz: 8
  Weisheit: 14
  Charisma: 10
Rettungswürfe:
  Stärke: 1
  Geschicklichkeit: 0
  Konstitution: 1
  Intelligenz: 0
  Weisheit: 0
  Charisma: 0
Fertigkeiten:
  Akrobatik: 1
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
  Nachforschungen: 0
  Naturkunde: 0
  Religion: 0
  Täuschen: 0
  Überlebenskunst: 1
  Überzeugen: 0
  Wahrnehmung: 1
Übung:
  Sprachen:
    - "[[Gemeinsprache]]"
    - "[[Orkisch]]"
  Werkzeuge:
    - "[[Holzschnitzwerkzeuge]]"
    - "[[Spiel|Spiele]]"
  Rüstungen:
    - "[[Leichte Rüstung]]"
    - "[[Mittelschwere Rüstung]]"
    - "[[Schwere Rüstung]]"
    - "[[Schilde]]"
  Waffen:
    - "[[Einfache Waffen]]"
    - "[[Kriegswaffen]]"
Aussehen:
  Geschlecht: männlich
  Alter: 29 Jahre
  Größenkategorie: "[[Mittelgroß]]"
  Größe: 180 cm
  Gewicht: 198 Pfund
  Augenfarbe: Grün
  Haarfarbe: Schwarz
  Hautfarbe: Weiß
Merkmale:
  Volk:
  Klasse:
    - "[[Durchschnaufen]]"
    - "[[Tatendrang]]"
    - "[[Kampfüberlegenheit#Schlag des Befehlshabers]]"
    - "[[Kampfüberlegenheit#Fällender Angriff]]"
    - "[[Kampfüberlegenheit#Parieren]]"
  Talente:
    - "[[Heiler]]"
    - "[[Meisterschaft Bögen]]"
Hintergrund:
  Volk: "[[Menschen|Mensch]]"
  Klasse: "[[Kämpfer]]"
  Subklasse: "[[Kampfmeister]]"
  Gesinnung: "[[Rechtschaffen Neutral]]"
  Hintergrund: "[[Söldner]]"
Persönlichkeit:
  Persönlichkeitsmerkmale:
  - Ich stelle mich Problemen frontal. Eine einfache, direkte Lösung ist der beste Weg zum Erfolg. Ich habe einen derben Sinn für Humor.
  Ideale: Leben und leben lassen. Ideale sind es nicht wert, dafür zu töten oder in den Krieg zu ziehen. (Neutral)
  Bindungen: Ich werde nie die vernichtende Niederlage vergessen, die meine Kompanie erlitten hat, oder die Feinde, die ihr zugefügt haben.
  Makel: Abneigung gegen militärische Führungspositionen / Autorität
tags:
- Charakter/GORN/Jon
---
# `=this.file.name`

> [!infobox]
> ![[Jon.jpeg]]
> ## Hintergrund
> |  |  |
> | ---- | ---- |
> |Name|`=this.Name`|
> | Stufe | `=this.Stufe` |
> | [[Völker\|Volk]] | `=this.Hintergrund.Volk` |
> | [[Klassen\|Klasse]] | `=this.Hintergrund.Klasse` |
> |  `$=dv.page(dv.current().Hintergrund.Klasse).Name_Subklassen` | `=this.Hintergrund.Subklasse` |
> | [[Gesinnung]] | `=this.Hintergrund.Gesinnung` |
> | [[_Übersicht Hintergründe\|Hintergrund]] | `=this.Hintergrund.Hintergrund` |
> |Feinde| `=this.Feinde`|
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
> ### Ideale
> `=this.Persönlichkeit.Ideale`
> ### Bindungen
> `=this.Persönlichkeit.Bindungen`
> ### Makel
> `=this.Persönlichkeit.Makel`
> ### Werdegang
> - Alter: 5-12 ~ Ausbildung in Bogenschießen
> - Alter: 13-17 Jahren ~ Soldaten Ausbildung/Training
> - Alter: 18-28 ~ Teil einer Armee
> - Alter: 29-? ~ Söldner/Abenteurer
> - Dracheninsel erkundet
> 	- Skelette getötet
> 	- Riesen-Schlange/Echse
> 	- blauen Drachen getötet
> 	- Kobolde getötet
> - Neverwinter
> 	- Goblins getötet
> - Phandalin
> 	- Magier getötet

[[Übung|Übungsbonus]]:  `=ceil(this.Stufe/4)+1`
[[Initiative|Initiativebonus]]: `=floor(((this.Attribute.Geschicklichkeit)-10)/2)`
[[Glückspunkte]]: `=this.Glück`
[[Erschöpft|Erschöpfung]]: `=this.Erschöpfung`

## Bewegung
| Gehen                                              | [[Spurt]]                                          | [[Hochsprung]] mit Anlauf                            | [[Hochsprung]] ohne Anlauf                             | [[Weitsprung]] mit Anlauf                 | [[Weitsprung]] ohne Anlauf                  |
| -------------------------------------------------- | -------------------------------------------------- | ---------------------------------------------------- | ------------------------------------------------------ | ----------------------------------------- | ------------------------------------------- |
| `=this.Bewegung*1.5` m (`=this.Bewegung` Kästchen) | `=this.Bewegung*3` m (`=this.Bewegung*2` Kästchen) | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)` m | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)/2` m | `=round((this.Attribute.Stärke*0.3),2)` m | `=round((this.Attribute.Stärke*0.3)/2,2)` m |

## Verteidigung
> [!column] 
>> ## Gesundheit
>> |         | [[Trefferpunkte]]        | [[Trefferwürfel]]        | [[Temporäre Trefferpunkte]] |
>> | ------- | ------------------------ | ------------------------ | --------------------------- |
>> | Maximal | `=this.Gesundheit.MaxTP` | `=this.Stufe` `=this.Hintergrund.Klasse.Trefferwürfel` |                             |
>> | Aktuell | `=this.Gesundheit.TP`    | `=this.Gesundheit.TW`    | `=this.Gesundheit.TempTP`   |
>
>>## Rüstung
>> | Rüstung         | [[Rüstungsklasse]]                                                                                             | [[Schadensreduktion]]                                                                                         |
>> | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
>> | `=this.Rüstung` `=choice(this.Schild, ", ", "")` `=choice(this.Schild, this.Schild, "")`  | `=10+floor(((this.Attribute.Geschicklichkeit)-10)/2)+choice(this.Rüstung.RP, this.Rüstung.RP, 0)` + `=choice(this.Schild, this.Schild.RP, 0)` | `=choice(this.Rüstung.SR, this.Rüstung.SR, 0)` + `=choice(this.Schild.SR, this.Schild.SR, 0)` |

## Angriff
> [!column]
>> ### Nahkampfwaffen
>> ```dataview
>> TABLE WITHOUT ID 
>> file.link AS "Waffe",
>> Reichweite,
>> floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)+ceil(this.Stufe/4)+1 AS "Bonus",
>> Schaden+"+"+(floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)) AS "Schaden",
>> Schadensart,
>> Eigenschaften
>> FROM #Gegenstand/Waffe/Klasse/Nahkampfwaffe 
>> WHERE contains(this.Waffen, file.link)
>> SORT file.name
>> ```
>
>> ### Schusswaffen 
>> ```dataview
>> TABLE WITHOUT ID 
>> file.link AS "Waffe",
>> Range1 AS "Min RW",
>> Range2 AS "Gnd RW",
>> Range3 AS "Max RW",
>> 2+floor(((this.Attribute.Geschicklichkeit)-10)/2)+ceil(this.Stufe/4)+1 AS "Bonus",
>> SchadenFern+"+"+floor((((this.Attribute.Geschicklichkeit)-10)/2)) AS "Schaden",
>> SchadensartFern AS "Schadensart",
>> EigenschaftenFern AS "Eigenschaften"
>> FROM #Gegenstand/Waffe/Klasse/Fernkampfwaffe/Schusswaffe 
>> WHERE contains(this.Waffen, file.link)
>> SORT file.name
>> ```
>> 
>> ### Wurfwaffen
>> ```dataview
>> TABLE WITHOUT ID 
>> file.link AS "Waffe",
>> Range1 AS "Min RW",
>> Range2 AS "Gnd RW",
>> Range3 AS "Max RW",
>> floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)+ceil(this.Stufe/4)+1 AS "Bonus",
>> SchadenFern+"+"+(floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)) AS "Schaden",
>> SchadensartFern AS "Schadensart",
>> EigenschaftenFern AS "Eigenschaften"
>> FROM #Gegenstand/Waffe/Klasse/Fernkampfwaffe/Wurfwaffe  
>> WHERE contains(this.Waffen, file.link)
>> SORT file.name
>> ```

Disclaimer: Waffen haben immer Übungsbonus...
## Stats
> [!column]
>> ## Attribute
>> | [[Attribute\|Attribut]] |           Attributswert            |         [[Attribute#Attributsmodifikator]]         |                                            Rettungswurfmodifikator                                             |
>> | ----------------------- |:----------------------------------:|:--------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------:|
>> | [[Stärke]]              |      `=this.Attribute.Stärke`      |      `=floor(((this.Attribute.Stärke)-10)/2)`      |           `=floor(((this.Attribute.Stärke)-10)/2)+(this.Rettungswürfe.Stärke*(ceil(this.Stufe/4)+1))`           |
>> | [[Geschicklichkeit]]    | `=this.Attribute.Geschicklichkeit` | `=min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)` | `=min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)+(this.Rettungswürfe.Geschicklichkeit*(ceil(this.Stufe/4)+1))` |
>> | [[Konstitution]]        |   `=this.Attribute.Konstitution`   |   `=floor(((this.Attribute.Konstitution)-10)/2)`   |     `=floor(((this.Attribute.Konstitution)-10)/2)+(this.Rettungswürfe.Konstitution*(ceil(this.Stufe/4)+1))`     |
>> | [[Intelligenz]]         |   `=this.Attribute.Intelligenz`    |   `=floor(((this.Attribute.Intelligenz)-10)/2)`    |      `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Rettungswürfe.Intelligenz*(ceil(this.Stufe/4)+1))`      |
>> | [[Weisheit]]            |     `=this.Attribute.Weisheit`     |     `=floor(((this.Attribute.Weisheit)-10)/2)`     |         `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Rettungswürfe.Weisheit*(ceil(this.Stufe/4)+1))`         |
>> | [[Charisma]]            |     `=this.Attribute.Charisma`     |     `=floor(((this.Attribute.Charisma)-10)/2)`     |         `=floor(((this.Attribute.Charisma)-10)/2)+(this.Rettungswürfe.Charisma*(ceil(this.Stufe/4)+1))`         |
>
>> ## Fertigkeiten
>> | [[Fertigkeiten\|Fertigkeit]] | Attribut                  |                                                                                       Fertigkeitswurfmodifikator                                                                                        | Übung                                                                                                                       |
>> | ---------------------------- | ------------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:| --------------------------------------------------------------------------------------------------------------------------- |
>> | [[Akrobatik]]                | [[Geschicklichkeit]]      |                                                 `=floor(((this.Attribute.Geschicklichkeit)-10)/2)+(this.Fertigkeiten.Akrobatik*(ceil(this.Stufe/4)+1))`                                                 | `=choice(this.Fertigkeiten.Akrobatik=2, "Expertise", choice(this.Fertigkeiten.Akrobatik=1, "Übung", ""))`                   |
>> | [[Arkane Kunde]]             | [[Intelligenz]]           |                                                  `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Arkane_Kunde*(ceil(this.Stufe/4)+1))`                                                  | `=choice(this.Fertigkeiten.Arkane_Kunde=2, "Expertise", choice(this.Fertigkeiten.Arkane_Kunde=1, "Übung", ""))`             |
>> | [[Athletik]]                 | [[Stärke]]                |                                                      `=floor(((this.Attribute.Stärke)-10)/2)+(this.Fertigkeiten.Athletik*(ceil(this.Stufe/4)+1))`                                                       | `=choice(this.Fertigkeiten.Athletik=2, "Expertise", choice(this.Fertigkeiten.Athletik=1, "Übung", ""))`                     |
>> | [[Auftreten]]                | [[Charisma]]              |                                                     `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Auftreten*(ceil(this.Stufe/4)+1))`                                                     | `=choice(this.Fertigkeiten.Auftreten=2, "Expertise", choice(this.Fertigkeiten.Auftreten=1, "Übung", ""))`                   |
>> | [[Einschüchtern]]            | [[Charisma]] / [[Stärke]] | `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Einschüchtern*(ceil(this.Stufe/4)+1))` / `=floor(((this.Attribute.Stärke)-10)/2)+(this.Fertigkeiten.Einschüchtern*(ceil(this.Stufe/4)+1))` | `=choice(this.Fertigkeiten.Einschüchtern=2, "Expertise", choice(this.Fertigkeiten.Einschüchtern=1, "Übung", ""))`           |
>> | [[Fingerfertigkeit]]         | [[Geschicklichkeit]]      |                                             `=floor(((this.Attribute.Geschicklichkeit)-10)/2)+(this.Fertigkeiten.Fingerfertigkeit*(ceil(this.Stufe/4)+1))`                                              | `=choice(this.Fertigkeiten.Fingerfertigkeit=2, "Expertise", choice(this.Fertigkeiten.Fingerfertigkeit=1, "Übung", ""))`     |
>> | [[Geschichte]]               | [[Intelligenz]]           |                                                   `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Geschichte*(ceil(this.Stufe/4)+1))`                                                   | `=choice(this.Fertigkeiten.Geschichte=2, "Expertise", choice(this.Fertigkeiten.Geschichte=1, "Übung", ""))`                 |
>> | [[Heilkunde]]                | [[Weisheit]]              |                                                     `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Heilkunde*(ceil(this.Stufe/4)+1))`                                                     | `=choice(this.Fertigkeiten.Heilkunde=2, "Expertise", choice(this.Fertigkeiten.Heilkunde=1, "Übung", ""))`                   |
>> | [[Heimlichkeit]]             | [[Geschicklichkeit]]      |                                               `=floor(((this.Attribute.Geschicklichkeit)-10)/2)+(this.Fertigkeiten.Heimlichkeit*(ceil(this.Stufe/4)+1))`                                                | `=choice(this.Fertigkeiten.Heimlichkeit=2, "Expertise", choice(this.Fertigkeiten.Heimlichkeit=1, "Übung", ""))`             |
>> | [[Mit Tieren umgehen]]       | [[Weisheit]]              |                                                `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Mit_Tieren_umgehen*(ceil(this.Stufe/4)+1))`                                                 | `=choice(this.Fertigkeiten.Mit_Tieren_umgehen=2, "Expertise", choice(this.Fertigkeiten.Mit_Tieren_umgehen=1, "Übung", ""))` |
>> | [[Motiv erkennen]]           | [[Weisheit]]              |                                                  `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Motiv_erkennen*(ceil(this.Stufe/4)+1))`                                                   | `=choice(this.Fertigkeiten.Motiv_erkennen=2, "Expertise", choice(this.Fertigkeiten.Motiv_erkennen=1, "Übung", ""))`         |
>> | [[Nachforschungen]]          | [[Intelligenz]]           |                                                `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Nachforschungen*(ceil(this.Stufe/4)+1))`                                                 | `=choice(this.Fertigkeiten.Nachforschungen=2, "Expertise", choice(this.Fertigkeiten.Nachforschungen=1, "Übung", ""))`       |
>> | [[Naturkunde]]               | [[Intelligenz]]           |                                                   `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Naturkunde*(ceil(this.Stufe/4)+1))`                                                   | `=choice(this.Fertigkeiten.Naturkunde=2, "Expertise", choice(this.Fertigkeiten.Naturkunde=1, "Übung", ""))`                 |
>> | [[Religion]]                 | [[Intelligenz]]           |                                                    `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Religion*(ceil(this.Stufe/4)+1))`                                                    | `=choice(this.Fertigkeiten.Religion=2, "Expertise", choice(this.Fertigkeiten.Religion=1, "Übung", ""))`                     |
>> | [[Täuschen]]                 | [[Charisma]]              |                                                     `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Täuschen*(ceil(this.Stufe/4)+1))`                                                      | `=choice(this.Fertigkeiten.Täuschen=2, "Expertise", choice(this.Fertigkeiten.Täuschen=1, "Übung", ""))`                     |
>> | [[Überlebenskunst]]          | [[Weisheit]]              |                                                  `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Überlebenskunst*(ceil(this.Stufe/4)+1))`                                                  | `=choice(this.Fertigkeiten.Überlebenskunst=2, "Expertise", choice(this.Fertigkeiten.Überlebenskunst=1, "Übung", ""))`       |
>> | [[Überzeugen]]               | [[Charisma]]              |                                                    `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Überzeugen*(ceil(this.Stufe/4)+1))`                                                     | `=choice(this.Fertigkeiten.Überzeugen=2, "Expertise", choice(this.Fertigkeiten.Überzeugen=1, "Übung", ""))`                 |
>> | [[Wahrnehmung]]              | [[Weisheit]]              |                                                    `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Wahrnehmung*(ceil(this.Stufe/4)+1))`                                                    | `=choice(this.Fertigkeiten.Wahrnehmung=2, "Expertise", choice(this.Fertigkeiten.Wahrnehmung=1, "Übung", ""))`               |
>>
>>[[Wahrnehmung#Passive Wahrnehmung]]: `=10+floor(((this.Attribute.Weisheit)-10)/2)`

## Übung

> [!column]
>> ## Rüstung
>> ```dataview
>> LIST
>> FROM #Gegenstand/Rüstung 
>> WHERE contains(this.Übung.Rüstungen, file.link) 
>> SORT file.name
>> ```
>> 
>> ## Waffen
>> ```dataview
>> LIST
>> FROM #Gegenstand/Waffe 
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
>> 
>> ## Werkzeuge
>> ```dataview
>> LIST
>> FROM #Gegenstand/Werkzeug 
>> WHERE contains(this.Übung.Werkzeuge, file.link)
>> SORT file.name
>> ```

## Merkmale
> [!column]
>> ## Talente
>> ```dataview
>> LIST
>> FROM #Talent
>> WHERE contains(this.Merkmale.Talente, file.link)
>> SORT file.name
>> ```
>
>> ## Klassenmerkmale
>> ```dataview
>> LIST
>> FROM #Merkmal
>> WHERE contains(this.Merkmale.Klasse, file.link)
>> SORT file.name
>> ```

## Aktionen
>[!column]
>> ## Kampfmerkmale (Verbrauch)
>>| Merkmal            | Verfügbar |
>>| ------------------ |:---------:|
>>| [[Durchschnaufen]] |    Ja    |
>>| [[Tatendrang]]             |    Ja     |
>>| [[Zusätzlicher Angriff]]  (Lv. 5) |    -     |
>>| [[Unbeugsamkeit]] (Lv. 9) |    -     |
>>| [[Zusätzlicher Angriff]]  (Lv. 11) |    -     |
>>| [[Zusätzlicher Angriff]]  (Lv. 20) |    -     |
>>
>>## Kurze Kampfmermal Aktions-Beschreibung
>>- **[[Durchschnaufen]]**
>>	**Auswirkung**: Heilt den Charakter
>>	**Verwendung**: 1x W10 + der Stufe des Kämpfers
>>	**Erholung**: kurze oder langen Rast
>>-  **[[Tatendrang]]**
>>	**Auswirkung**: Man kann nochmal im selben Zug  angreifen bzw. eine Aktion ausführen
>>	**Verwendung**: Kann 1 Mal verwendet werden
>>	**Erholung**: kurze oder langen Rast
>
>>## Manöver (Verbrauch)
>>| Ausgewählte Manöver                             | Verfügbar | Verfügbar | Verfügbar | Verfügbar | Verfügbar (Lv. 7) | Verfügbar (Lv. 15) |
>>| ----------------------------------------------- |:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|
>>| [[Kampfüberlegenheit#Schlag des Befehlshabers]] |    Ja    |    Ja     |    Ja     |    Ja     |    -    |    -    |
>>| [[Kampfüberlegenheit#Fällender Angriff]]        |    Ja    |    Ja     |    Ja     |    Ja     |    -    |    -    |
>>| [[Kampfüberlegenheit#Parieren]]                 |    Ja    |    Ja     |    Ja     |    Ja     |    -    |    -    |
>>
>>## Kurze Manöver Aktions-Beschreibung
>>- **[[Kampfüberlegenheit#Schlag des Befehlshabers]]**
>>        **Auswirkung**: Eigene Aktion + Bonus Aktion verwenden, damit verbündete Kreatur stattdessen als Reaktion  angreifen kann + Schadensbonus (Wert des Überlegenheitswürfels)
>>        **Verwendung**: Verbündete Kreatur muss mich sehen oder hören können
>> 
>>- **[[Kampfüberlegenheit#Fällender Angriff]]**
>>        **Auswirkung**: Versuchen das Ziel zu Fall zu bringen + Schadensbonus (Wert des Überlegenheitswürfels)
>>        **Verwendung**: Ziel (groß oder kleiner) muss Stärkerettungswurf ablegen
>> 
>>- **[[Kampfüberlegenheit#Parieren]]**
>>        **Auswirkung**: Schadensreduktion 
>>        **Verwendung**: Überlegenheitswürfel + Geschicklichkeitsmodifikator
>>
>>## Hinweis
>>- Überlegenheits-Würfel: W8
>>- Rettungswürfe gegen Manöver: `=8+ceil(this.Stufe/4)+1+min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)`


## Aussehen
- schlank
- athletisch
- gut aussehend
- leichter Bartwuchs

## Hintergrundgeschichte

### Kindheit & Ausbildung bei der Armee

Jon Longbow wurde in eine Familie von Soldaten geboren, die in der königlichen Armee dienten. Sein Vater war ein bekannter General, und seine Mutter war eine erfahrene Bogenschützin, die Soldaten im Bogenschießen ausbildete. Während seiner Kindheit war Jon von den Fähigkeiten seiner Mutter im Bogenschießen fasziniert und verbrachte die meiste Zeit damit, mit Pfeil und Bogen zu üben.
Im Alter von achtzehn Jahren trat Jon der Armee bei und trainierte hart, um ein Experte im Bogenschießen zu werden. Er stieg schnell in den Rängen auf und wurde zum Spezialisten im Bogenschießen. Sein natürliches Talent verdiente ihm den Spitznamen "Longbow" unter seinen Mitkämpfern.
Jons derber Sinn für Humor und seine Angewohnheit Fehler lieber zu leugnen als sie zuzugeben oder Entschuldigungen zu finden brachte ihn oft in Schwierigkeiten mit seinen Vorgesetzten. Während des Trainings machte er oft sarkastische Bemerkungen, die seine Ausbilder nervten, aber seine Mitkämpfer amüsierten.

### Kampagne gegen die Orks

Während einer Mission, um ein Dorf von raubenden Orks zu befreien, wurden Jon und seine Kameraden überfallen. Die Orks waren wilde Kämpfer, und die Schlacht war brutal und blutig. Im Chaos des Kampfes wurde Jons bester Freund und Mitbogenschütze von einem Ork getötet. Jon war von dem Verlust seines Freundes am Boden zerstört und fühlte sich für dessen Tod verantwortlich. Er wurde von Wut und einem Verlangen nach Rache gegenüber den Orks erfüllt. Er begann, sie als nichts weiter als blutrünstige Monster zu sehen, unfähig zu vernünftigem Handeln oder Mitgefühl. Als Jon weiterhin im Militär diente, traf er mehrmals auf Orks, und jede Begegnung diente nur dazu, seinen Hass zu schüren. Er sah sie als Bedrohung für die Menschheit und glaubte, dass sie ausgelöscht werden mussten.
Er hatte oft Schwierigkeiten, seine Emotionen im Umgang mit Orks zu kontrollieren und würde oft ohne Vorwarnung auf sie losgehen, selbst wenn er damit sich selbst und seine Kameraden in Gefahr brachte.
 
### Entlassung aus der Armee

Nachdem er viele Jahre in der Armee gedient hatte, wurde Jon Longbow zunehmend desillusioniert vom Militärleben. Die Handlungen die er im Auftrag seiner Vorgesetzten durchführen musste waren im immer mehr zuwider und widersprachen seinem persönlichen Ehrempfinden. Als er eines Tages den direkten Befehl eines vorgesetzten Offiziers missachtete, wurde er für seine Insubordination ausgepeitscht und unehrenhaft aus dem Militärdienst entlassen. Sehr zum Missfallen seines Vaters.
Von da an schlug er sich als Jäger und Söldner durchs Leben und frönte seiner Liebe zu Frauen und Alkohol um die schrecklichen Alpträume an seine verstümmelten und zerstückelten Kameraden zu verdrängen die ihn des Nachts wach halten...
