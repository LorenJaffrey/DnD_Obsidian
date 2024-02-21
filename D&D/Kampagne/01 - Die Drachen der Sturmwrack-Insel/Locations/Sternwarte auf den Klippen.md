## Drachenruh
>[!quote] Als ihr in Drachenruh ankommt, bemerkt ihr, dass es kaum heller geworden ist. Stattdessen hat der Himmel eine grünliche Farbe angenommen. Dicke graue Regenwolken verhängen den Himmel. 

- Regen setzt ein
- Runara gibt Schlüssel

## Anreise über Land
>[!quote] Als ihr über den steinigen Boden der Sturmwrack-Insel klettert, seht ihr merkwürdige, glasartige Kristallauswüchse aus dem Boden ragen. Die Vegetation hier zeigt rötliche, sich verzweigende Narben, die ähnliche Formen aufweisen. 

## D1: Ankunft bei der Sternwarte
>[!quote] Ein wilder, überwucherter Pfad windet sich zum Rand der Klippe. Der Aussichtspunkt wird von zwei Marmorstatuen mit Goldadern markiert, jede wie ein Drache geformt, die Mäuler in stummem Schrei aufgerissen. Vor euch liegt die verfallene Sternwarte, die sich auf Basaltsäulen ca. 10m aus den Fluten erhebt. Aus den Fenstern und der geborstenen Glaskuppel schillert vielfarbiges Licht und ihr hört drakonische Intonationen. Plötzlich ertönt ein bestialischer Schrei, doch er klingt nicht bedrohlich, sondern gequält. Als ob eine mächtige Bestie gefoltert wird...

- Wurf auf [[Nachforschungen]] gegen SG 10 enthüllt eine kleine Aussparung im Maul jeder Statue. Passend für den Kristallschlüssel.
- wenn Schlüssel benutzt wird kommen Mekk und Minn geflogen

### Kampf gegen Mek und Min
```statblock
name: Mek & Min
size: Klein
type: Humanoid
alignment: Rechtschaffen Böse
ac: 13
hp: 40
speed: 9m, Fliegen 9m
stats: [7, 16, 9, 8, 7, 8]
languages: Gemeinsprache, Drakonisch
senses: [[Wahrnehmung#Passive Wahrnehmung]] 8
cr: 1
traits:
  - name: Fliehen
    desc: Wenn sie halbes Leben erreichen explodiert die Waffe und versinkt im Meer. Mek stirbt und Min flieht in die Sternwarte.
actions:
  - name: Mylas Elementarkanone
    desc: Fernkampfangriff +5, Reichweite 9 18, ein Ziel. Treffer 1W12 Blitzschaden. Wenn der Angriff trifft, kannst du ein weiteres Ziel innerhalb 1,5 Meter wählen welches zusatzlich halben Schaden erleidet.
  - name: Peitsche
    desc: Nahkampfwaffenangriff +5 auf Treffer, Reichweite 3m, ein Ziel. Treffer 1W4+3 Hiebschaden
bonus_actions:
  - name: Blutmücke
    desc: Einer der beiden lässt seine Peitsche knallen. Eine Blutmücke innerhalb von 18m (12 Kästchen) kann sich 3m(2 Kästchen) bewegen und ihre Reaktion nutzen um anzugreifen.
```

- Kampf gegen Mek und Min und 6 Blutmücken

## D2: Rotunde
>[!quote] Der Platz liegt voller Steintrümmer - einst elegante Statuen, imposante Säulen und polierte Marmorwände. In der Mitte steht eine große Skulptur auf der sich Ringe mit rostigen Planeten und vergoldeten Sternen träge in einer ruckeligen Imitation planetarer Bewegungen drehen. Um die Skulptur sind 5 krude Totems verteilt. Sie haben entfernt die Form von Drachen und sind aus Holz, Geröll und Knochen gebaut. Jedes Totem hat eine andere Farbe. Eine Kugel aus schillernder Energie schwebt über der Skulptur. Neben der Skulptur im Süden liegt ein schwer mitgenommener bronzefarbener Drache angekettet am Boden. 

### Ritual des drakonischen Aufstiegs
Lässt Funkenschinder zu einem jungen blauen Drachen aufsteigen

#### Bestandteile
- 5 Totems (Bronze, Gold, Blau, Rot und Messing)
- Königstöter Meteorit
- Aidron opfern

