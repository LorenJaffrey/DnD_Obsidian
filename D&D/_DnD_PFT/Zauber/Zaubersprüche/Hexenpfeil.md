---
aliases:
  - Witch Bolt
tags:
  - Zauber/Offensiv
Grad: 1
Schule: "[[Hervorrufungszauber|Hervorrufung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 9 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: ein Zweig von einem Baum, der vom Blitz getroffen worden ist
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Schaden: 1d12
Schadensart: "[[Blitzschaden]]"
Ziel: Einzel
Klassen:
  - "[[Zauberer]]"
---
# `=this.file.name`
*Zauber des `=this.Grad`. Grades der `=this.Schule` `=choice(this.Ritual,"([[Ritual]])", "")`*

Zeitaufwand: `=this.Zeitaufwand`
Reichweite: `=this.Reichweite`
Komponenten: `=choice(this.Verbal, choice(this.Geste, choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]], [[Zaubergesten|Geste (G)]]"), choice(this.Material, "[[Verbale Zauberkomponenten|Verbal (V)]], [[Materialkomponenten|Material (M)]]", "[[Verbale Zauberkomponenten|Verbal (V)]]")), choice(this.Geste, choice(this.Material, "[[Zaubergesten|Geste (G)]], [[Materialkomponenten|Material (M)]]", "[[Zaubergesten|Geste (G)]]"),	choice(this.Material, "[[Materialkomponenten|Material (M)]]", "")))` `=choice(this.Materialkosten, "(", "")` `=this.Materialkosten` `=choice(this.Materialkosten, ")", "")`
Wirkungsdauer: `=choice(this.Konzentration, "[[Konzentration]], bis zu ", "")` `=this.Dauer`

## Beschreibung
*Ein Strahl knisternder, blauer Energie schießt auf eine Kreatur in Reichweite und erschafft einen anhaltenden Bogen aus Blitzen zwischen dir und dem Ziel.*

Führe einen [[Fernkampfangriff|Fernkampf]]-Zauberangriff gegen diese Kreatur aus. 
Bei einem Treffer erleidet sie 1W12 [[Blitzschaden]]. 
Außerdem kannst du für die Wirkungsdauer in jedem deiner Züge deine [[Aktion]] verwenden, um dem Ziel automatisch 1W12 [[Blitzschaden]] zuzufügen. 
Der Zauber endet, wenn du deine [[Aktion]] für eine andere Handlung verwendest oder sich das Ziel außerhalb der Reichweite des Zaubers oder in [[Deckung#Vollständige Deckung|Vollständiger Deckung]] befindet.

### Auf höheren Graden
Wenn du diesen Spruch mit einem [[Zauberplätze|Zauberplatz]] des 2. oder eines höheren [[Zaubergrad|Grades]] wirkst, steigt der Initialschaden für jeden [[Zaubergrad|Grad]] über den 1. hinaus um 1W12.

Quelle: Players Handbook, Seite: 240