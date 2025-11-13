---
tags:
  - Regeln/Nimble/WIP
---
# `=this.file.name`
Dein Held ist das Mittel, mit dem du deinen Abdruck in der Welt hinterlassen wirst. 
So erschaffst du deinen eigenen Helden:

## Schritt 1: Wähle deine Klasse
Dies hat den größten Einfluss auf deine weiteren Entscheidungen und darauf, wie dein Charakter mit der Welt interagiert:
```dataview
TABLE WITHOUT ID

file.link AS "Klasse",
Beschreibung

FROM #Regeln/Nimble/Charakter/Klasse 

SORT file.name
```

- **[[BERSERKER]].** Unaufhaltsame Kraft aus Zorn und Zerstörung.
- **[[GAUNER]].** Heimtückischer, hinterhältiger, schmutzig kämpfender Schurke.
- **[[KOMMANDANT]].** Meisterstratege, Anführer und Waffenexperte.
- **[[JÄGER]].** Findiger Überlebenskünstler, Bogenschütze und erfahrener Fährtenleser.
- **[[ARKANIST]].** Beherrsche Feuer, Eis und Blitze.
- **[[PALADIN]].** Treuer Wächter, Beschützer und Rächer der Schwachen.
- **[[SCHATTENRUFER]].** Beschwöre Horden entbehrlicher Diener.
- **[[KLERIKER]].** Meistre Leben und Tod. Führe einen treuen Begleiter.
- **[[KLANGWEBER]].** Inspirierende Präsenz, scharfer Verstand, schärfere Zunge.
- **[[DRUIDE]].** Gebieter über Wetter, Bestien und Natur.
- **[[WINDLÄUFER]].** Disziplinierter Kampfkünstler mit schnellen Händen und Füßen.

## Schritt 2: Wähle deine Herkunft
Wähle eine [[Abstammung]].
Wähle außerdem entweder aus den vorgefertigten [[Hintergründe|Hintergründen]]oder lege deine eigene Abenteuer-Motivation fest. 
Was hat deinen Helden angetrieben, ein Abenteurer zu werden? 
Wie kennst du die anderen Helden?

## Schritt 3: Fülle dein Charakterblatt aus
Benutze die [[Character Sheet Vorlage]].
Dieses Blatt hilft dir, Werte, Fähigkeiten, Ausrüstung und andere wichtige Informationen zu verwalten.

# Das Charakterblatt

## 1. Grundwerte & Attribute
Trage Charakterdetails ein: Name, [[Abstammung]], [[Klasse]], Stufe, Größe und Gewicht.
Markiere [[Vorteil und Nachteil|Vorteil]]  und [[Vorteil und Nachteil|Nachteil]] bei [[Rettungswurf|Rettungswürfen]] und wähle eine Werteverteilung. 
(Tipp: Setze die höchsten Zahlen in die Kernattribute deiner Klasse).

- **Standard:** +2, +2, +1, +0, +0, -1
- **Ausgeglichen:** +2, +1, +1, +1, +0, +0
- **Extrem (Min–Max):** +3, +1, +1, +1, -1, -1

> [!example]- Beispiel  
> [[Der Betrüger]] hat [[Geschicklichkeit|GE]] und [[Intelligenz|IN]] als seine Hauptwerte. 
> Mit der Min–Max-Verteilung könntest du +3 auf  [[Geschicklichkeit|GE]], +1 auf  [[Intelligenz|IN]], [[Charisma|CH]] und [[Konstitution|KO]]  und –1 auf  [[Stärke|ST]] und [[Weisheit|WE]]  setzen. 
> Markiere [[Vorteil und Nachteil|Vorteil]] für [[Geschicklichkeit|GE]]-[[Rettungswurf|Rettungswürfe]] und [[Vorteil und Nachteil|Nachteil]] für [[Weisheit|WE]]-[[Rettungswurf|Rettungswürfe]].

