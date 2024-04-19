---
aliases: 
- Goblins
tags:
- Kreatur/Humanoide/Goblinoide/Goblin
---
```statblock
monster: Goblin
image: [[goblin.png]]
size: [[Klein]]
type: [[Humanoide]]
subtype: ([[Goblins|Goblin]], [[Goblinoide]])
alignment: [[Neutral Böse]]
ac: 13 + 2 ([[Lederrüstung]], [[Holzschild]])
sr: 0 + 1 ([[Holzschild]])
hp: 7 (2W6)
hit_dice: 2W6
speed: 9 m (6 Kästchen)
skillsaves:
  - Heimlichkeit: 6
senses: [[Dunkelsicht]], [[Wahrnehmung#Passive Wahrnehmung]] 9
languages: Gemeinsprache, Goblinisch
traits:
  - name: [[Behändes Entkommen]]
actions:
  - name: [[Krummsäbel]]
    desc: Nahkampf-Waffenangriff +4 zum Treffen, Reichweite 1,5 m (1 Kästchen), ein Ziel. Treffer 5 (1W6+2) Hiebschaden, [[Tödlich]].
  - name: [[Kurzbogen]]
    desc: Fernkampf-Waffenangriff +4 zum Treffen, Reichweite 3/24/96 m (2/16/64 Kästchen), ein Ziel. Treffer 5 (1W6+2) Stichschaden.
reactions:
  - name: Parieren
    desc: Der Krummsäbel verleiht dem Goblin die Eigenschaft [[Parieren]] als Reaktion.
```