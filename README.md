# PF2e Flatfinder
A compendium of replacements for Feats, Actions and Activities to streamline running Flatfinder on Foundry. To be used with the Pathfinder 2e system and the Proficiency without Level variant enabled.
NOTE: this is module in very early development.

## What is included (and what isn't)
- Most Actions, Activities and Feats modified by Flatfinder have a modified version included in the module, marked with (FF).
- The description of the Treat Wounds activity has a table which can post the heal results to chat for you, but you must manually roll the Medicine check. **For it to work, it must be added to the character sheet of whoever is attempting the check**.
  - Medic Dedication correctly modifies the heal amounts of the Treat Wounds.
  - Two alternate Treat Wounds activities for Risky Surgery and Natural Medicine.
- The Follow the Expert effect and the Untrained Improvisation feat automation has been modified to work with Flatfinder.
- Effects to apply the modified Weak and Elite templates without changing level to avoid issues with "reflattening"

## How to use
- Install the module and activate it in your Pathfinder 2e World. 
- Enable the Proficiency without Level variant in the Game Settings.
  - Make sure the Untrained Proficiency Penalty is -2.
- Use the content in the Flatfinder compendium. 
  - The modified versions of the game elements changed by Flatfinder are marked (FF).
- **PF2e Flatten Proficiency Level Bonus for PCs and NPCs** is recommended to adjust NPC proficiency bonuses.
  
### Competence checks
As of release 0.2.0, Competence checks must be adjudicated manually by the GM. Properly automating Competence checks is not possible through simple Rules Elements, and coding them in TypeScript goes beyond my abilities. Maybe some day.
  
### Healing Feats
Remember to add the **Treat Wounds (FF)** activity to all characters who will ever Treat Wounds, use Battle Medicine or the like. That gives them a Base Healing attribute, which is required for the following to work.
- Roll the Medicine check in the **Treat Wounds (FF)** activity description.
- Click the field in the row of the table corresponding to the result of your Competence check.
- Apply the healing that just popped up in the chat.
**Medic Dedication (FF)** correctly modifies the Base Healing values in the **Treat Wounds (FF)** activity. **Mortal Healing (FF)** gives a toggle in the Action tab to add the +4 circumstance bonus.
To use **Risky Surgery (FF)** or **Natural Medicine (FF)**, add the **Risky Treat Wounds (FF)** and **Natural Treat Wounds (FF)** respectively and use those instead of the regular activity.
**Encouraging Words (FF)** works similarly, but the feat automatically gives you the corresponding action with working automatic calculations.

### Follow the Expert
Use **Effect: Follow the Expert (FF)** in lieu of the regular effect. You can drag it from the description for **Follow the Expert (FF)** or directly from the Flatfinder compendium.

### Weak and Elite templates
If you want to apply the Weak and Elite templates as described in Flatfinder, you should use the effects in the **FF Adjustments** folder instead of using the default Weak and Elite templates. These effects modify all stats properly, but they do not change level to avoid **pf2e-flatten** "reflattening" the creatures and undoing the changes. Use the **<2** version for creatures of level 1 or below.

### Other
The rest of the feats, actions and activities changed by Flatfinder, except the exceptions noted below, are included in the Flatfinder compendium and should appear in the Compendium Browser. Use the Flatfinder-modified items, marked by **(FF)**.

## Known gaps and issues
- The changes for Incapacitation and Ritual DCs are not implemented.
- Several feats are not automated properly.
- Unified Equipment Quality is not implemented.
- Earn Income and Craft are not implemented.
- Spells such as Animal Form don't have flattened modifiers.
- Items don't have flattened modifiers and DCs.