## 2. Fertigkeitspunkte
Auf Stufe 1 überträgst du deine [[Attribute|Attributsboni]] auf die jeweiligen [[Fertigkeiten]] (z. B. ein Held mit +2 [[Geschicklichkeit|GE]] trägt +2 bei [[Akrobatik]], [[Fingerfertigkeit]] und [[Heimlichkeit]] ein) und darf 6 weitere Punkte frei verteilen.

> [!example]- Beispiel  
> Wenn du –1 [[Intelligenz|IN]] hast, markiere  -1 bei [[Arkane Kunde]], [[Geschichte]], [[Nachforschungen]], [[Naturkunde]] und [[Religion]]. 
> Wiederhole das für deine anderen Attribute. 
> Mit den 6 Extrapunkten kannst du z. B. [[Heimlichkeit]] und [[Fingerfertigkeit]] je +3 erhöhen, 6 verschiedene Fertigkeiten  je +1 oder alle 6 Punkte in deine Lieblingsfertigkeit setzen.

## 3. Sekundäre Werte
Trage deine sekundären Werte ein:
- maximale [[Trefferpunkte]] 
- [[Trefferwürfel]] 
- [[Initiative|Initiativebonus]] (Standard: [[Geschicklichkeit|GE]])
- Größe
- [[Bewegungsrate]] (abhängig von der [[Abstammungen|Abstammung]])
- maximale [[Wunden]] (Standard: 6) 
- Inventarplätze (10 + [[Stärke]]) 

## 4. Ausrüstung & Geld
Helden beginnen auf Stufe 1 mit der für ihre [[Klasse]] und ihren [[Hintergründe|Hintergrund]] vorgeschriebenen Ausrüstung oder mit **50 GM**, um ihre Startausrüstung zu kaufen. 
Wenn du auf höherer Stufe beginnst, multipliziere den Betrag mit deiner Startstufe.

> [!faq]- Aber mein Charakter ist ein wohlhabender Adliger!  
> Kein Problem – dein Charakter hat momentan nur Zugang zu diesem Goldbetrag. 
> Warum sein Vermögen derzeit unerreichbar ist, liegt an dir und dem SL; es könnte ein guter Abenteueraufhänger sein, den vollen Reichtum freizuschalten.

## 5. Sprachen
Alle Helden sprechen [[Gemeinsprache]] (Standard). 
Jeder Punkt in [[Intelligenz|IN]] gewährt eine weitere bekannte [[Sprachen|Sprache]]. 

> [!tip]- GROFWINT DRAZLON!  
> Die Sprache einer anderen Kreatur zu sprechen kann Türen öffnen, die Waffen nicht können – wer bewaffnet ist, aber nicht kommunizieren kann, führt oft zum Kampf.

## 6. Weitere Fähigkeiten
Trage besondere Fähigkeiten ein, die du durch [[Klasse]], [[Abstammungen|Abstammung]], [[Hintergründe|Hintergrund]] oder ähnliche Quellen erhältst.

## 7. Inventarplätze
Jeder Held hat **10 + [[Stärke|ST]]** [[Inventarplätze]] für Ausrüstung und Beute (getragen, angelegt oder verpackt).  
* 1 Platz fasst eine einhändige Waffe, Schild, getragene Rüstung, Speerbündel, 500 GM oder 2 Tränke.  
* 2 Plätze fassen eine zweihändige Waffe, nicht getragene Rüstung oder ähnlich große Gegenstände.  
* Kleine zusammengehörige Dinge können in einem Slot gebündelt werden (z. B. Campingausrüstung: Seife, Decke, Bürste, Rationen).

> [!tip]- Über Munition  
> In den meisten Spielen musst du Munition nicht genau verfolgen. 
> Wenn du einen Köcher hast, hast du genug Pfeile. 
> Man geht davon aus, dass der Held Pfeile einsammelt, herstellt oder in einer Stadt nachkauft.

Alternativ kann der SL dir erlauben, alles zu tragen, was plausibel ist, ohne das genaue Buchführen.
- [ ] Inventar auslösen  [priority:: medium]