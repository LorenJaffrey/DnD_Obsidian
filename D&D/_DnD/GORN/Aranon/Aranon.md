---
Stufe: 4
Glück: 0
Erschöpfung: 0
Bewegung: 6
Rüstung: "[[Lederrüstung]]"
Schild: "[[Holzschild]]"
Waffen:
- "[[Kampfstab]]"
- "[[Krummsäbel]]"
- "[[Schleuder]]"
Gesundheit:
  MaxTP: 31
  TP: 25
  TW: 4
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
  Volk:
    - "[[Dunkelsicht]]"
    - "[[Feenblut]]"
  Klasse:
    - "[[Die Sprache des Waldes]]"
    - "[[Druidisch]]"
    - "[[Tiergestalt]]"
    - "[[Geistertotem]]"
    - "[[Zauberwirken Druide]]"
  Talente:
    - "[[Von Feen berührt]]"
Hintergrund:
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
---
# `=this.file.name`

> [!infobox]
> ![[Aranon.jpg]]
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

[[Übung|Übungsbonus]]:  `=ceil(this.Stufe/4)+1`
[[Initiative|Initiativebonus]]: `=floor(((this.Attribute.Geschicklichkeit)-10)/2)`
[[Glückspunkte]]: `=this.Glück`
[[Erschöpft|Erschöpfung]]: `=this.Erschöpfung`

