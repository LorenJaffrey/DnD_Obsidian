---
aliases:
  - Contagion
tags:
  - Zauber
Grad: 5
Schule: "[[Nekromantiezauber|Nekromantie]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: Berührung
Verbal: true
Geste: true
Material: false
Materialkosten: 
Dauer: 7 Tage
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
Wirkungsdauer:  `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Deine Berührung löst Krankheiten aus.*
Führe einen Nahkampf-Zauberangriff gegen eine Kreatur innerhalb deiner Reichweite aus. 
Bei einem Treffer verursachst du bei der Kreatur eine der unten beschriebenen [[Krankheiten]] deiner Wahl.

Am Ende jedes seiner Züge muss das Ziel einen [[Rettungswurf]] auf [[Konstitution]] ausführen. 
Nach drei gescheiterten [[Rettungswurf|Rettungswürfen]] hält die Krankheit für die Wirkungsdauer an und die Kreatur führt keine [[Rettungswurf|Rettungswürfe]] mehr aus. 
Nach drei erfolgreichen [[Rettungswurf|Rettungswürfen]] erholt sich die Kreatur von der [[Krankheiten|Krankheit]] und der Zauber endet.

Da dieser Zauber beim Ziel eine natürliche [[Krankheiten|Krankheit]] verursacht, sind alle Effekte wirksam, die [[Krankheiten]] heilen oder anderweitig lindern.

### Krankheiten
- [[Blendende Krankheit]]
- [[Fleischfäule]]
- [[Gedankenfeuer]]
- [[Krampfanfall]]
- [[Schleimiges Verderben]]
- [[Schmutzfieber]]