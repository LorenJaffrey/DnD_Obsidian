---
alias: 
tags: 
  - Zauber
Grad: 7
Schule: "[[Illusionszauber|Illusion]]"
Zeitaufwand: 10 Minuten
Reichweite: Sicht
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: 10 Tage
Konzentration: false
Ritual: false
Skalierbar: false
Schaden: 
Schadensart: 
Ziel: 
Klassen:
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"(Ritual)", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
Du lässt das Gelände in einem Gebiet von 1,5 x 1,5 km wie eine andere Art von Gelände aussehen, klingen, riechen und beeinflusst sogar, wie es sich anfühlt. Die grundsätzliche Gestalt der Landschaft bleibt aber dieselbe. Offene Felder oder eine Straße können wie ein Sumpf, ein Hügel, eine Erdspalte oder eine andere Art von schwierigem oder unpassierbarem Gelände erscheinen, ein Tümpel wie eine grasige Wiese, ein Abhang wie ein sanftes Gefälle oder eine mit Felsen übersäte Schlucht wie eine breite, flache Straße. Gleichermaßen bist du in der Lage, das Aussehen von Bauwerken zu verändern oder sie entstehen zu lassen, wo es keine gibt. Der Zauber kann keine Kreaturen verkleiden, verbergen oder hinzufügen. Die Illusion umfasst hörbare, visuelle, berührbare und olfaktorische Elemente, sodass sie freies Gelände in schwieriges verwandeln kann (und andersherum) oder anderweitig die Bewegung durch das Gebiet zu behindern vermag. Jedes Stück illusionäres Gelände (wie ein Fels oder ein Stock). das aus dem Bereich des Zaubers entfernt wird, verschwindet sofort. Kreaturen unter dem Einfluss von Wahrer Blick durchschauen die Illusion und erkennen die wahre Gestalt der Landschaft. Alle anderen Elemente der Illusion bleiben aber bestehen. Selbst wenn sich die Kreatur also der Illusion bewusst ist, kann sie noch immer physisch mit ihr interagieren.