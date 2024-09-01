---
aliases:
tags:
  - Zauber/Offensiv
Grad: 6
Schule: "[[Beschwörungszauber|Beschwörung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: true
Materialkosten: ein Saphir im Wert von 1.000 GM
Dauer: bis der Zauber gebannt wird
Konzentration: true
Ritual: true
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
Du berührst einen Gegenstand, der 10 Pfund oder weniger wiegt und dessen größte Ausdehnung maximal 1,80 m beträgt. Der Zauber hinterlässt ein unsichtbares Mal auf der Oberfläche des Gegenstands und schreibt dessen Namen auf den Saphir, den du als Materialkomponente nutzt. Für jeden verzauberten Gegenstand benötigst du einen eigenen Saphir. 
Anschließend kannst du zu einem beliebigen Zeitpunkt deine Aktion verwenden, um den Namen des Gegenstands auszusprechen und den Saphir zu zerschmettern. Der Gegenstand erscheint sofort in deiner Hand, unabhängig von seiner physischen oder planaren Entfernung, und der Zauber endet. Wenn eine andere Kreatur den Gegenstand trägt oder in der Hand hält, wird er nicht zu dir transportiert. Aber du erfährst, wer die Kreatur ist, die den Gegenstand in ihrem Besitz hat, und wo sie sich in diesem Augenblick ungefähr aufhält. 
**Magie bannen** oder ein ähnlicher Effekt, der erfolgreich auf den Saphir gewirkt wird, beendet den Zauber.