---
aliases: 
tags:
  - Merkmal/Klasse/Schurke
  - Regeln/PHB2024
Einsatz: Passiv
---
# `=this.file.name`
Du hast raffinierte Methoden entwickelt, deinen [[Hinterhältiger Angriff|Hinterhältigen Angriff]] einzusetzen.
Wenn du mit diesem Schaden bewirkst, kannst du **EINEN** der folgenden Effekte von [[Raffinierter Schlag]] hinzufügen. 
Jeder Effekt hat Würfelkosten in Form der Schadenswürfel für [[Hinterhältiger Angriff]], auf die du verzichten musst, um den Effekt hinzuzufügen. 
Du musst diese Würfel vor dem Wurf entfernen, und der Effekt tritt auf, sobald der Schaden des Angriffs bewirkt wurde. 

>[!example] Beispiel
>Wenn du den Gift-Effekt hinzufügst, entfernst du 1W6 von den Schadenswürfeln des [[Hinterhältiger Angriff|Hinterhältigen Angriffs]], bevor du würfelst.

Wenn ein Effekt von Raffinierter Schlag einen [[Rettungswurf]] erfordert, entspricht der [[Schwierigkeitsgrad|SG]] 8 plus deinem [[Geschicklichkeit#Geschicklichkeitsmodifikator]] plus deinem [[Übung|Übungsbonus]].

```dataview
TABLE WITHOUT ID

file.link AS "Raffinierter Schlag",
Kosten

FROM #Merkmal/Klasse/Schurke/Raffinierter_Schlag

WHERE Stufe < 14

SORT file.name
```