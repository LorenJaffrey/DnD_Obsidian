---
tags:
  - Gegenstand/Waffe/Art/Stichwaffe
  - Gegenstand/Waffe/Gruppe/Armbrust
  - Gegenstand/Waffe/Klasse/Fernkampfwaffe/Schusswaffe
  - Gegenstand/Waffe/Kategorie/Exotische_Waffe
  - Gegenstand/Waffe/Größe/Anderthalbhänder
  - Gegenstand/Magischer_Gegenstand/Waffe/Armbrust
Reichweite: 
Schaden: 
Schadensart: 
Eigenschaften: 
AngriffsbonusFern: 1
SchadenFern: 2d3+1
SchadensartFern: "[[Stichschaden]]"
Range1: 1,5(1)
Range2: 24(16)
Range3: 96(64)
EigenschaftenFern:
  - "[[Geschosse]] (Bolzen)"
  - "[[Rüstungsbrechend]] (1)"
  - "[[Repetiermechanismus]]"
  - "[[Angriffsbonus|Zielvorrichtung]] (1) (bereits eingerechnet)"
  - "[[Schadensbonus|Verstärkte Sehne]] (1) (bereits eingerechnet)"
Kategorie: "[[Exotische Waffen]]"
Hände: 2
Größe: 3
Gewicht: 10 Pfund
Kosten: 25 GM
Verfügbarkeit: gewöhnlich
---
## `=this.file.name`
> [!infobox]
> # `=this.file.name`
> ![[BIANKA.webp]]

Der "Ballistische Initiator mit Automatischer Nachlade Kampf Automatik", kurz B.I.A.N.K.A., ist bereits auf den ersten Blick eine beeindruckende technische Apparatur, die das Resultat gnomischer Ingenieurskunst verkörpert. 
Ihr Körper besteht aus seltenem Holz und leichtem, aber robustem Metall.
Die gesamte Konstruktion wirkt durchdacht und funktional, mit sichtbaren Zahnrädern und mechanischen Komponenten, die in einem harmonischen Design miteinander verbunden sind.

Das auffälligste Merkmal ist das integrierte Bolzenmagazin, das unten an der Armbrust angebracht ist und bis zu sechs Bolzen fasst. 
Es ist nicht nur funktional, sondern auch ein zentraler Bestandteil des Designs.
Die Bolzen sind durch ein Sichtfenster im Magazin gut sichtbar, was dem Schützen ermöglicht, jederzeit die verbleibende Munition im Auge zu behalten.

Die oberhalb der Armbrust angebrachte Zielvorrichtung ist eine präzise Linse, die die Schussgenauigkeit erheblich verbessert. 
Sie ist mechanisch verstellbar und passt sich den unterschiedlichen Bedingungen des Kampfes an. 

Die **B.I.A.N.K.A.** ist nicht nur eine Waffe, sondern auch ein Kunstwerk, das in jedem Detail das Streben nach technischer Perfektion widerspiegelt. 
Jeder, der sie in die Hand nimmt, spürt sofort die durchdachte Konstruktion und die Möglichkeit, mit dieser Apparatur das Blatt im Kampf zu wenden.

| Waffe             | Schaden             | Art                     |     Hände     |     Größe     | Min RW         | Gnd RW         | Max RW         | Eigenschaften             |
| ----------------- | ------------------- | ----------------------- |:-------------:|:-------------:| -------------- | -------------- | -------------- | ------------------------- |
| `=this.file.name` | `$="```dice:" + dv.current().SchadenFern + "```"` | `=this.SchadensartFern` | `=this.Hände` | `=this.Größe` | `=this.Range1` | `=this.Range2` | `=this.Range3` | `=this.EigenschaftenFern` |

## Handel

| Waffe             |         Gewicht | Kategorie         |
| ----------------- | ---------------:| ----------------- |
| `=this.file.name` | `=this.Gewicht` | `=this.Kategorie` |