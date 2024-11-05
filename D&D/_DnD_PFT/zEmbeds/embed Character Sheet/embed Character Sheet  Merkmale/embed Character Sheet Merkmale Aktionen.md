``` dataviewjs
var merkmale = dv.current().Merkmale;
var aktionen = [];
var aktionenString = "#### Aktionen";
var aktuellesMerkmal;

if (merkmale) {
	for (var i = 0, j = merkmale.length; i<j; i++) {
		aktuellesMerkmal = dv.page(merkmale[i]);
		if (typeof(aktuellesMerkmal.Einsatz) == "object") {
			if (dv.page(aktuellesMerkmal.Einsatz).file.name == dv.parse("[[Aktion]]").path)  {
				aktionen.push(merkmale[i]);
			}
		}
	}
	
	if (aktionen.length > 0) {
		for (var i = 0, j = aktionen.length; i<j; i++) {
			aktionenString += "\n - " + aktionen[i];
		}
	}
	dv.span(aktionenString);
}
```