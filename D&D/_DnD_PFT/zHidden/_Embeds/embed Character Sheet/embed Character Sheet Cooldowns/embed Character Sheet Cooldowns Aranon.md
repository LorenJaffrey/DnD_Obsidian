|                    | Maximal                                                                                   | Aufladung      |
| ------------------ | ----------------------------------------------------------------------------------------- | -------------- |
| [[Tiergestalt]]    | `INPUT[toggle:InputData.TiergestaltLadung1]` `INPUT[toggle:InputData.TiergestaltLadung2]` | [[Kurze Rast]] |
| [[Geistertotem]]   | `INPUT[toggle:InputData.GeistertotemLadung]`                                              | [[Kurze Rast]] |
| [[Nebelschritt]]   | `INPUT[toggle:InputData.NebelschrittLadung]`                                              | [[Lange Rast]] |
| [[Identifizieren]] | `INPUT[toggle:InputData.IdentifizierenLadung]`                                            | [[Lange Rast]] |

#### Tiergestalten
 ```dataview
TABLE WITHOUT ID
file.link AS "Tier",
HG
FROM #Kreatur/Tier 
SORT HG DESC
WHERE HG = "1/4" OR HG = "1/8" OR HG = 0
```