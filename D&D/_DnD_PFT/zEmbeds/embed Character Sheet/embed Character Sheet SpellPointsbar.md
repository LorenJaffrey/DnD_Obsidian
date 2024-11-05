```dataviewjs 
const maxSpellPoints = (dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad1*2)+(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad2*3)+
(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad3*5)+(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad4*6)+
(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad5*7)+(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad6*9)+
(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad7*10)+(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad8*11)+
(dv.page(dv.current().Hintergrund.Klasse).Zauberplätze["Stufe"+dv.current().Stufe].Grad9*13);


const currentSpellPoints = dv.current().InputData.Zauberpunkte;
const percentValue2 =  Math.round(currentSpellPoints / (maxSpellPoints / 100));
 
 const metaBindCode = `<div style="display: flex; align-items: center; width: 100%; position: relative;"><div style="flex: 1; position: relative;"><progress id="spellpoints" max="${maxSpellPoints}" value="${currentSpellPoints}" style="width: 100%; height: 20px; --progress: rgb(57, 159, 148) !important;"></progress><span id="percentage3" style="position: absolute; left: 50%; top: 50%; transform: translate(-50%, -70%); color: white; font-weight: bold;">Zauberpunkte</span></div><div style="width: 60px; text-align: center;">${percentValue2}%</div></div>`; 
dv.el('div', metaBindCode); 
```