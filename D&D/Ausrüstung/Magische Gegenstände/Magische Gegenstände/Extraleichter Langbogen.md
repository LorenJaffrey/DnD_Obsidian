---
tags:
- Magischer_Gegenstand/Waffe/Bogen
Art: "[[Magische Waffe]]"
Seltenheit: "ungewöhnlich"
Einstimmung: true
Kosten: 250 GM
Voraussetzung:
Verflucht: false
---
# `=this.file.name`
> [!infobox]
> ###### Eigenschaften
> | Eigenschaft |  |
> | ---- | ---- |
> | Art | `=this.Art` |
> | Seltenheit | `=this.Seltenheit` |
> | Einstimmung | `=choice(this.Einstimmung, "Ja", "Nein")` |
> | Verflucht | `=choice(this.Verflucht, "Ja", "Nein")` |
> | Voraussetzung | `=this.Voraussetzung` |
> | Kosten | `=this.Kosten` |

Der Träger erhält einen +1 Bonus auf Initiative-Würfe.