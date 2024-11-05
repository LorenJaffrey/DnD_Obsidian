``` dataviewjs
var merkmale = dv.current().Merkmale;
var bonusaktionen = [];
var bonusaktionenString = "#### Bonusaktionen";
var aktuellesMerkmal;

if (merkmale) {
	for (var i = 0, j = merkmale.length; i<j; i++) {
		aktuellesMerkmal = dv.page(merkmale[i]);
		if (typeof(aktuellesMerkmal.Einsatz) == "object") {
			if (dv.page(aktuellesMerkmal.Einsatz).file.name == dv.parse("[[Bonusaktion]]").path)  {
				bonusaktionen.push(merkmale[i]);
			}
		}
	}
	
	if (bonusaktionen.length > 0) {
		for (var i = 0, j = bonusaktionen.length; i<j; i++) {
			bonusaktionenString +=  "\n - " + bonusaktionen[i];
		}
	}
	dv.span(bonusaktionenString);
}
```