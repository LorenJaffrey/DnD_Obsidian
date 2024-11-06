---
tags:
  - Gegenstand/Waffe/Art/Wuchtwaffe
  - Gegenstand/Waffe/Gruppe/Stab
  - Gegenstand/Waffe/Klasse/Nahkampfwaffe
  - Gegenstand/Waffe/Kategorie/Einfache_Waffe
  - Gegenstand/Waffe/Größe/Großwaffe
  - Gegenstand/Magischer_Gegenstand/Zauberstecken
Art: "[[Zauberstecken]]"
Seltenheit: 
Einstimmung: true
Kosten: 
Voraussetzung:
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
> ###### Eigenschaften
> | Eigenschaft |  |
> | ---- | ---- |
> | Art | `=this.Art` |
> | Seltenheit | `=this.Seltenheit` |
> | Einstimmung | `=choice(this.Einstimmung, "Ja", "Nein")` |
> | Verflucht | `=choice(this.Verflucht, "Ja", "Nein")` |
> | Voraussetzung | `=this.Voraussetzung` |
> | Kosten | `=this.Kosten` |

Der schlanke, hohle [[Zauberstecken]] besteht aus Glas, ist aber so robust wie Eichenholz. 
Du musst auf den Stecken [[Einstimmung magischer Gegenstände|eingestimmt]] sein, um seine Vorteile zu nutzen und seine Zauber zu wirken.

## Rüstungsbonus
Solange du den Stecken hältst, erhältst du [[Rüstungsbonus]] (+1).

## Gespeicherte Zauber
Der Stecken hat 10 Ladungen, die genutzt werden können, um die Zauber in seinem Inneren zu wirken.
Es sind keine Komponenten notwendig.
Du musst Zauberwirker sein um diese Zauber einsetzen zu können.

Mit dem Stecken in Händen kannst du deine [[Aktion]] nutzen und eine Ladung verbrauchen um [[Magierrüstung]] zu wirken.
Alternativ kannst du deine [[Reaktion]] nutzen und zwei Ladungen verbrauchen um [[Schild]] zu wirken. 
 
Der Stecken erhält immer zur Morgendämmerung 1W6+4 verbrauchte Ladungen zurück. 
Wenn du die letzte Ladung des Steckens verbrauchst, wirf einen W20. 
Bei einer 1 zerbricht der Stecken und wird zerstört.

## Kampf
| Waffe             | Schaden         | Art                 |     Hände     |     Größe     | Eigenschaften         |
| ----------------- | --------------- | ------------------- |:-------------:|:-------------:| --------------------- |
| `=this.file.name` | `dice: Schaden` | `=this.Schadensart` | `=this.Hände` | `=this.Größe` | `=this.Eigenschaften` |

| Waffe             |         Gewicht | Kategorie         |
| ----------------- | ---------------:| ----------------- |
| `=this.file.name` | `=this.Gewicht` | `=this.Kategorie` |