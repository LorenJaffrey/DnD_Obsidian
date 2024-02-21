``` mermaid
graph TD
a(Phandalin)

m(Schrein von Savras)

subgraph Starterquests
b(Die Zwergenausgrabung)
d(Der Haderhügel)
f(Der Butterschädelhof)
end

subgraph Nebenquests
e(Das Holzfällerlager)
g(Die Bergzeh-Goldmine)
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
n(Turm der Stürme)
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
e --> Talosanhänger
Starterquests --> Nebenquests
l --> i
g --> m
i --> n
i --> o
x --> y
p --> q
r --> s
s --> SchwarzeSpinne
a --> Cryovain
Cryovain --> SchwarzeSpinne
```

| Quests                                | Step | Stufe | Art                        | Effekt                                                     |
| ------------------------------------- |:----:|:-----:| -------------------------- | ---------------------------------------------------------- |
| [[Goblinhinterhalt]]                  |  1   |   3   | Überfall                   |                                                            |
| [[Cragmaw Versteck]]                  |  1   |   3   | Rettung                    | Entführte NPCs gerettet                                    |
| [[Konfrontation mit den Rotbrennern]] |  2   |   4   | Informationen              | [[Rotbrenner-Versteck]] finden                             |
| [[Rotbrenner-Versteck]]               |  3   |   4   | Informationen              | [[Iarno Albrek]] finden, Exposition [[Schwarze Spinne]]    |
| [[Der Haderhügel]]                    |  3   |   4   | Warnung                    | Zugriff auf Heiltränke                                     |
| [[Die Zwergenausgrabung]]             |  3   |   4   | Warnung                    | Warnung an Ausgräber                                       |
| [[Der Butterschädelhof]]              |  3   |   4   | Angriff/Rettung            | vor Orküberfall gerettet, Exposition [[Cryovain]]          |
| [[Bergzeh-Goldmine]]                  |  4   |   5   | Lieferung                  | Exposition [[Schrein von Savras]]                          |
| [[Das Holzfällerlager]]               |  4   |   5   | Lieferung/Rettung          | Exposition Talosanhänger                                   |
| [[Gnomengard]]                        |  5   |   5   | Unterstützung holen        | Unterstützung für Kampf gegen [[Cryovain]]                 |
| [[Das Alte Haus im Wald]]             |  5   |   5   | Angriff                    | Talosanhänger aufhalten, Exposition [[Kreis des Donners]]  |
| [[Axtholm]]                           |  5   |   5   | Sichern                    | Unterschlupf für Bewohner von [[Phandalin]]                |
| [[Das Drachengrab]]                   |  5   |   5   | Unterstützung holen        | Drachentöter Schwert für Kampf gegen [[Cryovain]]          |
| [[Der Schrein von Savras]]            |  5   |   6   | Angriff                    | Vision von [[Eisnadelfestung]] oder [[Burg Cragmaw]]       |
| [[Der Turm der Stürme]]               |  5   |   6   | Angriff                    | Information über [[Eisnadelfestung]] oder [[Burg Cragmaw]] |
| [[Der Kreis des Donners]]             |  6   |   6   | Finale Talosanhänger       | [[Gorthok der Donnerkeiler]] vernichten                    |
| [[Die Eisnadelfestung]]               |  6   |   6   | Finale Cryovain            | [[Cryovain]] vernichten                                    |
| [[Die Wellenhallhöhle]]               |  7   |   6   | Finale [[Schwarze Spinne]] | [[Schwarze Spinne]] aufhalten                              |