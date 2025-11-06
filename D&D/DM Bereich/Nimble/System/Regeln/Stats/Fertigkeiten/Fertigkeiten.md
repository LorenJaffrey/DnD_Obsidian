---
aliases:
  - Fertigkeit
---
# `=this.file.name`
Jede Fertigkeit hat ein zugeordnetes [[Attribute|Attribut]], dessen [[Attribute|Attributswert]] für einen [[Fertigkeiten#Fertigkeitswurf]] herangezogen wird. 
Ein [[Fertigkeiten#Fertigkeitswurf]] stellt eine konkretere Art von [[Attribute#Attributswurf]] dar und profitiert von einem eventuellen Bonus des Anwenders in dieser Fertigkeit.

```dataview
TABLE attribut AS "Attribut"
FROM #Fertigkeit
SORT attribut, file.name
```

## Fertigkeitswurf
>[!info]
>W20 + [[Attribute|Attributswert]] + Bonus/Malus

Für Fertigkeitswürfe gelten ansonsten die selben Regeln wie für [[Attribute#Attributswurf|Attributswürfe]].