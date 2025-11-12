---
tags:
  - Nimble/Klasse
Trefferwürfel: 12
Kernattribute:
  - "[[Stärke]]"
  - "[[Geschicklichkeit]]"

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
[[Trefferpunkte]] auf Stufe 1: `$="```dice:1d" + dv.current().Trefferwürfel + "```"` + [[Konstitution]]
[[Trefferpunkte]] pro Stufenaufstieg: 1`="W" + this.Trefferwürfel` (min. 7) + [[Konstitution]]

## Übung

### Waffen
- [[Einfache Waffen]] 
- [[Kriegswaffen]] 

### Rettungswürfe
- [[Stärke]]
- [[Konstitution]]

## Ausrüstung
- [[Zweihandaxt]]
- vier [[Axt|Äxte]]
- [[Ausrüstungssets#Entdeckerausrüstung]]
- 15 GM
ODER
- 75 GM


**Saves:** STR+, INT-
**Armor:** None
**Starting Gear:** Battleaxe, Rations (meat), Rope (50 ft.)

---

| Stufe | Wutwürfel | Merkmale                |
| ----- | --------- | ----------------------- |
| 1     | 1W4       | [[Wut]]                 |
| 2     | 1W4       |                         |
| 3     | 1W4       |                         |
| 4     | 1W4       | Key Stat Increase       |
| 5     | 2W4       | Secondary Stat Increase |
| 6     | 2W6       |                         |
| 7     | 2W6       |                         |
| 8     | 2W6       | Key Stat Increase       |
| 9     | 2W8       | Secondary Stat Increase |
| 10    | 2W8       |                         |
| 11    | 2W8       |                         |
| 12    | 2W8       | Key Stat Increase       |
| 13    | 2W10      | Secondary Stat Increase |
| 14    | 2W10      |                         |
| 15    | 2W10      |                         |
| 16    | 2W10      | Key Stat Increase       |
| 17    | 2W12      | Secondary Stat Increase |
| 18    | 2W12      |                         |
| 19    | 2W12      |                         |
| 20    | 2W12      |                         |


# Stufen

## Stufe 1

**Wut**  
(1× pro Runde) Aktion: Würfle 1 Wutwürfel (1W4) und lege ihn beiseite. Addiere ihn zu jedem STÄ-Angriff, den du ausführst. Du kannst maximal SCHL Wutwürfel halten; sie verfallen, wenn deine Wut endet.

**War das schon alles?!**  
Wenn du angegriffen wirst, kannst du 1 oder mehr Wutwürfel ausgeben, um den erlittenen Schaden pro Würfel um STÄ + GES zu verringern.

> [!tip]- Deine Wut endet...  
> Wenn du den Kampf verlässt, auf 0 TP fällst oder eine Runde lang weder angreifst noch wütend bist.

> [!tip]- Ja!  
> Du kannst erneut in Wut verfallen und einen weiteren Wutwürfel erhalten, selbst wenn du bereits wütend bist. Wenn du dein Maximum erreicht hast, würfle normal und wähle, welche Würfel du behältst. Deine Wutwürfel werden beim Berechnen von Schaden gegen Monster-Rüstung mit einbezogen.

## Stufe 2

**Steigernde Wut**  
Wenn du zu Beginn deines Zuges wütend bist, würfle 1 Wutwürfel kostenlos.

**Eins mit den Ahnen**  
(1× pro Sichere Rast) Wenn du vor einer Entscheidung über Richtung oder Vorgehensweise stehst, kannst du deine Ahnen um Rat bitten, und sie führen dich auf den gefährlichsten oder herausforderndsten Pfad.

## Stufe 3

**Unterklasse**  
Wähle eine Berserker-Unterklasse.

**Blutrausch**  
Gib während deines Zuges 1 oder mehr Wutwürfel aus und bewege dich pro Würfel um GES Felder kostenlos.

## Stufe 4

**Andauernde Wut**  
Während du stirbst, verfällst du automatisch und kostenlos zu Beginn deines Zuges in Wut, hast maximal 2 Aktionen statt 1 und ignorierst STÄ-Rettungswürfe, um Angriffe auszuführen.

**Primäres Attributsplus**  
+1 STÄ oder GES. Wildes Arsenal. Wähle 1 Fähigkeit aus dem Wilden Arsenal.

> [!tip]- Zorn & Zerstörung  
> Wann immer du während einer Sicheren Rast eine bemerkenswerte Tat der Zerstörung oder Stärke vollbringst, kannst du deine verfügbaren Berserker-Optionen neu wählen.

## Stufe 5

**Wut (2)**  
Immer wenn du in Wut verfällst, erhältst du 2 Wutwürfel statt 1.

**Sekundäres Attributsplus**  
+1 INT oder WIL.

## Stufe 6

**Wildes Arsenal (2)**  
Wähle eine zweite Fähigkeit aus dem Wilden Arsenal.

**Steigernde Wut (2)**  
Deine Wutwürfel sind nun W6.

## Stufe 7

**Unterklasse**  
Erhalte das Merkmal deiner Berserker-Unterklasse.

## Stufe 8

**Wildes Arsenal (3)**  
Wähle eine dritte Fähigkeit aus dem Wilden Arsenal.

**Primäres Attributsplus**  
+1 STÄ oder GES.

## Stufe 9

**Steigernde Wut (3)**  
Deine Wutwürfel sind nun W8.

**Sekundäres Attributsplus**  
+1 INT oder WIL.

## Stufe 10

**Wildes Arsenal (4)**  
Wähle eine vierte Fähigkeit aus dem Wilden Arsenal.

## Stufe 11

**Unterklasse**  
Erhalte das Merkmal deiner Berserker-Unterklasse.

## Stufe 12

**Wildes Arsenal (5)**  
Wähle eine fünfte Fähigkeit aus dem Wilden Arsenal.

**Primäres Attributsplus**  
+1 STÄ oder GES.

## Stufe 13

**Steigernde Wut (4)**  
Deine Wutwürfel sind nun W10.

**Sekundäres Attributsplus**  
+1 INT oder WIL.

## Stufe 14

**Wildes Arsenal (6)**  
Wähle eine sechste Fähigkeit aus dem Wilden Arsenal.

## Stufe 15

**Unterklasse**  
Erhalte das Merkmal deiner Berserker-Unterklasse.

## Stufe 16

**Wildes Arsenal (7)**  
Wähle eine siebte Fähigkeit aus dem Wilden Arsenal.

**Primäres Attributsplus**  
+1 STÄ oder GES.

## Stufe 17

**Steigernde Wut (5)**  
Deine Wutwürfel sind nun W12.

**Sekundäres Attributsplus**  
+1 INT oder WIL.

## Stufe 18

**TIEFE WUT**  
Das Fallen auf 0 TP beendet deine Wut nicht mehr.

## Stufe 19

**Epische Gabe**  
Wähle eine Epische Gabe.

## Stufe 20

**GRENZENLOSE WUT**  
+1 auf zwei beliebige Attribute. Wann immer du auf einem Wutwürfel weniger als 6 würfelst, ändere das Ergebnis zu 6.