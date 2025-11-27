---
tags:
  - Regeln/Nimble/Charakter/Klasse
Trefferwürfel: 6
Kernattribute:
  - "[[Intelligenz]]"
  - "[[Weisheit]]"
Übung:
  Waffen:
    - "[[Einfache Waffen]]"
  Rüstungen:
Rettungswürfe:
  Vorteil:
    - "[[Rettungswurf#Intelligenzrettungswurf|Intelligenzrettungswürfe]]"
    - "[[Rettungswurf#Weisheitsrettungswurf|Weisheitsrettungswürfe]]"
  Nachteil:
    - "[[Rettungswurf#Stärkerettungswurf|Stärkerettungswürfe]]"
    - "[[Rettungswurf#Konstitutionsrettungswurf|Konstitutionsrettungswürfe]]"
    - "[[Rettungswurf#Geschicklichkeitsrettungswurf|Geschicklichkeitsrettungswürfe]]"
Beschreibung: Beherrsche und forme die Elemente von Feuer, Eis und Blitz.﻿
---
# `=this.file.name`
Elementare Macht fließt durch alle Dinge … finde sie, studiere sie und mache sie dir zunutze. 
Ein Arkanist erhält seinen ersten Faden des Großen Gewebes bei der Geburt.
Wahre Meisterschaft bleibt jedoch jenen verwehrt, die sich nur auf diese angeborene Gabe ausruhen. 
Stattdessen feilen sie durch fleißiges Studium an ihren natürlichen Talenten.
Mit Folianten und Pergament als ständigen Gefährten und der weisen Führung eines oder gleich mehrerer erfahrener Mentoren. Ja, dies ist der gewählte Pfad jener, die über die Elemente herrschen wollen.
Das Geflecht des Manas zu begreifen, ist kein triviales Unterfangen. 
Es enthüllt seine arkanen Geheimnisse nur dem aufrichtigen Sucher nach Wissen. 
Doch sobald der Adept lernt, die feinen Muster zu erkennen, in denen es sich entfaltet und in die Ätherweiten strömt, erhebt sich der Lehrling wirklich in den Stand eines Arkanisten. 

Was einen Arkanisten ausmacht:
- **Zauberformung.** Forme die Zauber, die du wirkst: dehne die Zeit, erlange außerdimensionale Sicht oder lasse Echos desselben Zaubers mehrfach erklingen.
- **Elementarmeisterschaft.** Entfessele die Macht der Elemente – lass Feuer vom Himmel regnen, friere Feinde an Ort und Stelle ein oder schlage mit donnernden Blitzen zu.
- **Chaos oder Kontrolle.** Reißt du das ausgefranste Gewebe des Manas unter deine Kontrolle – oder gibst du dich den Kräften des Chaos hin? Was erwartet dich … Diamanthaut? Elementare Fesselung? Verflüssigte Beine?

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
- [[Kampfstab]]
- [[Robe]]
- 5 [[Ration|Rationen]]
- [[Seife]]
- 15 GM

---

## Klassentabelle
| Stufe | Zaubergrad | Merkmale                                           |
| ----- |:----------:| -------------------------------------------------- |
| 1     |     0      | [[Elementare Zauberei]]                            |
| 2     |     1      |                                                    |
| 3     |     1      | [[Subklassen Arkanist\|Arkanist Subklasse]]        |
| 4     |     2      | [[Primäre Attributswerterhöhung]], [[Metamagie]],  |
| 5     |     2      | [[Sekundäre Attributswerterhöhung]]                |
| 6     |     3      |                                                    |
| 7     |     3      | [[Subklassen Arkanist\|Subklassen Merkmal]]        |
| 8     |     4      | [[Primäre Attributswerterhöhung]]                  |
| 9     |     4      | [[Sekundäre Attributswerterhöhung]], [[Metamagie]] |
| 10    |     5      | [[Metamagie]]                                      |
| 11    |     5      | [[Subklassen Arkanist\|Subklassen Merkmal]]        |
| 12    |     6      | [[Primäre Attributswerterhöhung]]                  |
| 13    |     6      | [[Sekundäre Attributswerterhöhung]], [[Metamagie]] |
| 14    |     7      | [[Metamagie]]                                      |
| 15    |     7      | [[Subklassen Arkanist\|Subklassen Merkmal]]        |
| 16    |     8      | [[Primäre Attributswerterhöhung]]                  |
| 17    |     8      | [[Sekundäre Attributswerterhöhung]]                |
| 18    |     9      |                                                    |
| 19    |     9      | [[Boons#EPIC Boons]]                               |
| 20    |     9      |                                                    |

# Stufen

## Stufe 1


## Stufe 2
**Mana und Freischaltung der Grad-1-Zauber**  
Du schaltest Grad-1-Zauber von Feuer, Eis und Blitz frei und erhältst einen Manapool, um diese Zauber zu wirken. Die maximale Manaanzahl beträgt immer (INT×3)+STUFE und wird bei einer sicheren Rast wieder aufgefüllt.

**Talentierter Forscher**  
Erhalte Vorteil auf Arkan- und Wissensproben, wenn du Zugang zu vielen Büchern und Zeit hast, sie zu studieren.

## Stufe 3
**Elementarmeisterschaft**  
Lerne die Nutzzauber aus einer Zauberschule, die du kennst.

> [!tip]- Studium!  
> Wenn du arkane Bücher studierst oder während einer sicheren Rast von einem höherstufigen Magier unterrichtet wirst, kannst du deine verfügbaren Magier-Optionen neu wählen.

## Stufe 4
**Zauberformmeister**  
Du erhältst die Fähigkeit, deine Zauber durch zusätzlichen Manaeinsatz mit mächtigen Effekten zu verstärken. Wähle 2 Zauberformmeister-Fähigkeiten.

## Stufe 5
**Elementarschub**  
Ein Adrenalinstoß und deine Verbindung zu den Elementen verleihen dir zusätzliche Kraft zu Beginn des Kampfes. Bei der Initiative bekommst du WIL Mana zurück (verfällt am Ende des Kampfes, wenn es ungenutzt bleibt).

**Verbesserte Zaubertricks**  
Deine Zaubertricks werden stärker.

## Stufe 6
**Elementarmeisterschaft (2)**  
Lerne die Nutzzauber aus einer zweiten Zauberschule, die du kennst.

## Stufe 9
**Zauberformmeister (2)**  
Wähle eine weitere Zauberformmeister-Fähigkeit.

## Stufe 10
**Elementarschub (2)**  
Deine Elementarschub-Fähigkeit gibt dir jetzt WIL + 1w4 Mana zurück.

**Verbesserte Zaubertricks**  
Deine Zaubertricks werden stärker.

## Stufe 14
**Elementarmeisterschaft (3)**  
Lerne die Nutzzauber aus einer dritten Zauberschule, die du kennst.

## Stufe 15
**Unterklasse**  
Erhalte dein Magier-Unterklassenmerkmal.

**Verbesserte Zaubertricks**  
Deine Zaubertricks werden stärker.

## Stufe 17
**Elementarschub (3)**  
Deine Elementarschub-Fähigkeit gibt dir jetzt WIL + 2w4 Mana zurück.

## Stufe 20
**Erzmagier**  
+1 auf zwei beliebige deiner Werte. Der erste gestufte Zauber, den du pro Begegnung wirkst, kostet 1 Aktion und 5 Mana weniger.

**Verbesserte Zaubertricks**  
Deine Zaubertricks werden stärker.