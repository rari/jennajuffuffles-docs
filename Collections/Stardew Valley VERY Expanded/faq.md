# FAQ & Troubleshooting — Stardew Valley VERY Expanded

> 📂 Docs / Collections / SVVE / FAQ

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* **1.6.15+**

---

**Community Center cutscene won't trigger**
> The Community Center cutscene has specific requirements that must be met:
> - Enter Pelican Town from the Bus Stop (not from another direction)
> - Must be Spring 5 or later in Year 1
> - Time must be between 8:00 AM and 1:00 PM
> - Day must be sunny (no rain or storms)
> - Cannot be a festival day
> - In multiplayer, only the host can trigger this cutscene
> 
> The mods in the collection do not change this event. These are vanilla requirements.
> If all conditions are met and it still won't trigger, check your SMAPI log for any errors that might be blocking the event.

**Rusty/Sewer Key changes in SVE**
> Due to Stardew Valley Expanded changes, the way you obtain the Rusty Key (Sewer Key) has changed from vanilla. Gunther no longer provides the Rusty Key at the museum.

<details>
<summary>How to obtain the Rusty Key in SVE (Spoiler)</summary>

> Instead, you need to reach 5 hearts with Marlon. Once you achieve this friendship level, he will mail you the key in a cutscene. Make sure to talk to Marlon regularly and give him gifts he likes to build friendship. See the SVE wiki for more details about friendship requirements and gift preferences.

</details>

**Minecart blocks the mine entrance**
> If you find a minecart blocking the entrance to the mines, you can fix this in the Generic Mod Config Menu (GMCM):
> 1. Open the game settings menu (⚙️) or press the GMCM hotkey
> 2. Navigate to **SVE** settings
> 3. Look for the option **"Original Mine Entrance"** and enable it
> 
> If this entry was missing from the GMCM menu, it indicates that your SVE configurations may not have merged properly during installation. Try removing and reinstalling the collection, or check your SMAPI log for configuration errors.

**Can't craft items despite having ingredients**
> Better Crafting has quality filters that may prevent you from crafting items if your ingredients don't meet the quality threshold. This is a common issue that catches many players off guard.
> 
> To fix this:
> 1. Open the crafting menu
> 2. Look for the **Stars button** on the right side of the interface
> 3. Click it to enable **"Show All Qualities"**
> 
> This will allow you to craft items regardless of ingredient quality. A common example is the Bait Maker, which can be blocked by quality filters if your ingredients don't match the selected quality level.

**Missing recipes in crafting menu (such as Chest)**
> Better Crafting organizes recipes into categories to make the crafting menu more manageable. If you can't find a recipe you know you should have (like the basic Chest):
> 1. Check other categories in the crafting menu - recipes are grouped by type
> 2. Look for **"Show All"** or **"Uncategorized"** options
> 3. Use the search function if available to find specific recipes
> 
> The basic Chest recipe should be in the "Building" or similar category. If you still can't find it, check that you have the required crafting level and that the recipe hasn't been disabled in mod settings.

**Duplicated NPCs**
> This is a rare base-game issue where an NPC can appear duplicated or "split" in your game world. If you encounter a duplicate NPC, you can remove them using SMAPI console commands:
> 
> 1. Load your save file in the game
> 2. Open the SMAPI console (the command window that appears when you launch the game)
> 3. In the console, type: `debug removenpc [InternalNPCName]`
>    - Replace `[InternalNPCName]` with the NPC's internal name
>    - Example: `debug removenpc SenS` (for Sen from Lurking in the Dark)
> 4. Save your game and exit
> 
> To find the internal name of an NPC:
> - In the SMAPI console, run: `patch export "Data/NPCDispositions"`
> - This will create a file that lists all NPCs and their internal names
> - Look for the duplicated NPC in the list

**East Scarp NPCs not attending festivals**
> This is expected behavior and not a bug. Some East Scarp expansion NPCs in particualr require you to have at least 4 hearts of friendship with them before they will attend festivals. 
> 
> To get them to appear at festivals:
> - Talk to them regularly (daily if possible)
> - Give them gifts they like (check their wiki pages for preferences)
> - Complete any quests they offer
> - Once you reach 4 hearts, they should start appearing at festivals

**Very slow load or crash on first load**
> Large collections like SVVE can take 3–5 minutes (or sometimes longer) to start a new save or load an existing one. This is normal due to the number of mods and content being loaded and dependant on available memory.
> 
> **Important:** During the loading process, avoid clicking, pressing keys, or alt-tabbing away from the game. Interacting with the game during loading can cause crashes or freezes. Just let it load - you'll see progress in the SMAPI console window. The game will be ready when the console stops showing loading messages.
> 
> If the game consistently crashes during loading (not just slow loading), check your SMAPI log for errors and see our troubleshooting guide.
>
> Disabling Dynamic Reflections may be a solution for users with limited memory.
