---
tags:
  - Regeln/Nimble/Charakter/Klasse
Trefferwürfel: 12
Kernattribute:
  - "[[Stärke]]"
  - "[[Geschicklichkeit]]"
Beschreibung: "Unaufhaltsame Kraft aus Zorn und Zerstörung."
---
# `=this.file.name`
Zorn und Zerstörung. Der Berserker ist die Verkörperung der Vernichtung. Er kennt weder Erschöpfung noch Vorsicht – beide werden von seiner unbändigen Wut vertrieben. 
Von jenen barbarischer Natur heißt es, sie nährten sich vom Staub des Krieges und tränken allein das Blut derer, die durch ihre Hand gefallen sind.

Der Tod ist ihm kein Fremder, denn man sagt, selbst der Tod fürchte sich davor, einen Berserker zu holen, ehe seine Kampfwut gestillt ist. 
Wenn ein Berserker einmal zu kämpfen begonnen hat, wird er nur stärker – befeuert von Kampfeslust und einer endlos brennenden Wut. 
Die Gefährlichsten unter ihnen sind nicht jene, die gut geruht haben, sondern diejenigen, die durch den Kampf an ihre Grenzen getrieben wurden. 
Es spielt keine Rolle, ob ein Berserker Axt oder Schwert führt; Fleisch wird vom Knochen gerissen, Köpfe von Schultern geschlagen. 
Viele sind unter der urtümlichen Gewalt des Berserkers zerbrochen – Schwert und Zauber sind nichts als Stroh im Sturm entfesselter Rage.

Als Berserker kannst du:
- **Zu einer rasenden Kampfmaschine werden.** Begegne dem Tod als altem Freund und kämpfe weiter!
- **Deinen Schaden auf unglaubliche Höhen steigern.** Je länger ein Kampf andauert, desto stärker entbrennt deine Wut – und mit ihr die rohe Gewalt deiner Angriffe.
- **Dein Wildes Arsenal einsetzen.** Wähle Fähigkeiten, um deine Feinde zu zerschmettern und dem Tod ins Gesicht zu lachen!

## Kernattribute
`$=dv.list(dv.current().Kernattribute)`

## Trefferpunkte
[[Trefferwürfel]]: 1`="W" + this.Trefferwürfel` pro Stufe
[[Trefferpunkte]] auf Stufe 1: `=this.Trefferwürfel` + [[Konstitution]]
[[Trefferpunkte]] pro Stufenaufstieg: `$="```dice:1d" + dv.current().Trefferwürfel + "```"` (min. 7) + [[Konstitution]]

## Waffen
- [[Einfache Waffen]] 
- [[Kriegswaffen]] 

## Rettungswürfe
- [[Vorteil und Nachteil|Vorteil]] auf **EINEN** der folgenden:
	- [[Rettungswurf#Stärkerettungswurf|Stärkerettungswürfe]] 
	- [[Rettungswurf#Geschicklichkeitsrettungswurf|Geschicklichkeitsrettungswürfe]]
- [[Vorteil und Nachteil|Nachteil]] auf **EINEN** der folgenden: 
	- [[Rettungswurf#Intelligenzrettungswurf|Intelligenzrettungswürfe]]
	- [[Rettungswurf#Weisheitsrettungswurf|Weisheitsrettungswürfe]]
	- [[Rettungswurf#Charismarettungswurf|Charismarettungswürfe]]

## Ausrüstung
- [[Streitaxt]]
- 5 [[Ration|Rationen]]
- [[Seil aus Hanf]] (15 Meter)
- 15 GM

---

## Klassentabelle
| Stufe | Wutwürfel | Merkmale                                                                  |
| ----- | --------- | ------------------------------------------------------------------------- |
| 1     | W4        | [[Wut]], [[Wüten]], [[War das schon alles]]                               |
| 2     | W4        | [[Aufsteigende Wut]], [[Eins mit den Ahnen]]                              |
| 3     | W4        | [[Berserker Subklassen\|Berserker Subklasse]], [[Blutrausch]]             |
| 4     | W4        | [[Primäre Attributswerterhöhung]], [[Wildes Arsenal]], [[Andauernde Wut]] |
| 5     | W4        | [[Sekundäre Attributswerterhöhung]], [[Verbessertes Wüten]]               | 
| 6     | W6        | [[Wildes Arsenal]]                                                        |
| 7     | W6        | [[Berserker Subklassen\|Subklassen Merkmal]]                              |
| 8     | W6        | [[Primäre Attributswerterhöhung]], [[Wildes Arsenal]]                     |
| 9     | W8        | [[Sekundäre Attributswerterhöhung]]                                       |
| 10    | W8        | [[Wildes Arsenal]]                                                        |
| 11    | W8        | [[Berserker Subklassen\|Subklassen Merkmal]]                              |
| 12    | W8        | [[Primäre Attributswerterhöhung]], [[Wildes Arsenal]]                     |
| 13    | W10       | [[Sekundäre Attributswerterhöhung]]                                       |
| 14    | W10       | [[Wildes Arsenal]]                                                        |
| 15    | W10       | [[Berserker Subklassen\|Subklassen Merkmal]]                              |
| 16    | W10       | [[Primäre Attributswerterhöhung]], [[Wildes Arsenal]]                     |
| 17    | W12       | [[Sekundäre Attributswerterhöhung]]                                       |
| 18    | W12       | [[Tiefe Wut]]                                                             |
| 19    | W12       | [[Boons#EPIC Boons]]                                                      |
| 20    | W12       | [[Grenzenlose Wut]]                                                       |