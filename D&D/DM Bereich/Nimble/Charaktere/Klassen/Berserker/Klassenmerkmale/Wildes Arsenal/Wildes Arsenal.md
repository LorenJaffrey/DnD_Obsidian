# `=this.file.name`
Wähle 1 Fähigkeit aus dem Wilden Arsenal:

> [!tip]- Zorn & Zerstörung  
> Wann immer du während einer [[Sichere Rast|Sicheren Rast]] eine bemerkenswerte Tat der Zerstörung oder Stärke vollbringst, kannst du deine verfügbaren Berserker-Optionen neu wählen.

```dataview
TABLE WITHOUT ID

file.link AS "Title",
Einsatz

FROM #Regeln/Nimble/Merkmal/Klasse/Berserker/Wildes_Arsenal

SORT file.name
```