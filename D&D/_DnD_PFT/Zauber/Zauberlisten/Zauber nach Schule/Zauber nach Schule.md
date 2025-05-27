---
aliases:
  - Schulen der Magie
---
# `=this.file.name`
Jeder Zauber gehört zu einer Schule der Magie. 
Sie helfen dabei, Zauber zu beschreiben, und haben keine eigenen Regeln. 
Andere Regeln können sich allerdings auf sie beziehen.

```dataview
TABLE WITHOUT ID

file.link AS "Schule der Magie",
Typische_Effekte AS "Typische Effekte"

FROM #Schule_der_Magie 

SORT file.name
```