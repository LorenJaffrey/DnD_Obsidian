---
aliases:
  - Fertigkeit
---
# `=this.file.name`
Jede Fertigkeit hat ein zugeordnetes [[Attribute|Attribut]], dessen [[Attribute#Attributsmodifikator]] für einen [[Fertigkeiten#Fertigkeitswurf]] herangezogen wird. 
Ein [[Fertigkeiten#Fertigkeitswurf]] stellt eine konkretere Art von [[Attribute#Attributswurf]] dar und profitiert von einem eventuellen [[Übung|Übungsbonus]] des Anwenders in dieser Fertigkeit.

```dataview
TABLE attribut AS "Attribut"
FROM #Fertigkeit
SORT attribut, file.name
```

## Fertigkeitswurf
>[!info]
>W20 + [[Attribute#Attributsmodifikator]] + [[Übung|Übungsbonus]] + Bonus/Malus

### Kombinierte Würfe
Kombinieren von mehreren [[Fertigkeiten]] oder [[Attribute|Attributen]] um eine Aufgabe zu ermöglichen bzw. zu vereinfachen
	- herausfinden wie ein Schloss, eine Falle, etc. funktioniert bevor man sich daran macht zu knacken oder entschärfen
	- schwächste Stelle in einer Wand finden bevor man versucht sie einzuschlagen

### Zeitfaktor
Bei gewissen [[Attribute#Attributswurf]] oder [[Fertigkeiten#Fertigkeitswurf]] kann Zeit einen Einfluss haben
	- ein Buch überfliegen oder es gründlich studieren
	- einen Raum kurz absuchen oder gründlich durchsuchen
	- eine Hängebrücke vorsichtig überqueren oder drüber rennen
- kann den Wurf erleichtern bzw. erschweren und oder [[Vorteil und Nachteil|Vorteil]]/[[Vorteil und Nachteil|Nachteil]] verleihen