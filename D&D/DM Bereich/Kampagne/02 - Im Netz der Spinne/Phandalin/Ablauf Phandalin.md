# `=this.file.name`

``` mermaid
graph LR
subgraph Orte
a(Barthens Proviant)
b(Löwenschilds Waren)
c(Minenbörse)
d(Gasthaus Steinhügel)
e(Schrein des Glücks)
f(Rathaus)
g(Bierhalle Schlafender Riese)
h(Erlenblatt Hof)
end

subgraph Personen
1(Elmar Barthen)
2(Harbin Wester)
3(Sildar Hallwinter)
4(Halia Dornklafter)
5(Toblen Steinhügel)
6(Schwester Garaele)
7(Linene Grauwind)
8(Quelline Erlenblatt)
9(Don-Jon Raskin)
end

subgraph Quests
A(Vorräte für Phandalin)
B(Halias Auftrag)
C(Warnung an Adabra)
D(Warnung an die Ausgräber)
E(Geborgene Waren)
F(Eskorte zur Mine)
H(Burg Cragmaw finden)
I(Suche nach Iarno)
J(Vorräte für die Holzfäller)
K(Karpfens Geschichte)
L(Rotbrenner machen Ärger)
M(Rotbrenner randalieren)
Q(Überfall auf den Butterschädelhof)
end

subgraph Locations
N(Butterschädelhof)
O(Zwergenausgrabung)
P(Haderhügel)
R(Holzfällerlager)
S(Bergzeh Goldmine)
T(Cragmaw Versteck)
U(Tresendar Anwesen)
V(Konfrontation mit den Rotbrennern)
end

a --> 1
f --> 2
f --> 3
c --> 4
d --> 5
e --> 6
b --> 7
d --> 9
h --> 8

1 --> A
4 --> B
2 --> C
2 --> D
7 --> E
9 --> F
3 --> I
3 --> H
2 --> J
8 --> K
1 --> L
5 --> M
2 --> Q

B --> V
K --> V
L --> V
M --> V
C --> P
J --> R
D --> O
F --> S
Q --> N
E --> T
I --> V
V --> U
```