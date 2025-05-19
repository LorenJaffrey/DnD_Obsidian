```dataviewjs
const page = dv.current();

const input = page.InputData ?? {};
const attr = page.Attribute ?? {};
const def = page.Verteidigung ?? {};

const geschickMod = Math.floor(((attr.Geschicklichkeit ?? 10) - 10) / 2);
const zusatzRüstung = def.Zusätzliche_Rüstung ?? 0;

let rüstungsklasse = 0;
if (input.MagierRüstung === true) {
    const schild = def.Schild?.RP ?? def.Schild ?? 0;
    rüstungsklasse = 13 + geschickMod + schild + zusatzRüstung;
} else {
    const natRüstung = def.Natürliche_Rüstung ?? 0;
    const rüstungRP = def.Rüstung?.RP ?? def.Rüstung ?? 0;
    rüstungsklasse = natRüstung + geschickMod + rüstungRP + zusatzRüstung;
}

// Schadensreduktion berechnen
const rüstungSR = def.Rüstung?.SR ?? 0;
const schildSR = def.Schild?.SR ?? 0;
const schadensreduktion = rüstungSR + schildSR;

// Markdown-Tabelle erzeugen
let table = `| [[Rüstungsklasse]] | [[Schadensreduktion]] |\n`;
table += `| :--------------------: | :------------------------: |\n`;
table += `| ${rüstungsklasse}           | ${schadensreduktion}                  |\n`;

dv.paragraph(table);

```

|    Beschreibung     |           Bonus (bereits eingerechnet)           |
|:-------------------:|:------------------------------------------------:|
| Zusätzliche Rüstung | `INPUT[number:Verteidigung.Zusätzliche_Rüstung]` |