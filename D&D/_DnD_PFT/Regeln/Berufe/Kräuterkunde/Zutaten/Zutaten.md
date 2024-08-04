---
tags:
  - Beruf/Kräuterkunde
aliases:
  - Kraut
---
# `=this.file.name`

| Zutat            | Effekt Roh                                              | Effekt Trank                                               | benötigte Dosen | SG  |
| ---------------- | ------------------------------------------------------- | ---------------------------------------------------------- | --------------- | --- |
| [[Winterkuss]]   | Keine Erschöpfung durch Kälte                           | Schadensresistenz gegen Kälteschaden                       | 6               | 18  |
| [[Ilmenblatt]]   | Vorteil bei Rettungswürfen auf Weisheit für eine Stunde |                                                            | 4               | 20  |
| [[Schneelilie]]  |             |                    |                 |     |
|                  |                                                         | Immun gegen [[Bezaubert]] und [[Verängstigt]] für 1 Stunde | 4               | 18  |
| [[Thonnys]]      | Vorteil auf [[Konzentration]] für 1 Stunde              |                                                            | 4               | 18  |
|                  | Erhöht die Geschwindigkeit um 1,5m für eine Stunde      | Erhöht Initiative um 1 für 1 Stunde                        | 3               | 19  |
| [[Blutgras]]     |                                                         |                                                            | 6               | 18  |
| Leerenwurzel     |                                                         |                                                            | 6               | 18  |
| [[Amanitakappe]] |                                                         |                                                            | 5               | 20  |
| [[Eisdorn]]      |                                                         |                                                            |                 |     |

```dataview
TABLE WITHOUT ID
file.link AS "Kraut",
Art,
Effekt.Roh AS "Effekt Roh",
Effekt.Verarbeitet AS "Effekt Verarbeitet"
FROM #Beruf/Kräuterkunde/Zutat
WHERE file.name != "Vorlage Kräuterkunde-Zutat"
SORT Art, file.name
```



## Pflanzenvorkommen
| Umgebung    | Beeren | Blätter | Blüten | Gräser | Pilze | Rinden | Wurzeln |
| ----------- |:------:|:-------:|:------:|:------:|:-----:|:------:|:-------:|
| Arktisch    |        |         |        |        |       |   X    |    X    |
| Küste       |        |    X    |        |   X    |       |        |         |
| Gebirgsland |        |    X    |        |        |       |   X    |         |
| Grasland    |   X    |         |   X    |        |       |        |         |
| Hügelland   |   X    |    X    |        |        |       |        |         |
| Sumpfland   |        |         |   X    |        |   X   |        |         |
| Unterreich  |        |    X    |        |        |   X   |        |         |
| Waldland    |   X    |         |        |        |       |   X    |         |
| Wüste       |        |         |   X    |   X    |       |        |         |
