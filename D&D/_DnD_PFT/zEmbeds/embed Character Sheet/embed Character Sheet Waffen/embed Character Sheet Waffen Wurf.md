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
                    const finesse = page?.Eigenschaften && page?.Eigenschaften?.some(e => e === "Finesse");
                    const attributeMod = finesse
                        ? Math.floor((dv.current().Attribute.Geschicklichkeit - 10) / 2)
                        : Math.floor((dv.current().Attribute.Stärke - 10) / 2);

                    // Calculate attack roll
                    const levelBonus = Math.ceil(dv.current().Stufe / 4) + 1;
                    const rangedAttackBonus = dv.current().AngriffsbonusFern || 0;
                    const attackRoll = `\`dice:1d20+${attributeMod + levelBonus + rangedAttackBonus}|none|noform\``;

                    // Calculate damage roll
                    const damageRoll = `\`dice:${page.SchadenFern}+${attributeMod}|none|noform\``;

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