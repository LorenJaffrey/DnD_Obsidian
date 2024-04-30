---
Stufe: 4
Niptac:
  Anzahl_Apparaturen: 2
  Energiekerngröße: W6
  Apparaturen:
    - "[[Gnomischer Flammenwerfer]]"
    - "[[Gnomisches Überbrückungskabel]]"
Bewegung: 5
Rüstung: "[[Beschlagene Lederrüstung]]"
Schild:
Waffen:
  - "[[Kurzschwert]]"
  - "[[Dolch]]"
  - "[[Beil]]"
  - "[[Schleuder]]"
  - "[[Leichte Armbrust]]"
Gesundheit:
  MaxTP: 35
  TP: 35
  TW: 4
  TempTP: 0
Attribute:
  Stärke: 8
  Geschicklichkeit: 17
  Konstitution: 14
  Intelligenz: 14
  Weisheit: 10
  Charisma: 14
Rettungswürfe:
  Stärke: 0
  Geschicklichkeit: 1
  Konstitution: 0
  Intelligenz: 1
  Weisheit: 0
  Charisma: 0
Fertigkeiten:
  Akrobatik: 0
  Arkane_Kunde: 0
  Athletik: 0
  Auftreten: 0
  Einschüchtern: 0
  Fingerfertigkeit: 2
  Geschichte: 0
  Heilkunde: 0
  Heimlichkeit: 1
  Mit_Tieren_umgehen: 0
  Motiv_erkennen: 0
  Nachforschungen: 0
  Naturkunde: 0
  Religion: 0
  Täuschen: 2
  Überlebenskunst: 0
  Überzeugen: 1
  Wahrnehmung: 1
Übung:
  Sprachen:
    - "[[Gemeinsprache]]"
    - "[[Gnomisch]]"
    - "[[Diebessprache]]"
  Werkzeuge:
    - "[[Diebeswerkzeug]]"
    - "[[Tüftlerwerkzeug]]"
    - "[[Fälscherausrüstung]]"
  Rüstungen:
    - "[[Leichte Rüstung]]"
  Waffen:
    - "[[Einfache Waffen]]"
    - "[[Handarmbrüste]]"
    - "[[Kurzschwert]]"
    - "[[Langschwert]]"
    - "[[Rapier]]"
Aussehen:
  Geschlecht: männlich
  Alter: 99 Jahre
  Größenkategorie: "[[Klein]]"
  Größe: 102 cm
  Gewicht: 49 Pfund
  Augenfarbe: Braun
  Haarfarbe: Schwarz
  Hautfarbe: Ocker
Merkmale:
  Volk:
    - "[[Dunkelsicht]]"
    - "[[Gnomische Gerissenheit]]"
    - "[[Artefaktkunde]]"
    - "[[Tüftler]]"
  Klasse:
    - "[[Hinterhältiger Angriff]]"
    - "[[Durchdachte Vorbereitung]]"
    - "[[Raffinierte Aktion]]"
    - "[[Zielsicher]]"
  Talente:
    - "[[Verschwinden]]"
Hintergrund:
  Volk: "[[Gnome|Gnom]]"
  Klasse: "[[Schurke]]"
  Subklasse: "[[Meistertüftler]]"
  Gesinnung: "[[Neutral Gut]]"
  Hintergrund: "[[Scharlatan]]"
Persönlichkeit:
  Persönlichkeitsmerkmale:
  - Ich kenne einen Witz für jede Situation, besonders für die, in denen Humor unangebracht ist.
  Ideale: Unabhängigkeit. Ich bin ein Freigeist, niemand kann mir vorschreiben, was ich zu tun oder zu lassen habe.
  Bindungen: Eine mächtige Person hat jemanden, den ich liebte, getötet. Der Tag meiner Rache wird kommen.
  Makel: Ich kann es nicht lassen, diejenigen zu beleidigen, die mächtiger sind als ich.
tags:
- Charakter/GORN
---
# `=this.file.name`
> [!infobox]
> ![[Niptac.jpeg]]
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
> ### Ideale
> `=this.Persönlichkeit.Ideale`
> ### Bindungen
> `=this.Persönlichkeit.Bindungen`
> ### Makel
> `=this.Persönlichkeit.Makel`

[[Übung|Übungsbonus]]:  `=ceil(this.Stufe/4)+1`
[[Initiative|Initiativebonus]]: `=floor(((this.Attribute.Geschicklichkeit)-10)/2)`

