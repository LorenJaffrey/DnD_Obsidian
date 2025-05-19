|                               |                                                                                                                       |
| ----------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| [[Gnomisches Verschwinden#Verschwinden]] | `INPUT[toggle:InputData.Fähigkeiten.Verschwinden]`                                                                    |
| [[Hinterhältiger Angriff]]    | `$="```dice:" + dv.page(dv.current().Hintergrund.Klasse).HinterhältigerAngriff["Stufe"+dv.current().Stufe] + "d6```"` |

#### Apparaturen (max `=ceil(this.Stufe/2)`)
| Apparatur 1                                   | Apparatur 2                                   | Apparatur 3                                   |
| --------------------------------------------- | --------------------------------------------- | --------------------------------------------- |
| `INPUT[toggle:InputData.Apparaturen.Ladung1]` | `INPUT[toggle:InputData.Apparaturen.Ladung2]` | `INPUT[toggle:InputData.Apparaturen.Ladung3]` |
 
```dataview
TABLE WITHOUT ID
file.link AS "Apparaturen", 
SG,
Einsatz
FROM #Merkmal/Klasse/Schurke/Meistertüftler/Apparatur 
WHERE contains(this.Niptac.Apparaturen, file.link)
SORT SG, file.link
```