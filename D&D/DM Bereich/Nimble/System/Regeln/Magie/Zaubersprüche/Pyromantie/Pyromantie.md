# `=this.file.name`

```dataview
TABLE WITHOUT ID

file.link AS "Zauber",
Grad,
Zeitaufwand, 
Reichweite,
Schaden,
Dauer,
choice(Konzentration,"X","") AS "Konzentration" 

FROM #Zauber

WHERE contains(Schule, [[Feuerzauber]])

SORT file.name
```



Entzünden﻿  
Grad-1-Feuerzauber﻿  
2 Aktionen | Einzelziel | Reichweite 8  
Schaden: 4w10 an ein Versengt﻿-Ziel, beendet die Bedingung beim Treffer.  
Erhöht gewirkt: +10 Schaden.

Waffe verzaubern﻿  
Grad-2-Feuerzauber﻿  
1 Aktion | Einzelziel  
Konzentration: Bis zu 1 Minute.  
Effekt: Eine Waffe, die du berührst, wird mit magischer Flamme verzaubert.  
Sie verursacht +SCHLÜSSEL﻿ Schaden und verursacht bei Krit Versengt﻿.  
Erhöht gewirkt: +SCHLÜSSEL﻿ Schaden.

Flammenbarriere﻿  
Grad-3-Feuerzauber﻿  
1 Aktion | Selbst  
Reaktion: Wenn du angegriffen wirst, verteidige dich kostenlos.  
Bis zum Beginn deines nächsten Zuges nehmen Nahkampfangreifer gegen dich SCHLÜSSEL﻿ Schaden (Rüstung ignoriert) und erhalten Versengt﻿.  
Erhöht gewirkt: +SCHLÜSSEL﻿ Schaden.

Pyroklasm﻿  
Grad-4-Feuerzauber﻿  
2 Aktionen | AoE | Reichweite 3  
Effekt: Andere innerhalb der Reichweite erhalten 2w20+10 Schaden (Rüstung ignoriert) bei misslungenem GE-Wurf.  
Halber Schaden beim Gelingen. Versengt﻿-Kreaturen scheitern automatisch.  
Erhöht gewirkt: +1 Reichweite, +2 Schaden.

Feurige Umarmung﻿  
Grad-5-Feuerzauber﻿  
2 Aktionen | AoE | Reichweite 8  
Konzentration: Bis zu 1 Minute.  
Effekt: Während innerhalb der Reichweite: 1 Verbündeter erhält die Effekte von Waffe verzaubern﻿.  
Feinde erlangen Versengt﻿, verlieren Schadensresistenz und ihre Immunität wird auf Resistenz reduziert.  
Erhöht gewirkt: +1 Verbündeter.

Lebender Inferno﻿  
Grad-7-Feuerzauber﻿  
3 Aktionen | Selbst  
Effekt: Du erhältst die Effekte von Flammenbarriere﻿ bis zu deinem nächsten Zug.  
Am Ende dieses und deines nächsten Zuges, wirke Pyroklasm﻿ kostenlos.  
Erhöht gewirkt: Flammenbarriere﻿ und Pyroklasm﻿ werden erhöht gewirkt.

Drachenform﻿  
Grad-9-Feuerzauber﻿  
5 Aktionen | Selbst  
Effekt: Verwandle dich in einen riesigen Drachen.  
Erhalte 3 Aktionen, Fluggeschwindigkeit 12, STUFE﻿ Rüstung, 10×STUFE﻿ temporäre TP und:  
Zahn & Kralle. Aktion:﻿ (Reichweite 2) 1w20+STUFE﻿ Schaden (Rüstung ignoriert). Verursacht Versengt﻿.  
Flammender Atem. 2 Aktionen:﻿ (Kegel 8). GE-Rettungswurf 20, SCHLÜSSEL﻿ w20 Schaden, halber Schaden bei Gelingen. Versengt﻿-Ziele scheitern automatisch.  
Du behältst diese Form, solange die durch diesen Zauber gewährten temporären TP bestehen (max. 10 Minuten). Endet sie, fällst du auf 0 TP.