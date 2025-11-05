---
tags:
  - Regeln/PHB2024
aliases:
  - Deckungen
---
# `=this.file.name`
Wände, Bäume, Kreaturen und andere Hindernisse können [[Deckung]] bieten und es damit schwieriger machen, ein Ziel zu treffen. 
Es gibt es drei Deckungsgrade, von denen jeder dem Ziel einen anderen Vorzug verschafft.
Eine [[Deckung]] ist nur wirksam, wenn der [[Angriff]] oder Effekt von der gegenüberliegenden Seite der Deckung kommt. 
Befindet sich das Ziel hinter mehreren [[Deckung|Deckungen]], zählt nur die wirksamste [[Deckung]]. 
Die Deckungen addieren sich nicht. 

>[!Example] Beispiel
>Steht ein Ziel hinter einer Kreatur, die Teildeckung gibt, sowie gleichzeitig hinter einem Baum, der Dreivierteldeckung gibt, verfügt das Ziel über Dreivierteldeckung.

```dataview
TABLE WITHOUT ID

file.link AS "Deckung",
Vorzug,
Beispiel

FROM #Deckung

SORT file.name
```