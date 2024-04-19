---
Stufe: 4
Glück: 0
Erschöpfung: 0
Bewegung: 6
Rüstung: "[[Lederrüstung]]"
Schild:
Waffen:
- "[[Dolch]]"
Gesundheit:
  MaxTP: 29
  TP: 16
  TW: 4
  TempTP: 0
Attribute:
  Stärke: 10
  Geschicklichkeit: 14
  Konstitution: 13
  Intelligenz: 14
  Weisheit: 8
  Charisma: 18
Rettungswürfe:
  Stärke: 0
  Geschicklichkeit: 0
  Konstitution: 0
  Intelligenz: 0
  Weisheit: 1
  Charisma: 1
Fertigkeiten:
  Akrobatik: 0
  Arkane_Kunde: 1
  Athletik: 0
  Auftreten: 0
  Einschüchtern: 0
  Fingerfertigkeit: 0
  Geschichte: 1
  Heilkunde: 0
  Heimlichkeit: 0
  Mit_Tieren_umgehen: 0
  Motiv_erkennen: 0
  Nachforschungen: 1
  Naturkunde: 0
  Religion: 0
  Täuschen: 1
  Überlebenskunst: 0
  Überzeugen: 0
  Wahrnehmung: 0
Übung:
  Sprachen:
    - "[[Gemeinsprache]]"
    - "[[Infernalisch]]"
    - "[[Abyssisch]]"
    - "[[Urtümlich]]"
  Werkzeuge:
  Rüstungen:
    - "[[Leichte Rüstung]]"
  Waffen:
    - "[[Einfache Waffen]]"
Aussehen:
  Geschlecht: männlich
  Alter: 39 Jahre
  Größenkategorie: "[[Mittelgroß]]"
  Größe: 184 cm
  Gewicht: 165 Pfund
  Augenfarbe: Gold
  Haarfarbe: Schwarz
  Hautfarbe: Menschlich
Merkmale:
  Volk:
    - "[[Dunkelsicht]]"
    - "[[Höllische Resistenz]]"
    - "[[Infernalisches Erbe]]"
  Klasse:
    - "[[Paktmagie]]"
    - "[[Pakt des Buches]]"
    - "[[Segen des dunklen Meisters]]"
    - "[[Qualvoller Strahl]]"
    - Zweite Schauerliche Anrufung?
  Talente:
    - "[[Infernalische Konstitution]]"
Hintergrund:
  Volk: "[[Tieflinge|Tiefling]]"
  Klasse: "[[Hexenmeister]]"
  Subklasse: "[[Der Unhold]]"
  Gesinnung: "[[Chaotisch Neutral]]"
  Hintergrund: "[[Weiser]]"
Persönlichkeit:
  Persönlichkeitsmerkmale:
  - wortgewandt
  - extrovertiert 
  - strategisch
  Ideale: Wissen, Macht, Selbstverwirklichung, Selbstfindung
  Bindungen: Buch der Schatten, Teuflischer Pakt
  Makel: eitel, egoistisch, kein Teilen von Gedanken oder Plänen
tags:
- Charakter/GORN
---
# `=this.file.name`

> [!infobox]
> > ![[Lucian.jpg]]
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
| Gehen                                              | [[Spurt]]                                          | [[Hochsprung]] mit Anlauf                            | [[Hochsprung]] ohne Anlauf                             | [[Weitsprung]] mit Anlauf                 | [[Weitsprung]] ohne Anlauf                  |
| -------------------------------------------------- | -------------------------------------------------- | ---------------------------------------------------- | ------------------------------------------------------ | ----------------------------------------- | ------------------------------------------- |
| `=this.Bewegung*1.5` m (`=this.Bewegung` Kästchen) | `=this.Bewegung*3` m (`=this.Bewegung*2` Kästchen) | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)` m | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)/2` m | `=round((this.Attribute.Stärke*0.3),2)` m | `=round((this.Attribute.Stärke*0.3)/2,2)` m |

## Verteidigung
> [!column] 
>> ## Gesundheit
>> |         | [[Trefferpunkte]]        | [[Trefferwürfel]]        | [[Temporäre Trefferpunkte]] |
>> | ------- | ------------------------ | ------------------------ | --------------------------- |
>> | Maximal | `=this.Gesundheit.MaxTP` | `=this.Stufe` `=this.Hintergrund.Klasse.Trefferwürfel` |                             |
>> | Aktuell | `=this.Gesundheit.TP`    | `=this.Gesundheit.TW` `=this.Hintergrund.Klasse.Trefferwürfel`    | `=this.Gesundheit.TempTP`   |
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
>> floor(((this.Attribute.Geschicklichkeit)-10)/2)+ceil(this.Stufe/4)+1 AS "Bonus",
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

