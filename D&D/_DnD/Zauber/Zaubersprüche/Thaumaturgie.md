---
aliases: 
- Thaumaturgy
tags: 
- Zauber
Grad: 0
Schule: "[[Verwandlungszauber|Verwandlung]]"
Zeitaufwand: "[[Zug#Aktion]]"
Reichweite: 9 Meter
Verbal: true
Geste: false
Material: false
Materialkosten: 
Dauer: 1m
Konzentration: false
Ritual: false
Skalierbar: false
Klassen:
- "[[Kleriker]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Du manifestierst ein kleines Wunder in Reichweite, ein Zeichen übernatürlicher Macht.*

Du kannst einen der folgenden magischen Effekte erzeugen:
- Deine Stimme dröhnt für 1 Minute dreimal so laut wie normal.
- Du lässt Flammen flackern, heller oder dunkler werden oder die Farbe wechseln. Der Effekt hält 1 Minute an.
- Du erzeugst für 1 Minute harmlose Erschütterungen des Bodens.
- Du erschaffst ein kurzes Geräusch, das von einem Punkt deiner Wahl in Reichweite ertönt, wie das Grollen von Donner, den Ruf eines Raben oder ein unheilvolles Flüstern.
- Du lässt eine nicht verriegelte Tür oder ein Fenster auffliegen oder zuschlagen.
- Du änderst für 1 Minute das Aussehen deiner Augen.

Wenn du diesen Zauber mehrmals wirkst, können bis zu drei der nicht sofortigen Effekte gleichzeitig aktiv sein. Du kannst solche Effekte als [[Zug#Aktion]] aufheben.

## Zauberlisten
- [[Kleriker]]