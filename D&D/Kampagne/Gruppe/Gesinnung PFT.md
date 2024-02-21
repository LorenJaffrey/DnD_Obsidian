# `=this.file.name`

``` dataview
TABLE Ordnung, Moral
FROM #Charakter/PFT 
SORT file.name
```

---

| Charakter | Ordnung | Moral | Ordnung | Moral |
| --------- |:-------:|:-----:|:-------:|:-----:|
| Aranon    |    3    |   3   |   0.8   |  0.8  |
| Drogan    |    2    |   4   |   0.7   |  0.9  |
| Jon       |    4    |   1   |   0.9   |  0.6  |
| Lucian    |   -3    |  -1   |   0.2   |  0.4  |
| Niptac    |   -2    |   1   |   0.3   |  0.6  |
<!-- TBLFM: $4=(($-2+5)/10) -->
<!-- TBLFM: $5=(($-2+5)/10) -->

---

|            | -4 Chaotisch | -3 Chaotisch | -2 Chaotisch | -1 Neutral | 0 Neutral | 1 Neutral | 2 Rechtschaffen | 3 Rechtschaffen | 4 Rechtschaffen |
|:----------:|:------------:|:------------:|:------------:|:----------:|:---------:|:---------:|:---------------:|:---------------:|:---------------:|
|   4 Gut    |              |              |              |            |           |           |     Drogan      |                 |                 |
|   3 Gut    |              |              |              |            |           |           |                 |     Aranon      |                 |
|   2 Gut    |              |              |              |            |           |           |                 |                 |                 |
| 1 Neutral  |              |              |    Niptac    |            |           |           |                 |                 |       Jon       |
| 0 Neutral  |              |              |              |            |           |           |                 |                 |                 |
| -1 Neutral |              |    Lucian    |              |            |           |           |                 |                 |                 |
|  -2 Böse   |              |              |              |            |           |           |                 |                 |                 |
|  -3 Böse   |              |              |              |            |           |           |                 |                 |                 |
|  -4 Böse   |              |              |              |            |           |           |                 |                 |                 |

---

``` mermaid
%%{init: {"quadrantChart": {"chartWidth": 400, "chartHeight": 400}, "themeVariables": {"quadrant1Fill": "#000000", "quadrant2Fill": "#000000", "quadrant3Fill": "#000000", "quadrant4Fill": "#000000"} }}%%
quadrantChart
    title Gesinnung PFT
    x-axis Chaotisch --> Rechtschaffen
    y-axis Boese --> Gut
    quadrant-1 Rechtschaffen Gut
    quadrant-2 Chaotisch Gut
    quadrant-3 Chaotisch Boese
    quadrant-4 Rechtschaffen Boese
    Aranon: [0.8, 0.8]
    Drogan: [0.7, 1]
    Jon: [0.9, 0.6]
    Lucian: [0.2, 0.4]
    Niptac: [0.3, 0.6]
```