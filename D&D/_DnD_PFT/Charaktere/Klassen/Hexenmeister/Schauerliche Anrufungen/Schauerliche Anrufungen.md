---
aliases:
  - Schauerliche Anrufung
  - Anrufung
  - Anrufungen
tags:
  - Merkmal/Klasse/Hexenmeister
  - Regeln/PHB2024
---
# `=this.file.name`
Du bist auf [[Schauerliche Anrufungen]] gestoßen, auf verbotenes Wissen, das dich mit einem dauerhaften magischen Attribut oder anderen Lektionen versehen hat.
Du erhältst eine [[Schauerliche Anrufungen|Anrufung]] deiner Wahl, beispielsweise [[Pakt des Buches]]. 

## Voraussetzungen
Wenn eine [[Schauerliche Anrufungen|Anrufung]] eine Voraussetzung hat, musst du diese erfüllen, um die Anrufung zu erlernen. 

>[!example] Beispiel
>Wenn eine [[Schauerliche Anrufungen|Anrufung]] erfordert, dass du ein Hexenmeister ab der 5. Stufe bist, kannst du diese Anrufung erst auswählen, wenn du die 5. Hexenmeisterstufe erreicht hast.

## Anrufungen erlangen und ersetzen
Wann immer du eine Hexenmeisterstufe erhältst, kannst du eine deiner [[Schauerliche Anrufungen|Anrufungen]] durch eine andere ersetzen, für die du qualifiziert bist. 
Du kannst eine [[Schauerliche Anrufungen|Anrufung]] nicht ersetzen, wenn sie die Voraussetzung für eine andere [[Schauerliche Anrufungen|Anrufung]] ist, über die du verfügst.

Wenn du bestimmte Hexenmeisterstufen erreichst, erhältst du weitere [[Schauerliche Anrufungen|Anrufungen]] deiner Wahl, wie in der Spalte „Bekannte Anrufungen" in der [[Hexenmeister#Klassentabelle]] dargestellt.

Du kannst eine [[Schauerliche Anrufungen|Anrufung]] nicht mehrfach auswählen, sofern in ihrer Beschreibung nicht anders angegeben.

## Liste der Schauerlichen Anrufungen
```dataview
TABLE WITHOUT ID

file.link AS "Anrufung",
Voraussetzung, 
Mindeststufe

FROM #Merkmal/Klasse/Hexenmeister/Schauerliche_Anrufung

SORT mindeststufe, file.name ASC
```