---
tags:
  - Gegenstand/Waffe/Art/Wuchtwaffe
  - Gegenstand/Waffe/Gruppe/Stab
  - Gegenstand/Waffe/Klasse/Nahkampfwaffe
  - Gegenstand/Waffe/Kategorie/Einfache_Waffe
  - Gegenstand/Waffe/Größe/Großwaffe
  - Gegenstand/Magischer_Gegenstand/Zauberstecken
Art: "[[Zauberstecken]]"
Seltenheit: Erbstück
Einstimmung: true
Kosten: 
Voraussetzung:
  - "[[Druide]]"
Verflucht: false
Reichweite: 1,5(1)
Schaden: 1d8
Schadensart: "[[Wuchtschaden]]"
Eigenschaften:
  - "[[Parieren]]"
  - "[[Finesse]]"
Kategorie: "[[Einfache Waffen]]"
Hände: 2
Größe: 4
Gewicht: 3 Pfund
---
# `=this.file.name`

> [!infobox]
> # `=this.file.name`
> ![[summerwood_staff.png]]
> ###### Eigenschaften
> | Eigenschaft |  |
> | ---- | ---- |
> | Art | `=this.Art` |
> | Seltenheit | `=this.Seltenheit` |
> | Einstimmung | `=choice(this.Einstimmung, "Ja", "Nein")` |
> | Verflucht | `=choice(this.Verflucht, "Ja", "Nein")` |
> | Voraussetzung | `=this.Voraussetzung` |
> | Kosten | `=this.Kosten` |

Dieser [[Zauberstecken]] gehörte einst dem Erzdruiden [[Lirian Grauwald]].
Er kann als magischer [[Kampfstab]] eingesetzt werden.
Außerdem kann er als [[Druidischer Fokus]] genutzt werden und besitzt eine schwache magische Aura der Natur.

```dynamic-embed
[[embed Waffe Nahkampf]]
```