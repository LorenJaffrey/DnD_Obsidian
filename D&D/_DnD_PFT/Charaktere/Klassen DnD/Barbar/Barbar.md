---
aliases:
  - Barbaren
tags:
  - Klasse
  - Regeln/PHB2024
Art: Krieger
Name_Subklassen: "[[Urtümliche Pfade|Urtümlicher Pfad]]"
Trefferwürfel: W12
Hauptattribut:
  - "[[Stärke]]"
Komplexität: Mittel
Kampfrausch:
  Stufe1:
    Anzahl: 2
    Bonusschaden: 2
  Stufe2:
    Anzahl: 2
    Bonusschaden: 2
  Stufe3:
    Anzahl: 3
    Bonusschaden: 2
  Stufe4:
    Anzahl: 3
    Bonusschaden: 2
  Stufe5:
    Anzahl: 3
    Bonusschaden: 2
  Stufe6:
    Anzahl: 4
    Bonusschaden: 2
  Stufe7:
    Anzahl: 4
    Bonusschaden: 2
  Stufe8:
    Anzahl: 4
    Bonusschaden: 2
  Stufe9:
    Anzahl: 4
    Bonusschaden: 3
  Stufe10:
    Anzahl: 4
    Bonusschaden: 3
  Stufe11:
    Anzahl: 4
    Bonusschaden: 3
  Stufe12:
    Anzahl: 5
    Bonusschaden: 3
  Stufe13:
    Anzahl: 5
    Bonusschaden: 3
  Stufe14:
    Anzahl: 5
    Bonusschaden: 3
  Stufe15:
    Anzahl: 5
    Bonusschaden: 3
  Stufe16:
    Anzahl: 5
    Bonusschaden: 4
  Stufe17:
    Anzahl: 6
    Bonusschaden: 4
  Stufe18:
    Anzahl: 6
    Bonusschaden: 4
  Stufe19:
    Anzahl: 6
    Bonusschaden: 4
  Stufe20:
    Anzahl: 6
    Bonusschaden: 4
---
# `=this.file.name`

## Klassentabelle

| Stufe |        Anzahl Kampfräusche         |            Kampfrausch Schaden            | Merkmale                                        |
|:-----:|:----------------------------------:|:-----------------------------------------:| ----------------------------------------------- |
|   1   | `=this.Kampfrausch.Stufe1.Anzahl`  | +`=this.Kampfrausch.Stufe1.Bonusschaden`  | [[Kampfrausch]], [[Ungerüstete Verteidigung]]   |
|   2   | `=this.Kampfrausch.Stufe2.Anzahl`  | +`=this.Kampfrausch.Stufe2.Bonusschaden`  | [[Rücksichtsloser Angriff]], [[Gefahrengespür]] |
|   3   | `=this.Kampfrausch.Stufe3.Anzahl`  | +`=this.Kampfrausch.Stufe3.Bonusschaden`  | [[Urtümliche Pfade]], [[Urwissen]]              |
|   4   | `=this.Kampfrausch.Stufe4.Anzahl`  | +`=this.Kampfrausch.Stufe4.Bonusschaden`  | [[Talente\|Talent]]                             |
|   5   | `=this.Kampfrausch.Stufe5.Anzahl`  | +`=this.Kampfrausch.Stufe5.Bonusschaden`  | [[Zusätzlicher Angriff]], [[Schnelle Bewegung]] |
|   6   | `=this.Kampfrausch.Stufe6.Anzahl`  | +`=this.Kampfrausch.Stufe6.Bonusschaden`  | Pfadmerkmal                                     |
|   7   | `=this.Kampfrausch.Stufe7.Anzahl`  | +`=this.Kampfrausch.Stufe7.Bonusschaden`  | [[Wilder Instinkt]], [[Instinktiver Sprung]]    |
|   8   | `=this.Kampfrausch.Stufe8.Anzahl`  | +`=this.Kampfrausch.Stufe8.Bonusschaden`  | [[Talente\|Talent]]                             |
|   9   | `=this.Kampfrausch.Stufe9.Anzahl`  | +`=this.Kampfrausch.Stufe9.Bonusschaden`  | [[Brutaler Hieb]]                               |
|  10   | `=this.Kampfrausch.Stufe10.Anzahl` | +`=this.Kampfrausch.Stufe10.Bonusschaden` | Pfadmerkmal                                     |
|  11   | `=this.Kampfrausch.Stufe11.Anzahl` | +`=this.Kampfrausch.Stufe11.Bonusschaden` | [[Unerbittlicher Kampfrausch]]                  |
|  12   | `=this.Kampfrausch.Stufe12.Anzahl` | +`=this.Kampfrausch.Stufe12.Bonusschaden` | [[Talente\|Talent]]                             |
|  13   | `=this.Kampfrausch.Stufe13.Anzahl` | +`=this.Kampfrausch.Stufe13.Bonusschaden` | [[Verbesserter Brutaler Hieb]]                  |
|  14   | `=this.Kampfrausch.Stufe14.Anzahl` | +`=this.Kampfrausch.Stufe14.Bonusschaden` | Pfadmerkmal                                     |
|  15   | `=this.Kampfrausch.Stufe15.Anzahl` | +`=this.Kampfrausch.Stufe15.Bonusschaden` | [[Anhaltender Kampfrausch]]                     |
|  16   | `=this.Kampfrausch.Stufe16.Anzahl` | +`=this.Kampfrausch.Stufe16.Bonusschaden` | [[Talente\|Talent]]                             |
|  17   | `=this.Kampfrausch.Stufe17.Anzahl` | +`=this.Kampfrausch.Stufe17.Bonusschaden` | [[Überlegener Brutaler Hieb]]                   |
|  18   | `=this.Kampfrausch.Stufe18.Anzahl` | +`=this.Kampfrausch.Stufe18.Bonusschaden` | [[Unbändige Stärke]]                            |
|  19   | `=this.Kampfrausch.Stufe19.Anzahl` | +`=this.Kampfrausch.Stufe19.Bonusschaden` | [[Talente\|Talent]]                             |
|  20   | `=this.Kampfrausch.Stufe20.Anzahl` | +`=this.Kampfrausch.Stufe20.Bonusschaden` | [[Meister der Wildnis]]                         |

