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
| Pflanzenart | Umgebung                  |
| ----------- | ------------------------- |
| Grün        | Wald, Grasland, Sumpf     |
| Wasser      | Küste, Sumpf, Unterwasser |
| Trocken     | Wüste, Gebirge            |
| Kalt        | Gebirge, Arktisch         |
| Pilz        | Wald, Sumpf, Unterreich   |