#### Ritual durchführen
Wurf auf [[Arkane Kunde]] gegen [[Schwierigkeitsgrad|SG]] 10
Bei erfolgreichem Wurf wird das Ritual beendet und Funkenschinder steigt zu einem Jungen Blauen Drachen auf.
Bei Misslingen erleidet er W20 [[Energieschaden]]

#### Skulptur
Die Skulptur bewegt sich mit der darin gebildeten Energiekugel.
Wenn die Skulptu zerstört wird endet das Ritual sofort.
Skulptur hat [[Rüstungsklasse]] 20 und 27 [[Trefferpunkte]].

#### Totems
Totems haben [[Rüstungsklasse]] 17 und 5 [[Trefferpunkte]].
Wenn alle Totems zerstört werden endet das Ritual sofort.
Wenn ein Totem zerstört wird wird der Wurf für das Ritual um -2 erschwert.
Lösen einen zusätzlichen Effekt pro Runde aus:

| W10  | Effekt             | Wirkung                                                                                                                                                                            |
| ---- | ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-2  | Astalagans Segen   | Aidron und die Charaktere erhalten jeweils 1W4+4 Trefferpunkte zurück, als das Bronzelicht sie umgibt und wärmt.                                                                   |
| 3-4  | Clyssavars Flammen | Funkenschinder muss einen [[Rettungswurf]] auf [[Geschicklichkeit]] bestehen oder erleidet 2W6 [[Feuerschaden]] wenn das goldene Licht mit ihm kollidiert.                           |
| 5-6  | Eldenemirs Gabe    | Funkenschinders Odemwaffe wird aufgeladen, wenn er ins blaue Licht gerät.                                                                                                          |
| 7-8  | Sharruths Zorn     | Alle Charaktere müssen einen [[Rettungswurf]] auf [[Geschicklichkeit]] bestehen oder erleiden 1W6 [[Feuerschaden]] wenn das rote Licht feurig explodiert.                            |
| 9-10 | Turadaers Tricks   | Während das Messinglicht um die herum schimmert und funkelt, sind Aidron und die Charaktere bei jedem [[Angriffswurf]] und [[Rettungswurf]] im [[Vorteil_und_Nachteil|Vorteil]] |

