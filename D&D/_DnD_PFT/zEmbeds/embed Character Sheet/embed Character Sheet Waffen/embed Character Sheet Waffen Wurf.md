```dataviewjs
try {
    // Check if the "Waffen" metadata includes ranged throwable weapons
    if (dv.current().Waffen && isThrowableWeapon(dv.current().Waffen)) {

        dv.header(3, "Wurfwaffen");

        // Create table with headers
        dv.table(
            ["Waffe", "Min RW", "Gnd RW", "Max RW", "Angriff", "Schaden", "Schadensart", "Eigenschaften"],
            dv.pages("#Gegenstand/Waffe/Klasse/Fernkampfwaffe/Wurfwaffe")
                .where(page => dv.current().Waffen && dv.current().Waffen.some(link => link.path === page.file.path))
                .sort(page => page.file.name)
                .map(page => {
                    // Determine the attribute modifier based on Finesse property
				    let magicStat = dv.page(dv.current().Hintergrund.Klasse).Zauberattribut ? dv.page(dv.current().Hintergrund.Klasse).Zauberattribut.fileName() : null;
                    let attackStat = dv.current().Attribute.Stärke;
                    if (page?.Eigenschaften?.some(link => link?.path?.includes("Gegenstände/Waffen/Waffeneigenschaften/Finesse.md"))){
	                    attackStat = Math.max(attackStat, dv.current().Attribute.Geschicklichkeit);
                    }
                    if (page?.Eigenschaften?.some(link => link?.path?.includes("Gegenstände/Waffen/Waffeneigenschaften/Magische Präzision.md"))){
	                    attackStat = Math.max(attackStat, dv.current().Attribute[magicStat]);
					}

                    // Calculate attack roll
                    const attackModifier = Math.floor((attackStat - 10) / 2);
                    const proficiencyBonus = Math.ceil(dv.current().Stufe / 4) + 1;
                    const rangedAttackBonus = dv.current().AngriffsbonusFern || 0;
                    const attackRoll = `\`dice:1d20+${attackModifier + proficiencyBonus + rangedAttackBonus}\``;

                    // Calculate damage roll
                    const damageRoll = `\`dice:${page.SchadenFern}+${attackModifier}\``;

                    return [
                        page.file.link,
                        page.Range1,
                        page.Range2,
                        page.Range3,
                        attackRoll,
                        damageRoll,
                        page.SchadensartFern,
                        page.EigenschaftenFern
                    ];
                })
        );
    }

    // Helper function to check if the weapon is a throwable ranged weapon
    function isThrowableWeapon(weaponList) {
        let isThrowable = false;

        for (let item of weaponList) {
            let page = dv.page(item.path);
            let targetTag = "Gegenstand/Waffe/Klasse/Fernkampfwaffe/Wurfwaffe";

            isThrowable = page?.tags && page?.tags?.some(tag => tag === targetTag);

            if (isThrowable) {
                break;
            }
        }

        return isThrowable;
    }

} catch (error) {
    console.error("An error occurred in DataviewJS:", error);
}

```