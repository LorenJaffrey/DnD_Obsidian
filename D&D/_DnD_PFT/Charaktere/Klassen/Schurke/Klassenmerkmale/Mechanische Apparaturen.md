---
aliases:
tags:
- Merkmal/Klasse/Schurke/Meistertüftler
---
# `=this.file.name`
Als gnomischer Tüftler stellst du hochspezialisierte Apparaturen her, die mächtige Effekte erzielen können, aber nicht immer zuverlässig funktionieren. 
Du kannst eine Anzahl von [[Apparaturen]] herstellen, die der Hälfte deiner Stufe als [[Schurke]] entspricht (aufgerundet).
Jede [[Apparaturen|Apparatur]] kann einmal pro[[Lange Rast|Langer Rast]] verwendet werden.
Zu Beginn jeder [[Lange Rast|Langen Rast]] kannst du [[Apparaturen]] herstellen. 
Diese [[Apparaturen]] halten bis zur nächsten [[Lange Rast|Langen Rast]] und werden dann unbrauchbar.

## Tüftlerwurf
Um eine [[Apparaturen|Apparatur]] zu aktivieren, musst du einen **Tüftlerwurf** gegen einen festgelegten Schwierigkeitsgrad bestehen.
Jede [[Apparaturen|Apparatur]] hat einen eigenen [[Schwierigkeitsgrad]] basierend auf ihrer Effektivität. 
Bei einem [[Misserfolg]] tritt ein Fehlzündungs-Effekt auf, der bei der jeweiligen [[Apparaturen|Apparatur]] vermerkt ist.

>[!info] Tüftlerwurf
>W20 + dein [[Übung|Übungsbonus]] für [[Tüftlerwerkzeug]] + dein [[Intelligenz#Intelligenzmodifikator]]

## Apparatur-SG
Manche deiner [[Apparaturen]] erfordern von deinem Ziel einen [[Rettungswurf]], um den Auswirkungen der [[Apparaturen]] zu widerstehen. 
Der [[Schwierigkeitsgrad]] des [[Rettungswurf|Rettungswurfs]] wird folgendermaßen berechnet:

>[!info] Apparatur-SG
>8 + dein [[Übung|Übungsbonus]] für [[Tüftlerwerkzeug]] + dein [[Intelligenz#Intelligenzmodifikator]]

## Apparaturen
```dataview
TABLE WITHOUT ID

file.link AS "Apparaturen", 
SG,
Stufe,
Einsatz

FROM #Merkmal/Klasse/Schurke/Meistertüftler/Apparatur 

SORT SG, file.name
```