#### Aidron befreien
Aidron ist mit 6 großen Eisennägeln und einer massiven Kette am Boden festgenagelt. Wenn min. 2 Nägel entfernt werden hat er genug Spielraum um sich zu befreien und seine Atemattacke einzusetzen.
Einen Eisennagel zu entfernen erfordert eine [[Zug#Aktion]].


```statblock
monster: Blue Dragon Wyrmling
```
## D3: Lager der Kobolde
>[!quote] Eine morsche Brücke aus Treibholz und Seilen überspannt den Abgrund zwischen der Rotunde und diesem Gebäude. Aus diesem eingestürzten Turm dringen Laute - ein Wuseln und ein Wispern. Lücken im Stein wurden mit Planken und Stoffresten geschlossen.

Min kauert in einer Ecke im Lager
- Bittet Charaktere ihn nicht zu töten
- es tut ihm Leid und Funkenschinder hat sie gezwungen ihm zu folgen
- jetzt ist sein Bruder tot und er bereut alles was er getan hat
- bietet an dem "bronzenen Drachen" zu dienen oder nach Drachenruh zurückzukehren

## D4: Einsames Studierzimmer
>[!quote] Der Rhythmus der Brandung hallt im Turm wider. Ein Teil des Bodens ist eingestürzt und gibt den Blick in die Kammer darunter frei. Aus den Trümmern ragen zerborstene Bücherregale in absurden Winkeln. Auf dem Boden verstreut liegen schimmlige Bücher.

Wenn Charaktere die Bücher untersuchen finden sie ein kleines schwarzes Tagebuch mit einem verzierten Schloss welches noch intakt wirkt.
- Wurf auf [[Wahrnehmung]] gegen [[Schwierigkeitsgrad|SG]] 15 enthüllt eine kleine arkane Rune über dem Schlüsselloch ([[Magie entdecken]] offenbart eine schwache magische Aura)
- Wurf auf [[Arkane Kunde]] gegen [[Schwierigkeitsgrad|SG]] 11 offenbart wie man die Rune deaktiviert. (Vorsichtig mit einem spitzen Metallgegenstand nachfahren)
- Wenn Buch geöffnet wird ohne die Rune zu deaktivieren erleidet der Öffnende 1W6 [[Giftschaden]] 
- Kann mithilfe von [[Diebeswerkzeug]] mit einem Wurf auf [[Fingerfertigkeit]] gegen [[Schwierigkeitsgrad|SG]] 12 geöffnet werden (alternativ Wurf auf [[Stärke]] gegen [[Schwierigkeitsgrad|SG]] 12)
- enthält Sternenkarten und Notizen zu stellaren Phänomenen. Darunter auch zum Königstöter Meteorit und dem Ritual des drakonischen Aufstiegs
- Am Anfang des Tagebuchs findet sich eine unterstrichene Passage: "Hört ihr vier Gelehrten: Schaut ins Licht des Drachen, denn es wird Euren Abstieg ins Wissen leiten."

### Schätze
Ein Charakter der den Turm durchsucht und einen Wurf auf [[Nachforschungen]] gegen [[Schwierigkeitsgrad|SG]] 12 besteht entdeckt einen losen Stein in der Nordwestwand. In dem Geheimfach dahinter findet sich ein [[Trank des Widerstands]] (Blitz) und eine Geldbörse mit 10 GM.

## D5: Sternwartenturm
>[!quote] Dieser Turm ragt höher als der Rest der Sternwarte. Seine Hauptetage befindet sich ca. 15m über dem Meeresspiegel und damit ca. 5m über der Rotunde. Eine primitive Seilwinde würde installiert, vermutlich um den Kobolden nach oben zu verhelfen.

>[!quote] Lichtstrahlen tanzen durch die Überreste einer Buntglaskuppel und werfen einen bunten Schimmer auf die bröckeligen Marmorwände. Auf dem staubigen Boden sind noch die goldenen Linien und Juwelenintarsien einer detaillierten Sternkarte zu erkennen. Vier berobte Alabasterstatuen umstellen den Raum. Ihr Ausdruck ist nicht mehr zu deuten.

### Verborgener Eingang
- Statuen können auf ihrem Sockel gedreht werden
- Wurf auf [[Wahrnehmung]] gegen [[Schwierigkeitsgrad|SG]] 15 enthüllt Schleifspuren auf dem Sockel der Statuen
- Wurf auf [[Nachforschungen]] gegen [[Schwierigkeitsgrad|SG]] 15 um Drachen-Konstellation zu entdecken. ([[Vorteil und Nachteil|Vorteil]] wenn Buch dazu benutzt wird)
- wenn alles Statuen auf das richtige Sternbild weisen senkt sich eine Wendeltreppe in den Boden

### Schätze
Der Hort von Funkenschinder enthält folgendes:
- 4500 KM (450 GM, 90 Pfund)
- 2200 SM (220 GM, 44 Pfund)
- 130 GM (2,6 Pfund)
- 5 blassblaue [[Quartz]]kristalle (je 10 GM)
- 5 blaue [[Jaspis]]e (je 50 GM)
- ein wasserfester Lederbeutel mit einem Fächer aus blauer Seide mit blauem Edelsteinsand bestäubt
- eine grobe Flöte
- eine Sanduhr mit glitzerndem Sand
- ein Satz von sieben Kerzenleuchtern

## D6: Geheime Bibliothek
> [!quote] Abgestandene Luft mit dem Geruch nach altem Pergament füllt euch die Nasen. Die Wände stehen mit Regalen voll, die vor alten Folianten und Schriftrollen schier zu bersten scheinen. Vitrinen sind zusammengebrochen und haben ihren Inhalt auf dem Boden verteilt.

- Wurf auf [[Nachforschungen]] gegen [[Schwierigkeitsgrad|SG]] 15 oder der Zauber [[Magie entdecken]] enthüllt folgende Schätze:
	- [[Streitaxt]] +1
	- [[Magische Schriftrolle]] mit dem Zauber [[Person bezaubern]]

## Drachenruh

### Runara
- dankt der Gruppe dass sie Funkenschinder besiegt haben aber bedauert den Tod des Drachen
- lädt sie ein sich in Drachenruh niederzulassen
- kann ihnen keine große Belohnung anbieten, aber vielleicht bekommen sie auf dem Festland etwas dafür

### Myla
- bedauert den Tod von Mek (und Min)
- kann den Drachenodem reparieren und verbessern