## Bewegung
| Gehen                                              | [[Spurt]]                                          | [[Hochsprung]] mit Anlauf                            | [[Hochsprung]] ohne Anlauf                           | [[Weitsprung]] mit Anlauf | [[Weitsprung]] ohne Anlauf |
| -------------------------------------------------- | -------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- | ------------------------- | -------------------------- |
| `=this.Bewegung*1.5` m (`=this.Bewegung` Kästchen) | `=this.Bewegung*3` m (`=this.Bewegung*2` Kästchen) | `=((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3)` m | `=((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3)/2` m | `=round((this.Attribute.Stärke*0.3)/2,2)` m                          | `=round((this.Attribute.Stärke*0.3),2)` m                           |
|                                                    |                                                    |                                                      |                                                      |                           |                            |
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
>> | `=this.Rüstung` `=choice(this.Schild, ", ", "")` `=choice(this.Schild, this.Schild, "")`  | `=10+floor(((this.Attribute.Geschicklichkeit)-10)/2)+choice(this.Rüstung.RP, this.Rüstung.RP, 0)` + `=choice(this.Schild, this.Schild.RP, 0)` | `=choice(this.Rüstung, this.Rüstung.SR, 0)` + `=choice(this.Schild.SR, this.Schild.SR, 0)` |

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
>> FROM #Waffe/Klasse/Nahkampfwaffe 
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
>> floor(((this.Attribute.Geschicklichkeit)-10)/2)+ceil(this.Stufe/4)+1 AS "Bonus",
>> SchadenFern+"+"+floor((((this.Attribute.Geschicklichkeit)-10)/2)) AS "Schaden",
>> SchadensartFern AS "Schadensart",
>> EigenschaftenFern AS "Eigenschaften"
>> FROM #Waffe/Klasse/Fernkampfwaffe/Schusswaffe 
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
>> FROM #Waffe/Klasse/Fernkampfwaffe/Wurfwaffe  
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
>> | [[Fertigkeiten\|Fertigkeit]] | Attribut                  |                                                                                       Fertigkeitswurfmodifikator                                                                                        |
>> | ---------------------------- | ------------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
>> | [[Akrobatik]]                | [[Geschicklichkeit]]      |                                                 `=floor(((this.Attribute.Geschicklichkeit)-10)/2)+(this.Fertigkeiten.Akrobatik*(ceil(this.Stufe/4)+1))`                                                 |
>> | [[Arkane Kunde]]             | [[Intelligenz]]           |                                                  `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Arkane_Kunde*(ceil(this.Stufe/4)+1))`                                                  |
>> | [[Athletik]]                 | [[Stärke]]                |                                                      `=floor(((this.Attribute.Stärke)-10)/2)+(this.Fertigkeiten.Athletik*(ceil(this.Stufe/4)+1))`                                                       |
>> | [[Auftreten]]                | [[Charisma]]              |                                                     `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Auftreten*(ceil(this.Stufe/4)+1))`                                                     |
>> | [[Einschüchtern]]            | [[Charisma]] / [[Stärke]] | `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Einschüchtern*(ceil(this.Stufe/4)+1))` / `=floor(((this.Attribute.Stärke)-10)/2)+(this.Fertigkeiten.Einschüchtern*(ceil(this.Stufe/4)+1))` |
>> | [[Fingerfertigkeit]]         | [[Geschicklichkeit]]      |                                             `=floor(((this.Attribute.Geschicklichkeit)-10)/2)+(this.Fertigkeiten.Fingerfertigkeit*(ceil(this.Stufe/4)+1))`                                              |
>> | [[Geschichte]]               | [[Intelligenz]]           |                                                   `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Geschichte*(ceil(this.Stufe/4)+1))`                                                   |
>> | [[Heilkunde]]                | [[Weisheit]]              |                                                     `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Heilkunde*(ceil(this.Stufe/4)+1))`                                                     |
>> | [[Heimlichkeit]]             | [[Geschicklichkeit]]      |                                               `=floor(((this.Attribute.Geschicklichkeit)-10)/2)+(this.Fertigkeiten.Heimlichkeit*(ceil(this.Stufe/4)+1))`                                                |
>> | [[Mit Tieren umgehen]]       | [[Weisheit]]              |                                                `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Mit_Tieren_umgehen*(ceil(this.Stufe/4)+1))`                                                 |
>> | [[Motiv erkennen]]           | [[Weisheit]]              |                                                  `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Motiv_erkennen*(ceil(this.Stufe/4)+1))`                                                   |
>> | [[Nachforschungen]]          | [[Intelligenz]]           |                                                `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Nachforschungen*(ceil(this.Stufe/4)+1))`                                                 |
>> | [[Naturkunde]]               | [[Intelligenz]]           |                                                   `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Naturkunde*(ceil(this.Stufe/4)+1))`                                                   |
>> | [[Religion]]                 | [[Intelligenz]]           |                                                    `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Religion*(ceil(this.Stufe/4)+1))`                                                    |
>> | [[Täuschen]]                 | [[Charisma]]              |                                                     `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Täuschen*(ceil(this.Stufe/4)+1))`                                                      |
>> | [[Überlebenskunst]]          | [[Weisheit]]              |                                                  `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Überlebenskunst*(ceil(this.Stufe/4)+1))`                                                  |
>> | [[Überzeugen]]               | [[Charisma]]              |                                                    `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Überzeugen*(ceil(this.Stufe/4)+1))`                                                     |
>> | [[Wahrnehmung]]              | [[Weisheit]]              |                                                    `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Wahrnehmung*(ceil(this.Stufe/4)+1))`                                                    |
>>
>>[[Wahrnehmung#Passive Wahrnehmung]]: `=10+floor(((this.Attribute.Weisheit)-10)/2)`

## Übung

> [!column]
>> ## Rüstung
>> ```dataview
>> LIST
>> FROM #Ausrüstung/Rüstung
>> WHERE contains(this.Übung.Rüstungen, file.link) 
>> SORT file.name
>> ```
>> 
>> ## Waffen
>> ```dataview
>> LIST
>> FROM #Waffe 
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
>> FROM #Werkzeug
>> WHERE contains(this.Übung.Werkzeuge, file.link)
>> SORT file.name
>> ```

## Merkmale
> [!column]
>> ## Volksmerkmale
>> ```dataview
>> LIST
>> FROM #Merkmal
>> WHERE contains(this.Merkmale.Volk, file.link)
>> SORT file.name
>> ```
>>
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