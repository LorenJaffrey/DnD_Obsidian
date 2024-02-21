---
aliases:
  - Sprache
---
## Standardsprachen
```dataview
TABLE WITHOUT ID

file.link AS "Sprache", Typische_Völker, Schrift

FROM #Sprache/Standard 

SORT file.name
```

## Exotische Sprachen
```dataview
TABLE WITHOUT ID

file.link AS "Sprache", Typische_Völker, Schrift

FROM #Sprache/Exotisch 

SORT file.name
```

## Sonstige Sprachen
```dataview
TABLE WITHOUT ID

file.link AS "Sprache", Typische_Völker, Schrift

FROM #Sprache/Sonstige 

SORT file.name
```