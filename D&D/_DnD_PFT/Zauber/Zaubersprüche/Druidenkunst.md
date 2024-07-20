---
aliases: 
  - Druidcraft
tags: 
  - Zauber
Grad: 0
Schule: "[[Verwandlungszauber|Verwandlung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 9 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: false
Schaden: 
Schadensart: 
Ziel: AoE
Klassen:
  - "[[Druide]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Du sprichst flüsternd mit den Geistern der Natur.*

Du erzeugst innerhalb der Reichweite einen der folgenden Effekte:
- Du erschaffst einen harmlosen sensorischen Effekt, der das Wetter an deinem Aufenthaltsort für die nächsten 24 Stunden vorhersagt. 
   Der Effekt halt 1 Runde lang an und könnte sich als goldene Kugel für einen klaren Himmel, als Wolke für Regen, als fallende Schneeflocken für Schnee oder Ähnliches manifestieren.
- Du bewirkst, dass augenblicklich eine Blume erblüht, eine Samenkapsel sich öffnet oder eine Blattknospe aufblüht.
- Du erschaffst einen harmlosen sensorischen Effekt, wie fallende Blätter, einen Windhauch, die Geräusche eines kleinen Tieres oder den leichten Geruch eines Stinktiers. 
   Der Effekt muss in einen Würfel mit 1,50 m Kantenlänge passen.
- Du kannst augenblicklich eine Kerze, eine Fackel oder ein kleines Lagerfeuer entzünden oder löschen.