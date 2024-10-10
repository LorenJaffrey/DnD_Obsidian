---
aliases:
  - Schadensart
---
# `=this.file.name`

| Schadensart              | Zustand ?          | Effekt                                         | Dauer | Beenden |
| ------------------------ | ------------------ | ---------------------------------------------- | ----- | ------- |
| [[Wuchtschaden]]         | [[Benommen]]       | Benommenheit                                   |       | KO RW   |
| [[Hiebschaden]]          | [[Bluten]]         | geringer Zusatzschaden, schwerer abzuschütteln |       | KO RW   |
| [[Stichschaden]]         | [[Erschöpft]]      | Erschöpfung                                    |       | -       |
| [[Energieschaden]]       | [[Liegend]]        | Umwerfen                                       |       | -       |
| [[Feuerschaden]]         | [[Brennend]]       | hoher Zusatzschaden, leicht abzuschütteln      |       | -       |
| [[Kälteschaden]]         | [[Gefroren]]       | Verlangsamend                                  |       | KO RW   |
| [[Blitzschaden]]         | [[Elektrifiziert]] | keine Reaktion                                 |       | KO RW   |
| [[Schallschaden]]        | [[Taub]]           | Taub + ?                                       |       | KO RW   |
| [[Giftschaden]]          | [[Vergiftet]]      | Nachteil auf Attributs- und Angriffswürfe      |       | KO RW   |
| [[Säureschaden]]         | [[Säurebespritzt]] | Schlechtere Rüstung                            |       | -       |
| [[Psychischer Schaden]]  | [[Verängstigt]]    | Angst                                          |       | WE RW   |
| [[Nekrotischer Schaden]] |                    | Keine Heilung                                  |       | KO RW   |
| [[Gleißender Schaden]]   |                    | Blind                                          |       | KO RW   |

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