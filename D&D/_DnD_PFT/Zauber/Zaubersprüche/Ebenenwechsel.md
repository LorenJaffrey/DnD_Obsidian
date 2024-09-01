---
aliases:
tags:
  - Zauber/Offensiv
Grad: 7
Schule: "[[Beschwörungszauber|Beschwörung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: true
Materialkosten: ein gegabelter Metallstab im Wert von mindestens 250 GM, eingestimmt auf die gewünschte Existenzebene
Dauer: unmittelbar
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
Du und bis zu acht bereitwillige Kreaturen, die sich in einem Kreis an den Händen halten, werden auf eine andere Existenzebene transportiert. Bestimme einen allgemeinen Zielort, wie die Messingstadt auf der Elementarebene des Feuers oder den Palast von Dispater auf der zweiten Ebene der Neun Höllen, und ihr erscheint in oder nahe diesem Ziel (nach Wahl des SL). Versucht ihr beispielsweise, die Messingstadt zu erreichen, könntet ihr dort in der Straße des Stahls eintreffen, vor dem Tor der Asche oder an einem Ort, von dem aus ihr über das Feuermeer auf die Stadt blickt.

Wenn du die Sigillensequenz eines Teleportationskreises zu einer anderen Existenzebene kennst, kann der Zauber euch auch zu diesem Kreis bringen. Ist der Teleportationskreis zu klein, um alle transportierten Kreaturen aufzunehmen, erscheinen sie in den nächstliegenden nicht besetzten Bereichen neben dem Kreis. Du kannst diesen Zauber auch verwenden, um eine unwillige Kreatur auf eine andere Ebene zu verbannen. Wähle eine Kreatur in Reichweite und führe einen Nahkampf-Zauberangriff gegen sie aus. Bei einem Treffer muss das Ziel einen Charismarettungswurf ablegen. Misslingt dieser, wird die Kreatur an einen zufälligen Ort einer von dir gewählten Existenzebene transportiert. Eine Kreatur, die auf diese Weise transportiert wurde, muss ihren Weg zurück auf deine aktuelle Existenzebene selbst finden.