## Trefferpunkte
[[Trefferwürfel]]: 1`=this.Trefferwürfel` pro Stufe
[[Trefferpunkte]] auf Stufe 1: 12 + [[Konstitution#Konstitutionsmodifikator]]
[[Trefferpunkte]] pro Stufenaufstieg: 1`=this.Trefferwürfel` (min. 7) + [[Konstitution#Konstitutionsmodifikator]]

## Übung
### Rüstungen
- [[Leichte Rüstung]]
- [[Mittelschwere Rüstung]]
- [[Schilde]]

### Waffen
- [[Einfache Waffen]] 
- [[Kriegswaffen]] 

### Rettungswürfe
- [[Stärke]]
- [[Konstitution]]

### Fertigkeiten
- zwei nach Wahl:
	- [[Athletik]]
	- [[Einschüchtern]]
	- [[Mit Tieren umgehen]]
	- [[Naturkunde]]
	- [[Überlebenskunst]]
	- [[Wahrnehmung]]

## Ausrüstung
- [[Zweihandaxt]]
- vier [[Axt|Äxte]]
- [[Ausrüstungssets#Entdeckerausrüstung]]
- 15 GM
ODER
- 75 GM

## Klassenbeschreibung
Ein großer Stammeskrieger der Menschen schreitet in Felle gehüllt und mit seiner Axt in der Hand durch den Schneesturm. Er lacht, als er auf den Frostriesen zustürmt, der es gewagt hat, die Elchherde seiner Leute zu rauben.
Eine Halborkin knurrt den neuesten Herausforderer an, der ihre Autorität über den wilden Stamm anzweifelt, und bereitet sich darauf vor, sein Genick mit bloßen Händen zu brechen - so wie bei den sechs vorherigen Rivalen.
Mit Schaum vor dem Mund donnert ein Zwerg seinen Helm in das Gesicht eines Drow-Kriegers, wirbelt dann herum und treibt seinen gepanzerten Ellbogen in den Magen eines weiteren Gegners.
Diese drei Barbaren, so unterschiedlich sie auch sein mögen, definieren sich durch ihre Wut und ihre ungezügelte, unstillbare und gedankenlose Raserei, die in ihrer Wildheit der eines in die Enge getriebenen Raubtiers entspricht, des unablässigen Anbrausens eines Sturms, des aufgewühlten Durcheinanders des Meeres. Für manche entspringt diese Wut der Zwiesprache mit wilden Tiergeistern, andere ziehen Energie aus einem sich anstauenden Groll, genährt durch das Leben in einer Welt voller Schmerz. Für jeden Barbar ist die Wut eine Kraft, die ihn nicht nur in den Kampfrausch treibt, sondern die auch unglaubliche Reflexe, Ausdauer und Stärke ermöglicht.

### Urinstinkte
Die Bevölkerung der Dörfer und Städte ist stolz darauf, wie sehr ihre zivilisierte Art sie vom Tier unterscheidet - als wenn es ein Zeichen von Überlegenheit wäre, die eigene Natur zu verleugnen. Für einen Barbaren ist Zivilisiertheit keine Tugend, sondern ein Zeichen der Schwäche. Die Starken nehmen ihre tierische Natur an, mitsamt der scharfen Sinne, der rohen Kraft und des wilden Zorns. Barbaren fühlen sich unwohl, wenn sie von Mauern und Gedränge umgeben sind. Sie blühen in der Wildnis ihrer Heimatländer auf, wie der Tundra, dem Dschungel oder dem Grasland, wo ihre Stämme leben und jagen. Erst in der Hitze der Schlacht fühlen sich Barbaren wirklich lebendig. Sie können sich in einen Berserkerzustand versetzen, in dem die Wut Überhand nimmt und ihnen übermenschliche Stärke und Widerstandskraft verleiht. Ein Barbar kann sich dieser Fähigkeit nur wenige Male bedienen, ohne eine Rast zu machen, doch reicht das in der Regel aus, um jede Bedrohung, die da kommen mag, in den Staub zu stampfen.

### Ein gefährliches Leben
Nicht jedes Mitglied eines Stammes, der von den Angehörigen einer zivilisierten Gesellschaft als „barbarisch" bezeichnet wird, hat auch die gleichnamige Klasse. Ein wahrer Barbar ist unter diesen Leuten genauso selten wie ein ausgebildeter Kämpfer in einem kleinen Weiler, und in Kriegszeiten nehmen beide eine ähnliche Rolle als Beschützer und Führer ihres Volks ein. Das Leben an den wilden Plätzen der Welt birgt viele tödliche Gefahren, wie rivalisierende Stämme, lebensgefährliches Wetter und schreckliche Monster. Um seine Leute vor diesen zu beschützen, stürzt sich ein Barbar kopfüber in jedes Wagnis. Der Mut der Barbaren im Angesicht der Gefahr passt perfekt zu einem Leben als Abenteurer. Die Wanderschaft ist oft die natürliche Lebensart ihrer Stämme, das entwurzelte Dasein eines Abenteurers stellt für die meisten Barbaren also keine Belastung dar. Manch einer mag die eng gewobenen Familienstrukturen seines Stammes vermissen, doch kann die Beziehung zu den Mitgliedern der Abenteurergruppe diese gelegentlich ersetzen.

### Einen Barbaren erschaffen
Mache dir bei der Erschaffung deines Barbaren zuerst darüber Gedanken, von wo dein Charakter kommt und was sein Platz in der Welt ist. Berate dich auch mit dem St. über eine angemessene Herkunft deines Abenteurers. Kommt er aus einem fernen Land und ist er in der Region, in der sich eure Gruppe jetzt aufhält, ein Fremder? Oder Bndet die Kampagne in einem rauen und umkämpften Grenzland statt, wo Stammeskrieger etwas ganz Gewöhnliches sind?
Was hat ihn dazu bewogen, das Leben eines Abenteurers zu führen? Wurde er von der Aussicht auf Reichtümer in die besiedelten Länder gelockt? Oder hat er sich den Soldaten dieser Länder nur angeschlossen, um sich einer gemeinsamen Bedrohung zu stellen? Haben Monster oder eine einfallende Horde ihn aus seinem Heimatland vertrieben und ihn zu einem entwurzelten Flüchtling gemacht? Vielleicht ist er auch ein Kriegsgefangener, der in Ketten in die Zivilisation kam und erst jetzt seine Freiheit wiedererlangte? Oder wurde er von seinen Leuten verstoßen, weil er ein Verbrechen beging, ein Tabu brach oder versuchte, die Häuptlingswürde in einem Zweikampf an sich zu reißen, und scheiterte?

## Origin Hooks

### Popkultur
- Wikinger
- Hulk
- Conan
- Thor

### Ausgestoßener aus einer Magierfamilie
- Ausgestoßener aus einer Magierfamilie, der sich beweisen will
- Muss alle Mitglieder seiner Familie (alles mächtige Magier) besiegen/töten
- Pfad der Wilden Magie