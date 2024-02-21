---
aliases: Fertigkeit
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

### Erfolgsgrad

| Erfolgsgrad           | Würfelwurf       | Effekt                                                               |
| --------------------- | ---------------- | -------------------------------------------------------------------- |
| einfacher Erfolg      | max. 5 über SG   | Erfolg                                                               |
| doppelter Erfolg      | max. 10 über SG  | Erfolg, kleiner positiver Effekt                                     |
| dreifacher Erfolg     | max. 15 über SG  | Erfolg, großer positiver Effekt                                      |
| Kritischer Erfolg     | natürliche 20    | Erfolg, kritischer positiver Effekt                                  |
| einfacher Misserfolg  | max. 5 unter SG  | Misserfolg, Wiederholungswurf möglich                                |
| doppelter Misserfolg  | max. 10 unter SG | Misserfolg, kein Wiederholungswurf möglich                           |
| dreifacher Misserfolg | max. 15 unter SG | Misserfolg, kein Wiederholungswurf möglich, kleiner negativer Effekt |
| kritischer Misserfolg | natürliche 1     | Misserfolg, kein Wiederholungswurf möglich, großer negativer Effekt  |

### Kombinierte Würfe
Kombinieren von mehreren [[Fertigkeiten]] oder [[Attribute]]n um eine Aufgabe zu ermöglichen bzw. zu vereinfachen
	- herausfinden wie ein Schloss, eine Falle, etc. funktioniert bevor man sich daran macht zu knacken oder entschärfen
	- schwächste Stelle in einer Wand finden bevor man versucht sie einzuschlagen

### Zeitfaktor
Bei gewissen [[Attribute#Attributswurf]] oder [[Fertigkeiten#Fertigkeitswurf]] kann Zeit einen Einfluss haben
	- ein Buch überfliegen oder es gründlich studieren
	- einen Raum kurz absuchen oder gründlich durchsuchen
	- eine Hängebrücke vorsichtig überqueren oder drüber rennen
- kann den Wurf erleichtern bzw. erschweren und oder [[Vorteil und Nachteil|Vorteil]]/[[Vorteil und Nachteil|Nachteil]] verleihen