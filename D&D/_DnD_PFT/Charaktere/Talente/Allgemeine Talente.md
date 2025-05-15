---
aliases:
tags:
Voraussetzungen:
Stufe:
Wiederholbar:
---
# `=this.file.name`

> [!infobox]
> |                                           |                                                             |
> | ------------------------ | ---------------------------------- |
> | Voraussetzungen   | `=this.Voraussetzungen` |
> | Stufe                              | `=this.Stufe`                           |
> | Mehrfach wählbar | `=this.Wiederholbar`         |

*Flavour Text*

## Attributswerterhöhung
Erhöhe deine [[Stärke]] oder [[Geschicklichkeit]] um 1 Punkt, bis zu einem maximalen Attributswert von 20.

## Weiterer Bonus
Du bist zäh wie Leder. Mit der Wahl dieses Talents erhöht sich dein [[Trefferpunktemaximum]] einmalig um das Doppelte deiner Stufe. Immer wenn du danach eine Stufe aufsteigst, erhöht sich dein [[Trefferpunkte]]maximum um weitere 2 Punkte.

```dataview
TABLE WITHOUT ID 
file.link AS "Talent", Stufe, Voraussetzungen, choice(Wiederholbar,"X","") AS "Wiederholbar", aliases AS "Alias"
FROM #Talent
WHERE Kategorie = "Allgemein"
SORT Stufe, file.name ASC
```