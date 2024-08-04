---
aliases:
  - 
tags:
  - Zauber
Grad: 5
Schule: "[[Illusionszauber|Illusion]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 9 Meter
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: 8 Stunden
Konzentration: false
Ritual: false
Skalierbar: false
Schaden: 
Schadensart: 
Ziel: 
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Dieser Zauber erlaubt es dir, das Aussehen einer beliebigen Anzahl von Kreaturen zu ändern, die sich in Reichweite befinden und die du sehen kannst. Du gibst jedem Ziel ein neues, illusionäres Erscheinungsbild. Ein unwilliges Ziel kann einen Charismarettungswurf ablegen und wird bei Erfolg nicht von
dem Effekt betroffen. Der Zauber verbirgt sowohl die physische Erscheinung als auch Kleidung, Rüstung, Waffen und Ausrüstung des Ziels. Du kannst jede Kreatur bis zu 30 cm kleiner oder größer erscheinen lassen sowie dick oder dünn beziehungsweise irgendetwas dazwischen. Ihr grundsätzlicher
Körpertyp ist nicht änderbar, du musst also eine Gestalt mit der gleichen Anordnung von Gliedmaßen wählen. Ansonsten bestimmst du, wie die Illusion aussieht. Der Zauber bleibt für die Wirkungsdauer bestehen, wenn du keine Aktion verwendest, um ihn früher aufzuheben. Die Veränderungen durch diesen Zauber halten einer körperlichen Untersuchung nicht stand. Nutzt du den Spruch beispielsweise, um der Kleidung einer Kreatur einen Hut beizufügen, durchdringen Gegenstände diesen einfach. Jeder, der ihn berührt, würde nichts fühlen oder nur den Kopf und die Haare der Kreatur spüren. Lässt du dich dünner erscheinen, als du bist, würde die Hand von jemandem, der dich berühren will, gegen dich stoßen, obwohl sie scheinbar noch in der Luft schwebt. Eine Kreatur kann ihre Aktion verwenden, um ein Ziel zu untersuchen. Sie legt einen Wurf auf Intelligenz (Nachforschungen) gegen den SG zum Widerstehen deiner Zauber ab. Bei Erfolg bemerkt sie, dass das Ziel auf irgendeine Art verkleidet ist.
