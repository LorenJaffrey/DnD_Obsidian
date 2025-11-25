---
tags:
  - Regeln/Nimble/Charakter/Klasse
Trefferwürfel: 6
Kernattribute:
  - "[[Geschicklichkeit]]"
  - "[[Intelligenz]]"
Übung:
  Waffen:
    - "[[Einfache Waffen]]"
    - "[[Finesse Waffen]]"
  Rüstungen:
    - "[[Leichte Rüstung]]"
Rettungswürfe:
  Vorteil:
    - "[[Rettungswurf#Geschicklichkeitsrettungswurf|Geschicklichkeitsrettungswürfe]]"
    - "[[Rettungswurf#Intelligenzrettungswurf|Intelligenzrettungswürfe]]"
  Nachteil:
    - "[[Rettungswurf#Stärkerettungswurf]]"
    - "[[Rettungswurf#Konstitutionsrettungswurf]]"
    - "[[Rettungswurf#Weisheitsrettungswurf]]"
Beschreibung: Heimlicher, hinterhältiger, schmutzig kämpfender Schurke.
---
# `=this.file.name`
Mantel und Dolch… und noch ein Dolch. 
Der gewöhnliche "[[Gauner]]" würde sich natürlich nie so nennen – eher straßenschlauer Schurke, Überlebenskünstler oder Befreier ungenutzter Wertgegenstände. 
Sie sind Meister von Heimlichkeit, Taschendiebstahl und dem geschmeidigen Wort. 
Manche der bösartigeren Sorte sind außerdem wahre Meister des Tötens.

[[Gauner]] finden sich in jeder Stadt und an jeder Wegkreuzung unter unzähligen Namen, doch sie alle glauben an etwas Ähnliches: 
Die Welt ist grausam und gnadenlos, und wer überleben will, hat keine Zeit für so alberne Dinge wie „Moral“ oder „Ehre“. 
Das sind Luxusgüter für Reiche und Mächtige. 
Ehre bringt dich um – Überleben heißt, sich zu nehmen, was man will, wenn sich die Gelegenheit bietet. 

Als [[Gauner]] kannst du:
- **Die Regeln brechen!** Du kannst deine Würfelwürfe in die Zahlen verwandeln, die dir am besten passen.
- **Heimlich eindringen und hinterrücks zuschlagen** und mit verheerenden kritischen Treffern selbst riesige, schwer gepanzerte Gegner mit einem einzigen Hieb zu Fall bringen.
- **Schmutzig kämpfen** mit Taschensand, Tiefschlägen und gemeinen Klingen. 
  Und wenn alles aus dem Ruder läuft, verschwindest du in der Nacht – und lebst, um an einem anderen Tag wieder zu betrügen.

## Kernattribute
`$=dv.list(dv.current().Kernattribute)`

## Trefferpunkte
[[Trefferwürfel]]: 1`="W" + this.Trefferwürfel` pro Stufe
[[Trefferpunkte]] auf Stufe 1: `=this.Trefferwürfel` + [[Konstitution]]
[[Trefferpunkte]] pro Stufenaufstieg: `$="```dice:1d" + dv.current().Trefferwürfel + "```"` (min. 7) + [[Konstitution]]

## Waffen
`$=dv.list(dv.current().Übung.Waffen)`

## Rüstung
`$=dv.list(dv.current().Übung.Rüstungen)`

## Rettungswürfe
- [[Vorteil und Nachteil|Vorteil]] auf **EINEN** der folgenden:
`$=dv.list(dv.current().Rettungswürfe.Vorteil)`
- [[Vorteil und Nachteil|Nachteil]] auf **EINEN** der folgenden: 
`$=dv.list(dv.current().Rettungswürfe.Nachteil)`

## Ausrüstung
- 2[[Dolch|Dolche]]
- 5 [[Ration|Rationen]]
- [[Schleuder]]
- [[Lederrüstung]]
- [[Kreide]]
- 15 GM

---

## Klassentabelle
| Stufe | Hinterhältiger Angriff | Merkmale                                                                             |
| ----- | ---------------------- | ------------------------------------------------------------------------------------ |
| 1     | W6                     | [[Hinterhältiger Angriff]], [[Gemeiner Opportunist]]                                 |
| 2     | W6                     | [[Auf der Hut]], [[Raffinierte Aktion]], [[Verlässliches Talent]], [[Betrügen]]      |
| 3     | W8                     | [[Subklassen Gauner\|Gauner Subklasse]], [[Diebessprache]]                           |
| 4     | W8                     | [[Primäre Attributswerterhöhung]], [[Schmutzige Tricks]]                             |
| 5     | W8                     | [[Sekundäre Attributswerterhöhung]], [[Klinge drehen]], [[Schnelle Auffassungsgabe]] |
| 6     | W8                     | [[Schmutzige Tricks]], [[So ist das nicht passiert]]                                 |
| 7     | 2W8                    | [[Subklassen Gauner\|Subklassen Merkmal]]                                            |
| 8     | 2W8                    | [[Primäre Attributswerterhöhung]], [[Schmutzige Tricks]]                             |
| 9     | 2W10                   | [[Sekundäre Attributswerterhöhung]]                                                  |
| 10    | 2W10                   | [[Schmutzige Tricks]]                                                                |
| 11    | 2W12                   | [[Subklassen Gauner\|Subklassen Merkmal]]                                            |
| 12    | 2W12                   | [[Primäre Attributswerterhöhung]], [[Schmutzige Tricks]]                             |
| 13    | 2W12                   | [[Sekundäre Attributswerterhöhung]], [[Verbessertes Klinge drehen]]                  |
| 14    | 2W12                   | [[Schmutzige Tricks]]                                                                |
| 15    | 2W20                   | [[Subklassen Gauner\|Subklassen Merkmal]]                                            |
| 16    | 2W20                   | [[Primäre Attributswerterhöhung]], [[Schmutzige Tricks]]                             |
| 17    | 3W20                   | [[Sekundäre Attributswerterhöhung]]                                                  |
| 18    | 3W20                   | [[Schmutzige Tricks]]                                                                |
| 19    | 3W20                   | [[Boons#EPIC Boons]]                                                                 |
| 20    | 3W20                   | [[Perfekte Ausführung]]                                                              |