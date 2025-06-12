``` mermaid
graph TD
a(Phandalin)

subgraph Starterquests
b(Die Zwergenausgrabung)
d(Der Haderhügel)
f(Der Butterschädelhof)
end

subgraph Nebenquests
e(Das Holzfällerlager)
end 

subgraph Cryovain

subgraph Unterstützungsquests
h(Axtholm)
c(Gnomengard)
j(Das Drachengrab)
end

k(Eisnadelfestung)
end

subgraph Talosanhänger
i(Das alte Haus im Wald)
l(Jagdhaus des Falken)
o(Kreis des Donners)
end

subgraph Intro
p(Goblinüberfall)
q(Cragmaw Versteck)
end

subgraph Rotbrenner
r(Konfrontation mit den Rotbrennern)
s(Rotbrenner Versteck)
end

subgraph SchwarzeSpinne
x(Burg Cragmaw)
y(Wellenhallhöhle)
end

Intro --> a
a --> Starterquests
a --> Rotbrenner
a --> Nebenquests
e --> Talosanhänger
Starterquests --> Cryovain
l --> i
i --> o
x --> y
p --> q
r --> s
s --> SchwarzeSpinne
Cryovain --> SchwarzeSpinne
```

| Quests                                     | Step | Stufe | Art                        | Effekt                                                    |
| ------------------------------------------ |:----:|:-----:| -------------------------- | --------------------------------------------------------- |
| [[Goblinhinterhalt]]                       |  1   |   3   | Überfall                   |                                                           |
| [[Cragmaw Versteck]]                       |  1   |   3   | Rettung                    | Entführte NPCs gerettet                                   |
| [[Konfrontation mit den Rotbrennern]]      |  2   |   4   | Informationen              | [[Rotbrenner-Versteck]] finden                            |
| [[Tresendar Anwesen\|Rotbrenner Versteck]] |  3   |   4   | Informationen              | [[Iarno Albrek]] finden, Exposition [[Schwarze Spinne]]   |
| [[Haderhügel]]                             |  3   |   4   | Warnung                    | Zugriff auf Heiltränke                                    |
| [[Zwergenausgrabung]]                      |  3   |   4   | Warnung                    | Warnung an Ausgräber                                      |
| [[Butterschädelhof]]                       |  3   |   4   | Angriff/Rettung            | vor Orküberfall gerettet, Exposition [[Cryovain]]         |
| [[Bergzeh-Goldmine]]                       |  4   |   5   | Lieferung                  | Exposition [[Schrein von Savras]]                         |
| [[Das Holzfällerlager]]                    |  4   |   5   | Lieferung/Rettung          | Exposition Talosanhänger                                  |
| [[Altes Haus im Wald]]                     |  5   |   5   | Angriff                    | Talosanhänger aufhalten, Exposition [[Kreis des Donners]] |
| [[Kreis des Donners]]                      |  5   |   5   | Finale Talosanhänger       | [[Gorthok der Donnerkeiler]] vernichten                   |
| [[Gnomengard]]                             |  5   |   5   | Unterstützung holen        | Unterstützung für Kampf gegen [[Cryovain]]                |
| [[Axtholm]]                                |  5   |   5   | Sichern                    | Unterschlupf für Bewohner von [[Phandalin]]               |
| [[Das Drachengrab]]                        |  5   |   5   | Unterstützung holen        | Drachentöter Schwert für Kampf gegen [[Cryovain]]         |
| [[Die Eisnadelfestung]]                    |  6   |   6   | Finale Cryovain            | [[Cryovain]] vernichten                                   |
| [[Die Wellenhallhöhle]]                    |  7   |   6   | Finale [[Schwarze Spinne]] | [[Schwarze Spinne]] aufhalten                             |