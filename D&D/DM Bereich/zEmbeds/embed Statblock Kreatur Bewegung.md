```dataviewjs
const movement = dv.current().Bewegung;
var string = "|  |  | \n | --- | --- |";
for (var key in movement) {
	if(movement[key] > 0) {
		if (string.length > 0) {
			string += " \n "
		}
	string += ("|  [[" + key + "]] | " + movement[key] + "m (" + movement[key]/1.5 + " Kästchen) |");
	}
}
dv.paragraph(string);
```