``` dataviewjs
var merkmale = dv.current().Merkmale;
var reaktionen = [];
var reaktionenString = "#### Reaktionen";
var aktuellesMerkmal;

if (merkmale) {
	for (var i = 0, j = merkmale.length; i<j; i++) {
		aktuellesMerkmal = dv.page(merkmale[i]);
		if (typeof(aktuellesMerkmal.Einsatz) == "object") {
			if (dv.page(aktuellesMerkmal.Einsatz).file.name == dv.parse("[[Reaktion]]").path)  {
				reaktionen.push(merkmale[i]);
			}
		}
	}

	if (reaktionen.length > 0) {
		for (var i = 0, j = reaktionen.length; i<j; i++) {
			reaktionenString +=  "\n - " + reaktionen[i];
		}
	}
	
	dv.span(reaktionenString);
}
```