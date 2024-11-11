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
                    let attackStat = page?.Eigenschaften?.some(link => link?.path?.includes("Gegenstände/Waffen/Waffeneigenschaften/Finesse.md"))
                        ? dv.current().Attribute.Geschicklichkeit
                        : dv.current().Attribute.Stärke;

                    let attackModifier = Math.floor((attackStat - 10) / 2);
                    let attackRoll = `\`dice:1d20+${attackModifier + Math.ceil(dv.current().Stufe / 4) + 1 + (page?.Angriffsbonus ?? 0)}|none|noform\``;

                    // Calculate Schaden
                    let damageModifier = Math.floor((attackStat - 10) / 2);
                    let damageRoll = `\`dice:${page.Schaden}+${damageModifier}|none|noform\``;

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


