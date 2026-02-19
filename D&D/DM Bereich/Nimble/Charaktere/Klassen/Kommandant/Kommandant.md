---
tags:
  - Regeln/Nimble/Charakter/Klasse
Trefferwürfel: 10
Kernattribute:
  - "[[Stärke]]"
  - "[[Charisma]]"
Übung:
  Waffen:
    - "[[Einfache Waffen]]"
    - "[[Kriegswaffen]]"
  Rüstungen:
    - "[[Schwere Rüstung]]"
    - "[[Schilde]]"
Rettungswürfe:
  Vorteil:
    - "[[Rettungswurf#Stärkerettungswurf|Stärkerettungswürfe]]"
    - "[[Rettungswurf#Charismarettungswurf|Charismarettungswürfe]]"
  Nachteil:
    - "[[Rettungswurf#Geschicklichkeitsrettungswurf|Geschicklichkeitsrettungswürfe]]"
    - "[[Rettungswurf#Intelligenzrettungswurf|Intelligenzrettungswürfe]]"
    - "[[Rettungswurf#Weisheitsrettungswurf|Weisheitsrettungswürfe]]"
Beschreibung: "Ein Taktiker, Anführer und Waffenmeister."
---
# `=this.file.name`
Soldat … Krieger … furchtloser Anführer.  
Unter den fähigsten Kämpfern der Welt sind die Kommandanten wahre Meister jeder Waffe und jeder Form des Nahkampfs. 
Eine kleine Einheit, geführt von einem ausgebildeten Kommandanten, erweckt mehr Furcht als unzählige Legionen ohne einen.

Ein „Reich“ ist erst dann wirklich ein _Imperium_, wenn es seine eigene Akademie der Kriegskunst besitzt – berühmte Schulen, in denen diese außergewöhnlich fähigen Soldaten in Schlachtfeldtaktik und Führungskunst unterrichtet werden. 

Kommandanten zeichnen sich aus durch:
- **Taktische Befehle.** Erteile mächtige Kommandos an deine Verbündeten, stärke ihre Fähigkeiten und koordiniere verheerende Angriffe. Beherrsche das Schlachtfeld mit Präzision und Können und wende das Blatt jeder Schlacht zu deinen Gunsten.    
- **Waffenmeisterschaft.** Beherrsche jede Waffenart und führe sie mit tödlicher Effizienz. Deine Vielseitigkeit stellt sicher, dass kein Gegner dir gewachsen ist.
- **Strategische Führung.** Nutze dein taktisches Geschick, um Feinde auszutricksen und zu überlisten, und führe deine Gruppe mit kluger Strategie und entschlossener Handlung zum Sieg.

## Kernattribute
`$=dv.list(dv.current().Kernattribute)`

## Trefferpunkte
[[Trefferwürfel]]: 1`="W" + this.Trefferwürfel` pro Stufe
[[Trefferpunkte]] auf Stufe 1: `=this.Trefferwürfel` + [[Konstitution]]
[[Trefferpunkte]] pro Stufenaufstieg: `$="```dice:1d" + dv.current().Trefferwürfel + "```"` (min. `=this.Trefferwürfel/2`) + [[Konstitution]]

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
- [[Kurzschwert]]
- [[Kettenhemd]]
- 5 [[Ration|Rationen]]
- 15 GM

---