### Aussehen
Lucian Blackthorn ist ein männlicher Tiefling-Hexenmeister von auffallender Erscheinung. 
Er ist groß und schlank mit einer athletischen Statur. 
Seine Haut ist menschlich und seine Augen leuchten in einem lebhaften Goldton, was ihm einen exotischen und fesselnden Blick verleiht. 
Sein Haar ist wild und schwarz, oft in unkonventionellen Frisuren gestylt, und er trägt einen gepflegten Drei-Tage-Bart, der sein selbstbewusstes Lächeln betont.

Lucians Hörner sind lang und geschwungen, ähnlich wie die eines gehörnten Dämons, und sie sind mit goldenen Verzierungen verziert, die seine Stärke und Macht betonen. 
Er kleidet sich gerne in auffällige und extravagante Roben, die mit goldenen oder silbernen Akzenten geschmückt sind und seinen selbstbewussten und extrovertierten Charakter widerspiegeln.

## Charakterbeschreibung
Lucian wurde als Sohn einer angesehenen Hexenmeisterfamilie in einer düsteren und mysteriösen Stadt geboren. 
Von klein auf war er von der Magie fasziniert und zeigte ein außergewöhnliches Talent für die dunklen Künste. 
Seine Eltern erkannten sein Potenzial und unterrichteten ihn in den Geheimnissen der Hexerei und des Okkultismus.

Mit der Zeit entwickelte sich Lucians Persönlichkeit zu einem extrovertierten und charismatischen Charakter, der es liebte, die Menschen um sich herum zu beeindrucken und zu unterhalten. 
Er reiste durch die Welt, um sein Wissen über die Magie zu erweitern und seine Fähigkeiten als Hexenmeister zu perfektionieren. 
Während seiner Reisen traf er auf verschiedene Abenteurergruppen und beteiligte sich an epischen Schlachten gegen dunkle Mächte und gefährliche Kreaturen.

Lucian ist bekannt für seine unkonventionellen Methoden und seinen unbändigen Hunger nach Macht und Wissen. 
Er ist jedoch auch bereit, seine Fähigkeiten und seine Magie einzusetzen, um denjenigen zu helfen, die seine Hilfe suchen und die gegen das Böse kämpfen. 
Sein Ruf als furchtloser und charismatischer Hexenmeister verbreitet sich weit und breit, und sein außergewöhnliches Aussehen und seine theatralische Persönlichkeit machen ihn zu einer unvergesslichen Figur in jeder Gesellschaft, der er begegnet.

Trotz seiner extrovertierten Natur und seinem gelegentlichen Hang zur Dramatik ist Lucian nicht ohne innere Dämonen.
Er trägt die Last seiner tieflingischen Herkunft und die ständige Versuchung der dunklen Künste, die in ihm schlummern. 
Er ist jedoch entschlossen, seine Kräfte für das Gute einzusetzen und das Böse zu bekämpfen, auch wenn er manchmal am Rande des Abgrunds tanzt.

Das ist Lucian Blackthorn, ein extrovertierter und charismatischer Tiefling-Hexenmeister, der mit seinem exotischen Aussehen, seiner theatralischen Persönlichkeit und seinen mächtigen Hexenmeisterzaubern die Menschen um sich herum fasziniert und beeindruckt.

Lucian ist ein Charakter mit extrovertierter Persönlichkeit und einem ausgeprägten Selbstbewusstsein. 
Er liebt es, im Mittelpunkt der Aufmerksamkeit zu stehen und zieht die Blicke anderer auf sich, sei es durch seine imposante Erscheinung oder seine gewandte Art zu sprechen.
Er ist charmant und überzeugend, mit einer ausgeprägten sozialen Intelligenz, die es ihm ermöglicht, mit Menschen auf unterschiedlichen Ebenen zu interagieren.

Lucian ist ein leidenschaftlicher Redner und liebt es, seine magischen Kräfte und sein Wissen über die dunklen Künste zu präsentieren. 
Er ist bekannt für seine theatralischen Auftritte und seine Fähigkeit, die Massen zu begeistern und zu faszinieren.
Er ist ein extrovertierter Entertainer und liebt es, die Grenzen des Konventionellen zu überschreiten und neue Erfahrungen zu machen.

Trotz seines extrovertierten Charakters ist Lucian auch klug und strategisch in seinen Entscheidungen. 
Er ist ein erfahrener Hexenmeister, der seine magischen Kräfte geschickt einsetzt, um seine Ziele zu erreichen und seine Feinde zu besiegen. 
Er ist jedoch auch bekannt für seine Unberechenbarkeit und seine Fähigkeit, in unerwartete Richtungen zu handeln, was ihn zu einem faszinierenden und manchmal beängstigenden Charakter macht.

Der Name des Unholdes muss erfahren werden um gesamtheitlich Macht über ihn zu gelangen. 
Der Unhold ist schon lange Begleiter der Familie und ist Fluch und Segen zu gleich. 
Er hilft in Notsituationen und kämpft an der Seite der Familie, verfolgt aber seine eigenen eher dunklen Interessen. 