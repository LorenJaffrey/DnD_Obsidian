---
tags: 
  - Regeln/PHB2024
aliases:
  - Schadensart
---
# `=this.file.name`

```dataview
TABLE WITHOUT ID

file.link AS "Schadensart",
Zustand

FROM #Schadensart

SORT file.name
```

## Schadensanfälligkeit
Wenn eine Kreatur [[Schadensarten#Schadensanfälligkeit]] gegen eine bestimmte [[Schadensarten|Schadensart]] besitzt, wird der erlittene Schaden verdoppelt.

## Schadensimmunität
Wenn eine Kreatur [[Schadensarten#Schadensimmunität]] gegen eine bestimmte [[Schadensarten|Schadensart]] besitzt, wird der erlittene Schaden ignoriert.

## Schadensresistenz
Wenn eine Kreatur [[Schadensarten#Schadensresistenz]] gegen eine bestimmte [[Schadensarten|Schadensart]] besitzt, wird der erlittene Schaden halbiert (abgerundet).

## Anwendungsreihenfolge
Schadensmodifikatoren werden in folgender Reihenfolge angewendet: zuerst Anpassungen wie Boni, Mali und Multiplikatoren, dann Resistenzen, als Drittes Anfälligkeiten.

>[!Example] Beispiel
>Eine Kreatur ist gegen alle Schadensarten resistent, anfällig für Feuerschaden, und sie befindet sich innerhalb einer magischen Aura, die jeden Schaden um 5 verringert. 
>Wenn diese Kreatur 28 Feuerschaden erleidet, wird der Schaden zuerst um 5 verringert (auf 23), dann aufgrund der Resistenz halbiert (und auf 11 abgerundet) und zum Schluss aufgrund der Anfälligkeit verdoppelt (auf 22).