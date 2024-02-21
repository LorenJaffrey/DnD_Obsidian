---
aliases:
tags:
- Merkmal/Klasse/Schurke/Meistertüftler
---
# `=this.file.name`

*Du lernst Apparaturen zu erschaffen die dir einen Vorteil im Kampf und außerhalb gewähren können.* 
Du lernst zwei Apparaturen herzustellen und vorzubereiten, die unter [[Meistertüftler#Apparaturen]] beschrieben sind. Einige dieser [[Meistertüftler#Apparaturen]] verstärken deinen [[Angriff]]. Du kannst nur eine einzelne [[Meistertüftler#Apparaturen]] pro [[Angriff]] einsetzen. 
Du kannst außerdem eine dir bekannte Apparatur durch eine andere ersetzen nachdem du eine [[Lange Rast]] beendet hast.

## Engergiekerne
Du besitzt 4 Engergiekerne, die W6 sind. Ein Engergiekerne wird nur bei einem erfolgreichen [[Attribute#Attributswurf]] oder [[Angriffswurf]] verbraucht, außer die [[Meistertüftler#Apparaturen]] besagt etwas anderes. Du regenerierst alle verbrauchten Engergiekerne wenn du eine [[Lange Rast]] beendest. Auf höheren Stufen erhältst du zusätzliche und größere Engergiekerne.

## Tüftlerwurf
Um eine [[Meistertüftler#Apparaturen]] zu benutzen ist ein Wurf auf [[Intelligenz]] gegen den [[Schwierigkeitsgrad]] der Apparatur notwendig. 
Eine Apparatur kann theoretisch von anderen Kreaturen benutzt werden, jedoch besitzen diese normalerweise keine [[Durchdachte Vorbereitung#Vorbereitungswürfel]] und [[Übung]] mit [[Tüftlerwerkzeug]], was die Benutzung erschwert.

>[!info]
>W20 + dein [[Übung|Übungsbonus]] für [[Tüftlerwerkzeug]] + dein [[Intelligenz#Intelligenzmodifikator]] + [[Durchdachte Vorbereitung#Vorbereitungswürfel]]

## Rettungswürfe
Manche deiner [[Meistertüftler#Apparaturen]] erfordern von deinem Ziel einen [[Rettungswurf]], um den Auswirkungen der [[Meistertüftler#Apparaturen]] zu widerstehen. Der [[Schwierigkeitsgrad]] des [[Rettungswurf]]s wird folgendermaßen berechnet:

>[!info]
>[[Schwierigkeitsgrad|SG]] für [[Rettungswurf]] gegen [[Meistertüftler#Apparaturen]] = 8 + dein [[Übung|Übungsbonus]] für [[Tüftlerwerkzeug]] + dein [[Intelligenz#Intelligenzmodifikator]]

## Apparaturen
```dataview
TABLE WITHOUT ID

file.link AS "Apparaturen", SG AS "Schwierigkeitsgrad"

FROM #Merkmal/Klasse/Schurke/Meistertüftler/Apparatur 

SORT SG, file.name
```