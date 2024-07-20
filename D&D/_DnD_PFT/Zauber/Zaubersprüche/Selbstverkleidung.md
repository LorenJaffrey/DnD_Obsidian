---
aliases: 
  - Disguise Self
tags: 
  - Zauber
Grad: 1
Schule: "[[Illusionszauber|Illusion]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: selbst
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: 1h
Konzentration: false
Ritual: false
Skalierbar: false
Schaden: 
Schadensart: 
Ziel:
Klassen:
  - "[[Barde]]"
  - "[[Magier]]"
  - "[[Zauberer]]"
  - "[[Magieschmied]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Mit diesem Zauber veränderst du dein Aussehen - inklusive deiner Kleidung, Rüstung, Waffen und anderen Besitztümer an deiner Person.*

Er bleibt für die Wirkungsdauer bestehen, wenn du keine [[Aktion]] verwendest, um ihn vorzeitig aufzuheben.

Du kannst dich bis zu 30 cm kleiner oder größer erscheinen lassen sowie dick oder dünn beziehungsweise irgendetwas dazwischen. 
Deinen grundlegenden Körpertyp kannst du nicht ändern, du musst also eine Gestalt annehmen, welche die gleiche Anordnung von Gliedmaßen besitzt. 
Ansonsten bestimmst du, wie die Illusion aussieht.

Die Veränderungen durch diesen Zauber halten einer körperlichen Untersuchung nicht stand. Nutzt du den Spruch beispielsweise, um deiner Kleidung einen Hut beizufügen, durchdringen Gegenstände diesen einfach. 
Jeder, der ihn berührt, würde nichts fühlen oder nur deinen Kopf und deine Haare spüren. 
Lässt du dich dünner erscheinen, als du bist, würde die Hand von jemandem, der dich berühren will, gegen dich stoßen, obwohl sie scheinbar noch in der Luft schwebt.

Eine Kreatur kann ihre [[Aktion]] verwenden, um dich zu untersuchen. Sie legt einen Wurf auf [[Nachforschungen]] gegen den SG zum Widerstehen deiner Zauber ab. 
Bei Erfolg bemerkt sie, dass du auf irgendeine Art verkleidet bist.