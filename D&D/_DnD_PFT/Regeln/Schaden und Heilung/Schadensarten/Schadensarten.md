---
aliases:
  - Schadensart
---
# `=this.file.name`

| Schadensart              | Zustand ?          | Effekt                                         | Dauer      | Beenden                     |
| ------------------------ | ------------------ | ---------------------------------------------- | ---------- | --------------------------- |
| [[Wuchtschaden]]         | [[Benommen]]       | Geschicklichkeit, Rüstung                      |            | KO RW                       |
| [[Hiebschaden]]          | [[Bluten]]         | geringer Zusatzschaden, schwerer abzuschütteln | Dauerhaft  | Heilung oder schwerer KO-RW |
| [[Stichschaden]]         | [[Erschöpft]]      | Erschöpfung                                    | Dauerhaft  | Lange Rast                  |
| [[Energieschaden]]       | [[Liegend]]        | Umwerfen                                       | Dauerhaft  | Aufstehen                   |
| [[Feuerschaden]]         | [[Brennend]]       | hoher Zusatzschaden, leicht abzuschütteln      | 1W4 Runden | Aktion                      |
| [[Kälteschaden]]         | [[Verlangsamt]]    | Geschicklichkeit, Verlangsamend                | 1W4 Runden | KO RW                       |
| [[Blitzschaden]]         | [[Elektrifiziert]] | Überspringen                                   |            | KO RW                       |
| [[Schallschaden]]        | [[Taub]]           | Taub                                           |            | KO RW                       |
| [[Giftschaden]]          | [[Vergiftet]]      | Konstitution                                   |            | KO RW                       |
| [[Säureschaden]]         | [[Verätzt]]        | Schlechtere Rüstung                            |            | Reparieren                  |
| [[Psychischer Schaden]]  | [[Verängstigt]]    | Angst                                          |            | WE RW                       |
| [[Nekrotischer Schaden]] | [[Nekrotisiert]]   | Keine Heilung                                  |            | KO RW                       |
| [[Gleißender Schaden]]   | [[Blind]]          | Blind                                          |            | KO RW                       |

```dataview
TABLE WITHOUT ID

file.link AS "Schadensart"

FROM #Schadensart

SORT file.name
```

## Schadensanfälligkeit
Wenn eine Kreatur [[Schadensarten#Schadensanfälligkeit]] gegen eine bestimmte [[Schadensarten|Schadensart]] besitzt, wird der erlittene Schaden verdoppelt.

## Schadensimmunität
Wenn eine Kreatur [[Schadensarten#Schadensimmunität]] gegen eine bestimmte [[Schadensarten|Schadensart]] besitzt, wird der erlittene Schaden ignoriert.

## Schadensresistenz
Wenn eine Kreatur [[Schadensarten#Schadensresistenz]] gegen eine bestimmte [[Schadensarten|Schadensart]] besitzt, wird der erlittene Schaden halbiert (abgerundet).