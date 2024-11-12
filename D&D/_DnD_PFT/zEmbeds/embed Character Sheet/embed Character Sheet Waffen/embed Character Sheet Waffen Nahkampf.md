```dataviewjs
try {
    // Check if the "Waffen" metadata includes "Nahkampf"
    if (dv.current().Waffen && isMeleeWeapon(dv.current().Waffen)) {

        dv.header(3, "Nahkampfwaffen");

        dv.table(
            ["Waffe", "Reichweite", "Angriff", "Schaden", "Schadensart", "Eigenschaften"],
            dv.pages("#Gegenstand/Waffe/Klasse/Nahkampfwaffe")
                .where(p => dv.current().Waffen && dv.current().Waffen.some(link => link.path === p.file.path) && p.tags.includes('Gegenstand/Waffe/Klasse/Nahkampfwaffe'))
                .sort(page => page.file.name)
                .map(page => {
                    // Calculate Angriff
                    let magicStat = dv.page(dv.current().Hintergrund.Klasse).Zauberattribut ? dv.page(dv.current().Hintergrund.Klasse).Zauberattribut.fileName() : null;
                    let attackStat = dv.current().Attribute.Stärke;
                    if (page?.Eigenschaften?.some(link => link?.path?.includes("Gegenstände/Waffen/Waffeneigenschaften/Finesse.md"))){
	                    attackStat = Math.max(attackStat, dv.current().Attribute.Geschicklichkeit);
                    }
                    if (page?.Eigenschaften?.some(link => link?.path?.includes("Gegenstände/Waffen/Waffeneigenschaften/Magische Präzision.md"))){
	                    attackStat = Math.max(attackStat, dv.current().Attribute[magicStat]);
					}
                    let attackModifier = Math.floor((attackStat - 10) / 2);
                    let proficiencyBonus = Math.ceil(dv.current().Stufe / 4) + 1;
                    let attackRoll = `\`dice:1d20+${attackModifier + proficiencyBonus + (page?.Angriffsbonus ?? 0)}\``;

                    // Calculate Schaden
                    let damageRoll = `\`dice:${page.Schaden}+${attackModifier}\``;

                    return [
                        page.file.link,
                        page.Reichweite,
                        attackRoll,
                        damageRoll,
                        page.Schadensart,
                        page.Eigenschaften
                    ];
                })
        );
    }

    function hasTag(page, targetTag) {
        return page?.tags && page?.tags?.some(tag => tag === targetTag);
    }

    function isMeleeWeapon(weaponList) {
        let isMeleeWeapon = false;

        for (let item of dv.current().Waffen) {
            let page = dv.page(item.path);
            let targetTag = "Gegenstand/Waffe/Klasse/Nahkampfwaffe";

            // Call the function and store the result
            isMeleeWeapon = hasTag(page, targetTag);

            if (isMeleeWeapon) {
                break;
            }
        }

        return isMeleeWeapon
    }

} catch (error) {
    console.error("An error occurred in DataviewJS:", error);
}
```