> [!checks] 
> -  
> 	- [[Glück|Glückspunkte]] 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> -  
> 	- [[Erschöpft|Erschöpfung]]     
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 
> 	- [ ] %% %% 

## Niptac
### Aufladungen 
| [[Durchdachte Vorbereitung#Engergiekerne]] | Anzahl [[Durchdachte Vorbereitung#Engergiekerne]]                                                                                                                                       |         [[Verschwinden#Verschwinden]]         |
|:------------------------------------------:| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |:---------------------------------------------:|
|      `=this.Niptac.Energiekerngröße`       | <input type="checkbox" unchecked id="446ae6"> <input type="checkbox" unchecked id="5f3d3b"> <input type="checkbox" unchecked id="112c14"> <input type="checkbox" unchecked id="c98f08"> | <input type="checkbox" unchecked id="75076a"> |

### Apparaturen (max `=this.Niptac.Anzahl_Apparaturen`)
```dataview
TABLE WITHOUT ID
file.link AS "Apparaturen", 
SG AS "Schwierigkeitsgrad"
FROM #Merkmal/Klasse/Schurke/Meistertüftler/Apparatur 
WHERE contains(this.Niptac.Apparaturen, file.link)
SORT SG, file.link
```

## Bewegung
| Gehen                                              | [[Spurt]]                                          | [[Hochsprung]] mit Anlauf                            | [[Hochsprung]] ohne Anlauf                             | [[Weitsprung]] mit Anlauf                 | [[Weitsprung]] ohne Anlauf                  |
| -------------------------------------------------- | -------------------------------------------------- | ---------------------------------------------------- | ------------------------------------------------------ | ----------------------------------------- | ------------------------------------------- |
| `=this.Bewegung*1.5` m (`=this.Bewegung` Kästchen) | `=this.Bewegung*3` m (`=this.Bewegung*2` Kästchen) | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)` m | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)/2` m | `=round((this.Attribute.Stärke*0.3),2)` m | `=round((this.Attribute.Stärke*0.3)/2,2)` m |

## Verteidigung

### Gesundheit
|             | [[Trefferpunkte]]               | [[Trefferwürfel]] (`=this.Hintergrund.Klasse.Trefferwürfel`) | [[Temporäre Trefferpunkte]]         |
| ----------- | ------------------------------- | ------------------------------------------------------------ | ----------------------------------- |
| **Aktuell** | `INPUT[number():Gesundheit.TP]` | `INPUT[number():Gesundheit.TW]`                              | `INPUT[number():Gesundheit.TempTP]` |
| Maximal     | `=this.Gesundheit.MaxTP`        | `=this.Stufe`                                                |                                     |


### Rüstung
| Rüstung                                                                                  | [[Rüstungsklasse]]                                                                                                                            | [[Schadensreduktion]]                                                                         |
| ---------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `=this.Rüstung` `=choice(this.Schild, ", ", "")` `=choice(this.Schild, this.Schild, "")` | `=10+floor(((this.Attribute.Geschicklichkeit)-10)/2)+choice(this.Rüstung.RP, this.Rüstung.RP, 0)` + `=choice(this.Schild, this.Schild.RP, 0)` | `=choice(this.Rüstung.SR, this.Rüstung.SR, 0)` + `=choice(this.Schild.SR, this.Schild.SR, 0)` |

## Angriff

### Nahkampfwaffen
```dataview
TABLE WITHOUT ID 
file.link AS "Waffe",
Reichweite,
floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)+ceil(this.Stufe/4)+1 AS "Bonus",
Schaden+"+"+(floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)) AS "Schaden",
Schadensart,
Eigenschaften
FROM #Gegenstand/Waffe/Klasse/Nahkampfwaffe
WHERE contains(this.Waffen, file.link)
SORT file.name
```

### Schusswaffen 
```dataview
TABLE WITHOUT ID 
file.link AS "Waffe",
Range1 AS "Min RW",
Range2 AS "Gnd RW",
Range3 AS "Max RW",
floor(((this.Attribute.Geschicklichkeit)-10)/2)+ceil(this.Stufe/4)+1 AS "Bonus",
SchadenFern+"+"+floor((((this.Attribute.Geschicklichkeit)-10)/2)) AS "Schaden",
SchadensartFern AS "Schadensart",
EigenschaftenFern AS "Eigenschaften"
FROM #Gegenstand/Waffe/Klasse/Fernkampfwaffe/Schusswaffe
WHERE contains(this.Waffen, file.link)
SORT file.name
```

### Wurfwaffen
```dataview
TABLE WITHOUT ID 
file.link AS "Waffe",
Range1 AS "Min RW",
Range2 AS "Gnd RW",
Range3 AS "Max RW",
floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)+ceil(this.Stufe/4)+1 AS "Bonus",
SchadenFern+"+"+(floor(((choice(contains(Eigenschaften, [[Finesse]]), this.Attribute.Geschicklichkeit, this.Attribute.Stärke))-10)/2)) AS "Schaden",
SchadensartFern AS "Schadensart",
EigenschaftenFern AS "Eigenschaften"
FROM #Gegenstand/Waffe/Klasse/Fernkampfwaffe/Wurfwaffe 
WHERE contains(this.Waffen, file.link)
SORT file.name
```

Disclaimer: Waffen haben immer Übungsbonus...
## Stats
### Attribute
| [[Attribute\|Attribut]] |           Attributswert            |                      [[Attribute#Attributsmodifikator]]                      |                                                          Rettungswurfmodifikator                                                          |
| ----------------------- |:----------------------------------:|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------:|
| [[Stärke]]              |      `=this.Attribute.Stärke`      |                   `=floor(((this.Attribute.Stärke)-10)/2)`                   |                        `=floor(((this.Attribute.Stärke)-10)/2)+(this.Rettungswürfe.Stärke*(ceil(this.Stufe/4)+1))`                        |
| [[Geschicklichkeit]]    | `=this.Attribute.Geschicklichkeit` | `=min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)` | `=min(floor(((this.Attribute.Geschicklichkeit)-10)/2),this.Rüstung.Dex_cap)+(this.Rettungswürfe.Geschicklichkeit*(ceil(this.Stufe/4)+1))` |
| [[Konstitution]]        |   `=this.Attribute.Konstitution`   |                `=floor(((this.Attribute.Konstitution)-10)/2)`                |                  `=floor(((this.Attribute.Konstitution)-10)/2)+(this.Rettungswürfe.Konstitution*(ceil(this.Stufe/4)+1))`                  |
| [[Intelligenz]]         |   `=this.Attribute.Intelligenz`    |                `=floor(((this.Attribute.Intelligenz)-10)/2)`                 |                   `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Rettungswürfe.Intelligenz*(ceil(this.Stufe/4)+1))`                   |
| [[Weisheit]]            |     `=this.Attribute.Weisheit`     |                  `=floor(((this.Attribute.Weisheit)-10)/2)`                  |                      `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Rettungswürfe.Weisheit*(ceil(this.Stufe/4)+1))`                      |
| [[Charisma]]            |     `=this.Attribute.Charisma`     |                  `=floor(((this.Attribute.Charisma)-10)/2)`                  |                      `=floor(((this.Attribute.Charisma)-10)/2)+(this.Rettungswürfe.Charisma*(ceil(this.Stufe/4)+1))`                      |

### Fertigkeiten
| [[Fertigkeiten\|Fertigkeit]] | Attribut                  |                                                                                       Fertigkeitswurfmodifikator                                                                                        | Übung                                                                                                                       |
| ---------------------------- | ------------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:| --------------------------------------------------------------------------------------------------------------------------- |
| [[Akrobatik]]                | [[Geschicklichkeit]]      |                                                 `=floor(((this.Attribute.Geschicklichkeit)-10)/2)+(this.Fertigkeiten.Akrobatik*(ceil(this.Stufe/4)+1))`                                                 | `=choice(this.Fertigkeiten.Akrobatik=2, "Expertise", choice(this.Fertigkeiten.Akrobatik=1, "Übung", ""))`                   |
| [[Arkane Kunde]]             | [[Intelligenz]]           |                                                  `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Arkane_Kunde*(ceil(this.Stufe/4)+1))`                                                  | `=choice(this.Fertigkeiten.Arkane_Kunde=2, "Expertise", choice(this.Fertigkeiten.Arkane_Kunde=1, "Übung", ""))`             |
| [[Athletik]]                 | [[Stärke]]                |                                                      `=floor(((this.Attribute.Stärke)-10)/2)+(this.Fertigkeiten.Athletik*(ceil(this.Stufe/4)+1))`                                                       | `=choice(this.Fertigkeiten.Athletik=2, "Expertise", choice(this.Fertigkeiten.Athletik=1, "Übung", ""))`                     |
| [[Auftreten]]                | [[Charisma]]              |                                                     `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Auftreten*(ceil(this.Stufe/4)+1))`                                                     | `=choice(this.Fertigkeiten.Auftreten=2, "Expertise", choice(this.Fertigkeiten.Auftreten=1, "Übung", ""))`                   |
| [[Einschüchtern]]            | [[Charisma]] / [[Stärke]] | `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Einschüchtern*(ceil(this.Stufe/4)+1))` / `=floor(((this.Attribute.Stärke)-10)/2)+(this.Fertigkeiten.Einschüchtern*(ceil(this.Stufe/4)+1))` | `=choice(this.Fertigkeiten.Einschüchtern=2, "Expertise", choice(this.Fertigkeiten.Einschüchtern=1, "Übung", ""))`           |
| [[Fingerfertigkeit]]         | [[Geschicklichkeit]]      |                                             `=floor(((this.Attribute.Geschicklichkeit)-10)/2)+(this.Fertigkeiten.Fingerfertigkeit*(ceil(this.Stufe/4)+1))`                                              | `=choice(this.Fertigkeiten.Fingerfertigkeit=2, "Expertise", choice(this.Fertigkeiten.Fingerfertigkeit=1, "Übung", ""))`     |
| [[Geschichte]]               | [[Intelligenz]]           |                                                   `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Geschichte*(ceil(this.Stufe/4)+1))`                                                   | `=choice(this.Fertigkeiten.Geschichte=2, "Expertise", choice(this.Fertigkeiten.Geschichte=1, "Übung", ""))`                 |
| [[Heilkunde]]                | [[Weisheit]]              |                                                     `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Heilkunde*(ceil(this.Stufe/4)+1))`                                                     | `=choice(this.Fertigkeiten.Heilkunde=2, "Expertise", choice(this.Fertigkeiten.Heilkunde=1, "Übung", ""))`                   |
| [[Heimlichkeit]]             | [[Geschicklichkeit]]      |                                               `=floor(((this.Attribute.Geschicklichkeit)-10)/2)+(this.Fertigkeiten.Heimlichkeit*(ceil(this.Stufe/4)+1))`                                                | `=choice(this.Fertigkeiten.Heimlichkeit=2, "Expertise", choice(this.Fertigkeiten.Heimlichkeit=1, "Übung", ""))`             |
| [[Mit Tieren umgehen]]       | [[Weisheit]]              |                                                `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Mit_Tieren_umgehen*(ceil(this.Stufe/4)+1))`                                                 | `=choice(this.Fertigkeiten.Mit_Tieren_umgehen=2, "Expertise", choice(this.Fertigkeiten.Mit_Tieren_umgehen=1, "Übung", ""))` |
| [[Motiv erkennen]]           | [[Weisheit]]              |                                                  `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Motiv_erkennen*(ceil(this.Stufe/4)+1))`                                                   | `=choice(this.Fertigkeiten.Motiv_erkennen=2, "Expertise", choice(this.Fertigkeiten.Motiv_erkennen=1, "Übung", ""))`         |
| [[Nachforschungen]]          | [[Intelligenz]]           |                                                `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Nachforschungen*(ceil(this.Stufe/4)+1))`                                                 | `=choice(this.Fertigkeiten.Nachforschungen=2, "Expertise", choice(this.Fertigkeiten.Nachforschungen=1, "Übung", ""))`       |
| [[Naturkunde]]               | [[Intelligenz]]           |                                                   `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Naturkunde*(ceil(this.Stufe/4)+1))`                                                   | `=choice(this.Fertigkeiten.Naturkunde=2, "Expertise", choice(this.Fertigkeiten.Naturkunde=1, "Übung", ""))`                 |
| [[Religion]]                 | [[Intelligenz]]           |                                                    `=floor(((this.Attribute.Intelligenz)-10)/2)+(this.Fertigkeiten.Religion*(ceil(this.Stufe/4)+1))`                                                    | `=choice(this.Fertigkeiten.Religion=2, "Expertise", choice(this.Fertigkeiten.Religion=1, "Übung", ""))`                     |
| [[Täuschen]]                 | [[Charisma]]              |                                                     `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Täuschen*(ceil(this.Stufe/4)+1))`                                                      | `=choice(this.Fertigkeiten.Täuschen=2, "Expertise", choice(this.Fertigkeiten.Täuschen=1, "Übung", ""))`                     |
| [[Überlebenskunst]]          | [[Weisheit]]              |                                                  `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Überlebenskunst*(ceil(this.Stufe/4)+1))`                                                  | `=choice(this.Fertigkeiten.Überlebenskunst=2, "Expertise", choice(this.Fertigkeiten.Überlebenskunst=1, "Übung", ""))`       |
| [[Überzeugen]]               | [[Charisma]]              |                                                    `=floor(((this.Attribute.Charisma)-10)/2)+(this.Fertigkeiten.Überzeugen*(ceil(this.Stufe/4)+1))`                                                     | `=choice(this.Fertigkeiten.Überzeugen=2, "Expertise", choice(this.Fertigkeiten.Überzeugen=1, "Übung", ""))`                 |
| [[Wahrnehmung]]              | [[Weisheit]]              |                                                    `=floor(((this.Attribute.Weisheit)-10)/2)+(this.Fertigkeiten.Wahrnehmung*(ceil(this.Stufe/4)+1))`                                                    | `=choice(this.Fertigkeiten.Wahrnehmung=2, "Expertise", choice(this.Fertigkeiten.Wahrnehmung=1, "Übung", ""))`               |

[[Wahrnehmung#Passive Wahrnehmung]]: `=10+floor(((this.Attribute.Weisheit)-10)/2)`

## Übung

### Rüstung
```dataview
LIST
FROM #Gegenstand/Rüstung
WHERE contains(this.Übung.Rüstungen, file.link) 
SORT file.name
```
 
### Waffen
```dataview
LIST
FROM #Gegenstand/Waffe 
WHERE contains(this.Übung.Waffen, file.link) 
SORT file.name
```

### Sprachen
```dataview
LIST
FROM #Sprache
WHERE contains(this.Übung.Sprachen, file.link)
SORT file.name
```

## Werkzeuge
```dataview
LIST
FROM #Gegenstand/Werkzeug
WHERE contains(this.Übung.Werkzeuge, file.link)
SORT file.name
```

## Merkmale
### Volksmerkmale
```dataview
LIST
FROM #Merkmal
WHERE contains(this.Merkmale.Volk, file.link)
SORT file.name
```

### Talente
```dataview
LIST
FROM #Talent
WHERE contains(this.Merkmale.Talente, file.link)
SORT file.name
```

### Klassenmerkmale
```dataview
LIST
FROM #Merkmal
WHERE contains(this.Merkmale.Klasse, file.link)
SORT file.name
```

## Aussehen
Niptac ist ein kleiner, schlanker Gnom mit wildem, struppigem Haar und einer spitzen Nase. Er trägt oft schmutzige Kleidung und eine alte Lederjacke, um sich vor Wind und Wetter zu schützen. Seine Augen sind immer wachsam und vorsichtig, und er hält sich oft im Hintergrund, um nicht aufzufallen.

## Hintergrundgeschichte
Niptac wurde als jüngstes Kind einer Familie von Gnome geboren. Sein Vater war ein Magier, der in vielen Schlachten gekämpft hatte, um das Königreich zu verteidigen. Seine Mutter war eine begabte Mechanikerin und Ingenieurin, die viele nützliche Maschinen und Werkzeuge entwickelt hatte, um das Leben ihrer Familie einfacher zu gestalten.
Niptac wuchs in einer glücklichen Familie auf, leider besaß er keinerlei Talent für Magie, wie sein Vater, auch wenn er es oft versuchte Ihm beizubringen. Daher ließ er sich von seiner Mutter in die Geheimnisse der Mechanik einweihen und versuchte damit sein mangelndes magisches Geschick auszugleichen.

Eines Tages kehrte sein Vater nicht von einer Schlacht zurück, und die Familie war am Boden zerstört. Niptacs Mutter musste hart arbeiten, um die Familie über Wasser zu halten, und Niptac übernahm viele Aufgaben im Haushalt, um ihr zu helfen.

Als Niptac älter wurde, entwickelte er eine Leidenschaft für das Schmuggeln und den Handel mit verbotenen Gütern. Er erkannte, dass er damit seiner Familie helfen und seine Mutter von der harten Arbeit entlasten konnte. Er begann, seine Fähigkeiten als Dieb und Schmuggler zu entwickeln und wurde schließlich zu einem der besten in der Stadt.

Obwohl Niptac ein Dieb war, hatte er eine starke Moral und stahl nur von reichen Händlern und Adligen, die es sich leisten konnten, etwas zu verlieren. Er spendete auch regelmäßig einen Teil seines Einkommens an Bedürftige in der Stadt und unterstützte seine Familie so gut er konnte.

Niptac hat immer noch die Erinnerung an seinen Vater und den Mut, sowie die Weisheit, die er in der Schlacht gezeigt hat, in sich. Er hofft, dass er eines Tages selbst in der Lage sein wird, sein Königreich zu verteidigen und seine Familie stolz zu machen.
