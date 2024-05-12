---
tags:
  - Beruf/Kräuterkunde
aliases:
  - Kraut
---
# `=this.file.name`

| Zutat               | Effekt Roh                                                       | Effekt Trank                                                  | benötigte Dosen | SG  |
| ------------------- | ---------------------------------------------------------------- | ------------------------------------------------------------- | --------------- | --- |
| Schattiges Moos     | Vorteil auf Rettungswurf gegen Gifte                             | Schadensresistenz gegen Giftschaden für 1 Stunde              | 4               | 20  |
| [[Tarnele]]         | +2 Erholung aus nächstem [[Trefferwürfel]]                       | Maximale Erholung aus nächstem [[Trefferwürfel]]              | 5               | 20  |
| [[Rubinmorchel]]    | +2 Erholung aus nächstem [[Trefferwürfel]]                       |                                                               |                 |     |
| [[Blaukappe]]       | Verlangsamt Infektionen durch gewöhnliche Krankheiten            | Heilt gewöhnliche Krankheiten                                 | 5               | 15  |
| [[Jorugawurzel]]    | Verlangsamt Infektionen durch gewöhnliche Krankheiten            |                                                               | 5               | 15  |
| [[Belmartblatt]]    | Gewährt 3 temporäre Trefferpunkte für eine Stunde                |                                                               | 3               | 19  |
| [[Weißweidenrinde]] | Gewährt 3 temporäre Trefferpunkte für eine Stunde                | Gewährt 10 temporäre Trefferpunkte für eine Stunde            | 5               | 20  |
| [[Ilmenblatt]]      | Vorteil bei Rettungswürfen auf Weisheit für eine Stunde          | Immun gegen [[Verängstigt]] und [[Bezaubert]] für 1 Stunden   | 4               | 20  |
| Rote Kaktee         | Vorteil bei Rettungswürfen auf Konstitution für eine Stunde      | Besteht automatisch Todesrettungswürfe für 1 Stunde           | 4               | 20  |
|                     | Vorteil bei Rettungswürfen auf Charisma für eine Stunde          | Vorteil auf Überzeugen, Täuschen, Motiv erkennen für 1 Stunde | 4               | 20  |
| [[Blutwurzel]]      | Reduziert eine Erschöpfungsstufe                                 | Entfernt alle Erschöpfungsstufen bei einer langen Rast        | 4               | 20  |
| [[Drakusblume]]     | Reduziert eine Erschöpfungsstufe                                 | Heilt Lähmung                                                 | 6               | 18  |
| [[Donfstängel]]     | +2 Bonus auf [[Wahrnehmung#Passive Wahrnehmung]] für eine Stunde | +5 Bonus auf Passive Wahrnehmung für eine Stunde              | 3               | 15  |
| [[Hydradistel]]     | Vorteil auf [[Warhnehmung]] für 1 Stunde (Sicht)                 | Heilt [[Blind\|Blindheit]]                                    | 5               | 19  |
| [[Olginwurzel]]     | Vorteil auf [[Warhnehmung]] für 1 Stunde (Gehör)                 | Heilt [[Taub\|Taubheit]]                                      | 5               | 19  |
| [[Windsporen]]      | Maximale Atemanhaltezeit verdoppelt                              | Muss 1 Stunde lang nicht atmen                                |                 |     |
| [[Dianthuskraut]]   | Maximale Atemanhaltezeit verdoppelt                              | Erhält Schwimmbewegung gleich normaler Bewegung               | 4               | 18  |
| [[Krötenschemel]]   | Gewährt [[Dunkelsicht]] für 1 Stunde                             | Gewährt [[Überlegene Dunkelsicht]] für 1 Stunde               | 5               | 20  |
| Liliendistel        | Vorteil bei Rettungswurf gegen [[Bezaubert]] und [[Verängstigt]] | Immun gegen [[Bezaubert]] und [[Verängstigt]] für 1 Stunde    | 4               | 18  |
| [[Thonnys]]         | Vorteil auf [[Konzentration]] für 1 Stunde                       |                                                               | 4               | 18  |
| [[Gulmondblatt]]    | Vorteil auf [[Athletik]] für 1 Stunde                            | +1 auf Schadenswürfe für 1 Stunde                             | 5               | 20  |
| [[Atmonblüte]]      | Erhöht die Geschwindigkeit um 1,5m für eine Stunde               | Erhöht [[Rüstungsklasse]] um 1 für 1 Stunde                   | 6               | 20  |
| Spornwurzel         | Erhöht die Geschwindigkeit um 1,5m für eine Stunde               | Erhöht Initiative um 1 für 1 Stunde                           | 3               | 19  |
| [[Blutgras]]        |                                                                  |                                                               | 6               | 18  |
| Leerenwurzel        |                                                                  |                                                               | 6               | 18  |
| [[Amanitakappe]]    |                                                                  |                                                               | 5               | 20  |
| [[Eisdorn]]         | Keine Erschöpfung durch Kälte                                    | Schadensresistenz gegen Kälteschaden                          | 6               | 18  |

```dataview
TABLE WITHOUT ID
file.link AS "Kraut",
Art,
Effekt.Roh AS "Effekt Roh",
Effekt.Verarbeitet AS "Effekt Verarbeitet",
AnzahlDosenFürVerarbeitung AS "Dosen",
VerarbeitungsSG AS "SG"
FROM #Beruf/Kräuterkunde/Zutat
WHERE file.name != "Vorlage Kräuterkunde-Zutat"
SORT file.name
```

## Pflanzenvorkommen
| Pflanzenart | Umgebung                  |
| ----------- | ------------------------- |
| Grün        | Wald, Grasland, Sumpf     |
| Wasser      | Küste, Sumpf, Unterwasser |
| Trocken     | Wüste, Gebirge            |
| Kalt        | Gebirge, Arktisch         |
| Pilz        | Wald, Sumpf, Unterreich   |

## Effekte