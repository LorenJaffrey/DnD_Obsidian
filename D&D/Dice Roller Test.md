---
Schaden: 2d6+1d4+5
Bonus: 1
---
## Zusammengesetzt aus DataView JS
```dataviewjs
dv.span("`dice:" + dv.current().Schaden + "+" + dv.current().Bonus + "|none`")
```

`$="```dice:" + dv.current().Schaden + "+" + dv.current().Bonus + "```"`

## Kombiniere unterschiedliche Würfel und Modifikatoren
`dice:2d6+1d4+5`

## Metadaten
`dice: Schaden`
--> nur erste Würfel

## Vorteil
`dice:2d20k`

## Exploding Crits
`dice:1d6!i` --> einzeln nacheinander
`dice:1d6!!i`