```dataviewjs
try {
    // Check if the "Waffen" metadata includes "Fernkampf" weapons (long-range)
    if (dv.current().Waffen && isRangedWeapon(dv.current().Waffen)) {

        dv.header(3, "Schusswaffen");

        dv.table(
            ["Waffe", "Min RW", "Gnd RW", "Max RW", "Angriff", "Schaden", "Schadensart", "Eigenschaften"],
            dv.pages("#Gegenstand/Waffe/Klasse/Fernkampfwaffe/Schusswaffe")
                .where(p => dv.current().Waffen && dv.current().Waffen.some(link => link.path === p.file.path) && p.tags.includes("Gegenstand/Waffe/Klasse/Fernkampfwaffe/Schusswaffe"))
                .sort(page => page.file.name)
                .map(page => {
                    // Calculate attack roll
                    const attackModifier = Math.floor((dv.current().Attribute.Geschicklichkeit - 10) / 2);
                    const levelBonus = Math.ceil(dv.current().Stufe / 4) + 1;
                    const rangedAttackBonus = dv.current().AngriffsbonusFern || 0;
                    const attackRoll = `\`dice:1d20+${attackModifier + levelBonus + rangedAttackBonus}|none|noform\``;

                    // Calculate damage roll
                    const damageModifier = Math.floor((dv.current().Attribute.Geschicklichkeit - 10) / 2);
                    const damageRoll = `\`dice:${page.SchadenFern}+${damageModifier}|none|noform\``;

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

    // Helper function to check if the weapon is a ranged weapon
    function hasTag(page, targetTag) {
        return page?.tags && page?.tags?.some(tag => tag === targetTag);
    }

    function isRangedWeapon(weaponList) {
        let isRangedWeapon = false;

        for (let item of dv.current().Waffen) {
            let page = dv.page(item.path);
            let targetTag = "Gegenstand/Waffe/Klasse/Fernkampfwaffe/Schusswaffe";

            // Call the function and store the result
            isRangedWeapon = hasTag(page, targetTag);

            if (isRangedWeapon) {
                break;
            }
        }

        return isRangedWeapon;
    }

} catch (error) {
    console.error("An error occurred in DataviewJS:", error);
}
```