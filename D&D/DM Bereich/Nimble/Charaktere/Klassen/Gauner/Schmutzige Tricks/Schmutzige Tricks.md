# `=this.file.name`
Wähle 1 Fähigkeit aus den [[Schmutzige Tricks|Schmutzigen Tricks]]:

> [!tip]- Geschäftsgeheimnisse  
> Verbringst du während einer sicheren Rast eine Nacht damit, mit anderem zwielichtigen Gesindel „Fachgespräche“ zu führen, kannst du deine verfügbaren Schummler‑Optionen neu wählen.

```dataview
TABLE WITHOUT ID

file.link AS "Title",
Einsatz

FROM #Regeln/Nimble/Merkmal/Klasse/Gauner/Schmutzige_Tricks

SORT file.name
```