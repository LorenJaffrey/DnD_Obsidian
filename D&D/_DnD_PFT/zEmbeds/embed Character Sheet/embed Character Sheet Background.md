## `=this.Hintergrund.Name`
 `="!" + this.Hintergrund.Bild`
```dynamic-embed
[[embed Character Sheet Healthbar]]
```
## Hintergrund
|                                                              |                                 |
| ------------------------------------------------------------ | ------------------------------- |
| Stufe                                                        | `=this.Stufe`                   | 
| [[Völker\|Volk]]                                             | `=this.Hintergrund.Volk`        |
| [[Klassen\|Klasse]]                                          | `=this.Hintergrund.Klasse`      |
| `$=dv.page(dv.current().Hintergrund.Klasse).Name_Subklassen` | `=this.Hintergrund.Subklasse`   |
| [[Gesinnung]]                                                | `=this.Hintergrund.Gesinnung`   |
| [[_Übersicht Hintergründe\|Hintergrund]]                     | `=this.Hintergrund.Hintergrund` |
 
## Aussehen
|                 |                                  |
| --------------- | -------------------------------- |
| Geschlecht      | `=this.Aussehen.Geschlecht`      |
| Alter           | `=this.Aussehen.Alter`           |
| Größenkategorie | `=this.Aussehen.Größenkategorie` |
| Größe           | `=this.Aussehen.Größe`           |
| Gewicht         | `=this.Aussehen.Gewicht`         |
| Augenfarbe      | `=this.Aussehen.Augenfarbe`      |
| Haarfarbe       | `=this.Aussehen.Haarfarbe`       |
| Hautfarbe       | `=this.Aussehen.Hautfarbe`       |

### Persönlichkeitsmerkmale 
`=this.Persönlichkeit.Persönlichkeitsmerkmale[0]`
`=this.Persönlichkeit.Persönlichkeitsmerkmale[1]`
`=this.Persönlichkeit.Persönlichkeitsmerkmale[2]`

### Ideale
`=this.Persönlichkeit.Ideale`

### Bindungen
`=this.Persönlichkeit.Bindungen`
 
### Makel
`=this.Persönlichkeit.Makel`