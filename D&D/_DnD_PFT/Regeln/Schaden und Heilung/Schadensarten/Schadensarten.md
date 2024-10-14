---
aliases:
  - Schadensart
---
# `=this.file.name`

| Schadensart              | Zustand ?          | Effekt                                         | Dauer     | Beenden                     |
| ------------------------ | ------------------ | ---------------------------------------------- | --------- | --------------------------- |
| [[Wuchtschaden]]         | [[Benommen]]       | Geschicklichkeit, Rüstung                      | 3 Runden  | KO RW                       |
| [[Hiebschaden]]          | [[Bluten]]         | geringer Zusatzschaden, schwerer abzuschütteln | Dauerhaft | Heilung oder schwerer KO-RW |
| [[Stichschaden]]         | [[Erschöpft]]      | Erschöpfung                                    | Dauerhaft | Lange Rast                  |
| [[Energieschaden]]       | [[Liegend]]        | Umwerfen                                       | Dauerhaft | Aufstehen                   |
| [[Feuerschaden]]         | [[Brennend]]       | hoher Zusatzschaden, leicht abzuschütteln      | Dauerhaft | Aktion                      |
| [[Kälteschaden]]         | [[Verlangsamt]]    | Geschicklichkeit, Verlangsamend                | 3 Runden  | KO RW                       |
| [[Blitzschaden]]         | [[Elektrifiziert]] | Überspringen                                   | 3 Runden  | KO RW                       |
| [[Schallschaden]]        | [[Taub]]           | Taub                                           | 3 Runden  | KO RW                       |
| [[Giftschaden]]          | [[Vergiftet]]      | Konstitution                                   | Dauerhaft | KO RW                       |
| [[Säureschaden]]         | [[Verätzt]]        | Schlechtere Rüstung                            | Dauerhaft | Reparieren                  |
| [[Psychischer Schaden]]  | [[Verängstigt]]    | Angst                                          | Dauerhaft | WE RW                       |
| [[Nekrotischer Schaden]] | [[Nekrotisiert]]   | Keine Heilung                                  | Dauerhaft | KO RW                       |
| [[Gleißender Schaden]]   | [[Blind]]          | Blind                                          | 3 Runden  | KO RW                       |

```dataview
TABLE WITHOUT ID

file.link AS "Schadensart",
Zustand,
Dauer

FROM #Schadensart

SORT file.name
```

## Schadensanfälligkeit
Wenn eine Kreatur [[Schadensarten#Schadensanfälligkeit]] gegen eine bestimmte [[Schadensarten|Schadensart]] besitzt, wird der erlittene Schaden verdoppelt.

## Schadensimmunität
Wenn eine Kreatur [[Schadensarten#Schadensimmunität]] gegen eine bestimmte [[Schadensarten|Schadensart]] besitzt, wird der erlittene Schaden ignoriert.

## Schadensresistenz
Wenn eine Kreatur [[Schadensarten#Schadensresistenz]] gegen eine bestimmte [[Schadensarten|Schadensart]] besitzt, wird der erlittene Schaden halbiert (abgerundet).