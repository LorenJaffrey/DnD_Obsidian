---
aliases:
  - 
tags:
  - Zauber/Offensiv
Grad: 6
Schule: "[[Verwandlungszauber|Verwandlung]]"
Zeitaufwand: "[[Aktion]]"
Reichweite: 18 Meter
Verbal: true
Geste: true
Material: true
Materialkosten: ein Magnetstein und eine Prise Staub
Dauer: unmittelbar
Konzentration: false
Ritual: false
Skalierbar: true
Schaden: 10d6+40
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
Ein dünner grüner Strahl fährt aus deinem ausgestreckten Finger auf ein Ziel in Reichweite, das du sehen kannst. Das Ziel kann eine Kreatur, ein Gegenstand oder ein Gebilde aus magischer Energie sein, wie die Mauer, die durch den Zauber Energiewand erschaffen wird. Eine Kreatur, die Ziel dieses Zaubers ist, muss einen Geschicklichkeitsrettungswurf ablegen. Bei einem Misserfolg erleidet sie 10W6+40 Energieschaden. Reduziert dieser Schaden das Ziel auf 0 Trefferpunkte, wird es aufgelöst. Eine aufgelöste Kreatur und alles, was sie trägt und in Händen hält (mit Ausnahme von magischen Gegenständen), zerfallen zu einem Haufen feinen, grauen Staubs. Die Kreatur kann nur durch die Zaubersprüche Wahre Auferstehung oder Wunsch wieder zum Leben erweckt werden. Alle nicht-magischen Gegenstände oder Gebilde aus magischer Energie der Größenkategorie groß oder kleiner werden von diesem Zauber automatisch aufgelöst. Ist das Ziel riesig oder größer, löst der Zauber einen Teil davon auf, der einem Würfel mit 3 m Kantenlänge entpricht. Magische Gegenstände sind von diesem Zauber nicht betroffen.

## Auf höheren Graden
Wenn du diesen Spruch mit einem Zauberplatz des 7. oder eines höheren Grades wirkst, steigt der Schaden für jeden Grad über den 6. hinaus um 3W6.