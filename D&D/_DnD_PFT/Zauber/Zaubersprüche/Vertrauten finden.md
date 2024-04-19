---
aliases:
  - Find Familiar
tags:
  - Zauber
Grad: 1
Schule: "[[Beschwörungszauber]]"
Zeitaufwand: 1h
Reichweite: 3 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: Holzkohle, Weihrauch und Kräuter im Wert von 10 GM, die in einer Feuerschale aus Messing von Flammen verzehrt werden
Dauer: unmittelbar
Konzentration: false
Ritual: true
Skalierbar: false
Klassen:
- "[[Magier]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du erhältst die Dienste eines Vertrauten, eines Geistes, der die Gestalt eines der folgenden Tiere deiner Wahl annimmt: 
- Eidechse
- Eule
- Falke
- Fisch (Quipper)
- Fledermaus
- Frosch (Kröte)
- Giftschlange
- Katze
- Krabbe
- Oktopus
- Rabe
- Ratte
- Seepferdchen
- Spinne
- Wiesel

Der Vertraute erscheint in einem nicht besetzten Bereich in Reichweite und besitzt die Spielwerte der ausgewählten Gestalt, ist jedoch ein [[Celestische Wesen|Celestisches Wesen]], ein [[Feenwesen]] oder ein [[Unholde|Unhold]] (deine Wahl) und kein [[Tiere|Tier]].
Dein Vertrauter agiert unabhängig von dir, folgt aber immer deinen Befehlen. Im Kampf würfelt er seine eigene [[Initiative]] und handelt selbstständig. Ein Vertrauter kann nicht angreifen, aber alle anderen [[Aktionen]] ausführen.

Fallen die [[Trefferpunkte]] des Vertrauten auf 0, verschwindet er und lässt keine physische Form zurück. Er erscheint wieder. wenn du den Zauber erneut wirkst. 
Als [[Zug#Aktion]] kannst du deinen Vertrauten kurzzeitig fortschicken. Er verschwindet in einer Taschendimension, wo er auf deinen Ruf wartet. Alternativ kannst du ihn für immer fortschicken. Solange der Vertraute fortgeschickt ist, kannst du eine [[Zug#Aktion]] verwenden, um ihn in einem nicht besetzten Bereich innerhalb von 9 m erscheinen zu lassen. Wenn die [[Trefferpunkte]] des Vertrauten auf 0 fallen oder er in der Taschendimension verschwindet, bleiben in seinem Bereich seine Kleidung und Ausrüstung zurück.

Solange sich dein Vertrauter innerhalb von 30 m aufhält, bist du in der Lage, telepathisch mit ihm zu kommunizieren. Außerdem kannst du als [[Zug#Aktion]] bis zum Beginn deines nächsten [[Zug]] durch die Augen und Ohren deines Vertrauten sehen und hören, als würdest du dich an seinem Standort befinden. Dabei stehen dir alle besonderen Sinne des Vertrauten zur Verfügung. Während dieser Zeit bist du [[Taub]] und [[Blind]] für deine eigene Umgebung.

Du kannst nicht mehr als einen Vertrauten gleichzeitig haben.
Wenn du diesen Zauber wirkst, obwohl du bereits über einen Vertrauten verfügst, lässt du ihn stattdessen eine neue Gestalt annehmen. Wähle eins der oben genannten Tiere, in das sich dein Vertrauter verwandelt.
Wenn du außerdem einen Zauber mit der Reichweite Berührung wirkst, kann dein Vertrauter diesen überbringen, als hättest du ihn gewirkt. Dein Vertrauter muss sich innerhalb von 30 m von dir befinden und seine [[Zug#Reaktion]] verwenden, um den Zauber zu überbringen, wenn du ihn wirkst. Erfordert der Zauber einen [[Zauberangriffswürfe|Zauberangriffswurf]], verwende deinen Angriffsmodifikator für den Wurf.