## Klassentabelle
| Stufe | Kampfwürfel | Merkmale                                        |
| ----- | ----------- | ----------------------------------------------- |
| 1     |             | [["Koordinierter Schlag!"]]                     |
| 2     |             |                                                 |
| 3     |             | [[Subklassen Kommandant\|Kommandant Subklasse]] |
| 4     | W6          | [[Primäre Attributswerterhöhung]]               |
| 5     | W8          | [[Sekundäre Attributswerterhöhung]]             |
| 6     | W8          | [[Wildes Arsenal]]                              |
| 7     | W8          | [[Subklassen Kommandant\|Subklassen Merkmal]]    |
| 8     | W8          | [[Primäre Attributswerterhöhung]]               |
| 9     | W10         | [[Sekundäre Attributswerterhöhung]]             |
| 10    | W10         |                                                 |
| 11    | W10         | [[Subklassen Kommandant\|Subklassen Merkmal]]    |
| 12    | W10         | [[Primäre Attributswerterhöhung]]               |
| 13    | W12         | [[Sekundäre Attributswerterhöhung]]             |
| 14    | W12         |                                                 |
| 15    | W12         | [[Subklassen Kommandant\|Subklassen Merkmal]]    |
| 16    | W12         | [[Primäre Attributswerterhöhung]]               |
| 17    | W20         | [[Sekundäre Attributswerterhöhung]]             |
| 18    | W20         |                                                 |
| 19    | W20         | [[Boons#EPIC Boons]]                            |
| 20    | W20         |                                                 |


# Stufen

## Stufe 2
**Befehle des Kommandanten**  
Wähle 2 Befehle des Kommandanten.

**Feldsanitäter**  
Würfle 1 zusätzlichen Würfel für jeden Heiltrank, den du verabreichst. Immer wenn du oder ein Verbündeter Trefferwürfel ausgebt, um TP zu regenerieren, und du mindestens zehn Minuten mit der Untersuchung ihrer Wunden verbracht hast, darf diese Kreatur deinen Bonus auf Untersuchung zu den zurückgewonnenen TP addieren.

## Stufe 4
**Für jedes Schlachtfeld gerüstet**  
Wähle eine Kampftaktik. Wenn du Initiative würfelst, erhältst du STÄ Kampfwürfel, jeweils w6. (1/Angriff) darfst du einen Kampfwürfel ausgeben, um ein Spezialmanöver auszuführen. Kampfwürfel verfallen, wenn der Kampf endet.

> [!tip]- Hartes Training  
> Immer wenn du während einer sicheren Rast mit deiner Gruppe oder anderen Soldaten trainierst, kannst du andere verfügbare Kommandanten‑Optionen wählen.

## Stufe 5
**Meisterkommandant**  
Wenn du Initiative würfelst, erhältst du 1 verbrauchte Anwendung von Koordinierter Schlag zurück (verfällt, wenn sie in dieser Begegnung nicht genutzt wird). Angriffe aus deinen Koordinierten Schlägen ignorieren nun Nachteil.

**Kampftaktiken**  

## Stufe 6
**Für jedes Schlachtfeld gerüstet (2)**  
Wähle eine weitere Kampffähigkeit oder erhalte +1 maximales Kampfwürfel‑Limit.

**Waffenmeisterschaft**  
Du darfst 2× pro Runde kostenlos eine Waffe wegstecken und eine andere ziehen. Wähle einen Waffentyp, in dem du dich spezialisierst.

## Stufe 8
**Für jedes Schlachtfeld gerüstet (3)**  
Wähle eine weitere Kampffähigkeit oder erhalte +1 maximales Kampfwürfel‑Limit.

## Stufe 9
**Meisterkommandant (2)**  
+1 Nutzung von Koordinierter Schlag pro Sicherer Rast.

## Stufe 10
**Für jedes Schlachtfeld gerüstet (4)**  
Wähle eine weitere Kampffähigkeit oder erhalte +1 maximales Kampfwürfel‑Limit.

**Waffenmeisterschaft (2)**  
Wähle einen zweiten Waffentyp, in dem du dich spezialisierst.

## Stufe 12
**Für jedes Schlachtfeld gerüstet (5)**  
Wähle eine weitere Kampffähigkeit oder erhalte +1 maximales Kampfwürfel‑Limit.

## Stufe 13
**Meisterkommandant (3)**  
+1 Nutzung von Koordinierter Schlag pro Sicherer Rast.

## Stufe 14
**Waffenmeisterschaft (3)**  
Du beherrschst nun alle Waffentypen vollständig.

## Stufe 16
**Für jedes Schlachtfeld gerüstet (6)**  
Wähle eine weitere Kampffähigkeit oder erhalte +1 maximales Kampfwürfel‑Limit.

## Stufe 17
**Meisterkommandant (4)**  
+1 Nutzung von Koordinierter Schlag pro Sicherer Rast.

## Stufe 18
**Unvergleichliche Taktik**  
Wenn du in einer Begegnung zum ersten Mal Koordinierter Schlag einsetzt, erhält ein Verbündeter, der dich hören kann, 1 zusätzliche Aktion für seinen nächsten Zug.

## Stufe 19
**Epischer Segen**  
Wähle einen Epischen Segen.

## Stufe 20
**Hauptmann der Legionen**  
+1 auf zwei beliebige deiner Werte. Wenn du in einer Begegnung zum ersten Mal Koordinierter Schlag einsetzt, erhält JEDER Verbündete innerhalb von 12 Feldern +1 Aktion (ersetzt Unvergleichliche Taktik).