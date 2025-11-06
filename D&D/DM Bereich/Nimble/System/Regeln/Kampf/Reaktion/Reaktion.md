---
aliases:
  - Reaktionen
---
# `=this.file.name`

Reaktionen kosten 1 Aktion und werden ausgeführt, wenn **nicht** dein Zug ist. Ein Held kann jede Reaktion höchstens 1× pro Runde einsetzen und beginnt seinen nächsten Zug dann mit entsprechend weniger Aktionen.

```dataview
TABLE WITHOUT ID

file.link AS "Reaktion"

FROM #Zug/Reaktion

SORT file.name
```