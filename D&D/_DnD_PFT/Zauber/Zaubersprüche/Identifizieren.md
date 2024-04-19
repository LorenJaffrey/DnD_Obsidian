---
aliases: 
- Identify
tags: 
- Zauber
Grad: 1
Schule: "[[Erkenntniszauber|Erkenntnismagie]]"
Zeitaufwand: 1m
Reichweite: Berührung
Verbal: true
Geste: true
Material: true
Materialkosten: eine Perle im Wert von mindestens 100 GM und eine Eulenfeder
Dauer: unmittelbar
Konzentration: false
Ritual: true
Skalierbar: false
Klassen:
- "[[Barde]]"
- "[[Magier]]"
- "[[Magieschmied]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du wählst einen Gegenstand, den du berühren musst, während du den Zauber wirkst. 
Handelt es sich um einen magischen Gegenstand oder ein anderweitig mit Magie erfülltes Objekt, würfle einen W20, addiere deinen [[Attribute#Attributsmodifikator]] zum Zauberwirken und vergleiche das Ergebnis mit der folgenden Tabelle. Wenn du [[Übung]] in [[Arkane Kunde]] hast, erhältst du [[Vorteil und Nachteil|Vorteil]] auf den Wurf. 

![[Identifikation magischer Gegenstände#Magische Gegenstände Seltenheit SG]]

Bist du erfolgreich erfährst du, welche Eigenschaften es hat, wie du sie nutzen kannst, ob der Gegenstand eine Einstimmung erforderlich macht und wie viele Ladungen er hat. 
Du erlangst auch Kenntnis darüber, ob Zauber auf dem Gegenstand liegen und welche dies sind. Wurde der Gegenstand durch einen Zauber erschaffen, ist dir bekannt, um welchen es sich handelt.

Wenn du stattdessen eine Kreatur berührst, während du den Zauber wirkst, erfährst du, welche Zauber das Ziel augenblicklich beeinflussen.

Wenn du beim Identifizieren eines Gegenstands auf diese Weise scheiterst, kannst du es nach einer [[Kurze Rast|Kurzen Rast]] erneut versuchen.