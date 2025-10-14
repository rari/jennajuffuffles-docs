# FAQ & Known Issues

> 📂 **Docs** / [Start](/start.md) / **FAQ & Known Issues**

*Last updated:* 2025-14-10  
*Applies to Stardew Valley:* **1.6.15+**

> 📖 This guide will be available right on the Nexus Collection page soon!

This page addresses the most common questions and issues players encounter with *Stardew Valley VERY Expanded* (svVe) and its companion collections.

---

## Getting Started FAQs

### Do I need the optional mods?
Yes. While some mods are marked as "optional" to simplify collection stacking, you should install them when using a single collection. These include essential interface improvements, map enhancements, and additional content. 

Expansions are now included as optional mods due to feedback of players feeling overwhelmed and others wanting an even more expanded world. All expansions are curated and selected for a high quality experience. 

### Should I update individual mods myself?
No. Always wait for collection updates rather than updating individual mods. This ensures compatibility and prevents conflicts.

### Can I combine your collections?
Yes. The *Aesthetic Valley* collections are designed to work alongside *Stardew Valley VERY Expanded*. You can use all three together, though this requires more careful mod selection and conflict resolution. See our [Combining Collections](/combining.md) guide for detailed instructions. 

### Can I use this expansion if it's my first time playing Stardew Valley?
Yes, though first-time players should be aware that these collections add substantial content and features that may feel overwhelming. While experiencing vanilla *Stardew Valley* first is recommended, it's not required.

### Do all players need the collection for co-op?
Yes. All players should have matching mods and configurations for the best co-op experience. Mismatched setups can cause sync issues and gameplay problems.

*Multiplayer groups may also elect to use the [Multiplayer Mod Manager](https://www.nexusmods.com/stardewvalley/mods/6609) as well to ensure consist versioning across all player's loadouts.* 

### Where can I download the collections?
Nexus Mods is the only official source. Premium users benefit from one-click downloads. Avoid unauthorized sources to ensure you receive updates and support the mod creators.

**Note:** The Nexus Mods App is currently having minor difficulties handling specific files, such as Solarium Spa from Stardew Valley VERY Expanded. We're seeking a fix for this issue.

---

## Gameplay FAQs

### Why won't the Community Center cutscene trigger?
The Community Center cutscene has specific requirements that are easy to miss. Here's what you need:

- Enter **Pelican Town from the Bus Stop**  
- On or after **Spring 5**, between **8:00 AM–1:00 PM**  
- On a sunny day (not a festival)  
- Host must trigger in multiplayer

*These are the same requirements as vanilla Stardew Valley, but they frequently confuse players.*

### How do I get the Rusty / Sewer Key?
Due to changes in *Stardew Valley Expanded*, **Gunther no longer provides the Rusty Key**.

<details><summary>Click to reveal spoiler details</summary>

Instead, you need to reach 5 hearts with **Marlon**, who will mail the key to you in a cutscene.

**Requirements:**
- **Time:** Any
- **Map:** Adventurer Summit  
- **Season:** Any
- **Weather:** Any
- **Additional:** In year 1, you must have 5 hearts with Marlon. In year 2 or later, there is no friendship requirement, but you must have reached the bottom of the mines at least once

**Description:** Marlon explains that you've proven your worth and introduces you to Krobus, a friendly shadow person who lives in the Pelican Town sewers. Krobus is protected by the Guild and hidden from the town, as humans are generally hostile toward shadow people. After this introduction, Marlon gives you the key to visit Krobus whenever you want.

*Read more about Marlon on the [official Stardew Valley Expanded wiki](https://stardew-valley-expanded.fandom.com/wiki/Marlon).*

</details>

---

## Setup & Customization FAQs

### Can I add more mods?
Yes. These collections serve as excellent foundations for further customization. When adding mods, test them individually and carefully review compatibility notes carefully. Creating a private collection for your additions simplifies future updates.

*Note: While we provide support for the core collections, we may have limited ability to help with mods not included in JennaJuffuffles collections.*

### Can I disable a mod that the collection requires?
Yes. You have full control over your mod setup. Disable the collection in the **Mods view** without affecting recommended mods. This prevents Vortex from managing the collection and allows you to make custom modifications.

*Tip: Add the "Collections" column in Vortex Mods tab (⚙️ >> Collections) to easily find and manage your collection files.*

---

## Known Technical Issues

### Performance & Launching

#### Very Slow Load Time or Crashes

Large collections can take **3–5 minutes** (or longer on lower-specification PCs) to start a new save or load from the title screen.

> **Important:** Avoid using mouse or keyboard input during loading. Wait until the screen fades in and music starts, as input during loading can cause the game to crash.

#### Multiplayer / Split-Screen Desync

Multiplayer sessions may occasionally lag or lose sync. Relaunching the game or restarting the session usually resolves it.

#### SMAPI Not Launching

- Re-add **SMAPI** as the primary tool in Vortex Dashboard.  
- Follow the SMAPI section of the [Install Guide](/install.md) to connect SMAPI to your launch shortcut.

#### Failed to Store Cache Entry (SinZational Speedy Solutions)

You may see red error messages in your SMAPI log like:

```
ERROR  SinZational Speedy Solutions  Failed to store cache entry for [file path].tmx
```

**Example:**
```
00:40:19  ERROR  SinZational Speedy Solutions  Failed to store cache entry for
c:\program files (x86)\steam\steamapps\common\Stardew Valley\Mods\[CP] Ridgeside Village\Assets\Maps\EventMaps\RSVOpenPlot.tmx
```

This message comes from the *SinZational Speedy Solutions* performance optimization mod. It indicates that the mod couldn't cache a specific map file for faster loading.

> **Important:** This is not a crash or gameplay-affecting error. The game and affected mods will still load and function normally.

**Solution:**  
None needed. This error is purely informational and safe to ignore.

*This issue does not indicate missing files, corruption, or mod conflicts. You might see it more often with custom maps or large mods that have unique file structures.*

### Mod Conflicts & File Rules

#### Unresolved File Conflicts (Manage Rules)

The collection includes preset load order rules that should apply automatically. If Vortex shows conflict warnings, the load order was not applied by the collection.

1. In **Vortex >> Mods panel >> Manage Rules (button)**, check that configuration, compatibility, or translation files load ***after*** the mods they impact.  
2. Click **Deploy**.  

> Do not use **Use Suggested** as this may create loops or additional conflicts.

#### Minecart Blocks the Mine Entrance

Access the Generic Mod Config Menu (GMCM) through the game's settings menu or the ⚙️ menu from the main menu.

- Toggle in GMCM: `*Stardew Valley Expanded* >> Original Mine Entrance`.

> This issue may indicate that configurations were not merged properly.

### UI & Crafting Bugs

#### Can't Craft Items Despite Having Ingredients

Better Crafting may be set to not use certain quality levels of ingredients, making it appear you're missing items you actually have.

**Solution:**
- Open the crafting menu and look for quality filters
- Make sure "Show All Qualities" is enabled (Stars button on right side)

*Example: If you can't craft a Bait Maker despite having a Sea Urchin, check that the crafting menu is set to use all quality levels of ingredients.*

#### Missing Recipes in Crafting Menu

Better Crafting organizes recipes into groups, which can hide some recipes from view.

**Solution:**
- Check different categories in the crafting menu
- Look for a "Show All" or "Uncategorized" section

*People usually first notice this when they go to craft their first chest.*

### Visual & UI Conflicts

#### Can't Exit House / Corrupted Farm Map

This occurs when your **farm map mod becomes disabled or fails to load**.  
Maps cannot be switched mid-save unless using a mod like [Easy Farm Switcher](https://www.nexusmods.com/stardewvalley/mods/16873).

**Solution:**  
- Exit the game.  
- Re-enable the farm map mod in Vortex.  
- Click **Deploy**.

---

## NPC & World Bugs

### Duplicated NPCs

This is caused by a bug that causes some NPCs to split. This is a known issue in the game (not specifically related to the collection) with an unknown cause that sometimes happens when talking to NPCs while they are in movement.

**Solution:**  
1. Load your save.  
2. Run in SMAPI console:
```bash
debug removenpc [InternalNPCName]
```
3. Save and exit.

**Common Example:** For Sen specifically, use:
```bash
debug removenpc SenS
```

To find internal names for other NPCs:
```bash
patch export "Data/NPCDispositions"
```

### East Scarp NPCs Not Attending Festivals

Certain NPCs from East Scarp do not attend festivals unless you have 4 hearts with them. This is expected behavior and not a bug.

---


## Vortex Behaviors & Workarounds

Vortex has improved significantly over the years, but certain behaviors still confuse users. Common issues include:

### Updating can overwrite or delete custom configs

Vortex may delete your custom `config.json` (or other settings files) during an update. This is a known behavior that affects personal configurations. Configs bundled with collections aren't affected.

**Solution:** 

1. **Recommended:** Use the newer "Sync Mod Configurations" button built specifically for Stardew configuration management. This will automatically create a custom configuration mod for you and can be disabled at any time in Settings.

2. **Alternative:** See our [Personalization & Custom Configurations](/personalization.md) guide for detailed instructions on protecting your custom settings.

### Mod staging may fail silently 

Vortex stores mods in a compressed library, extracts them to staging, then deploys them to the Mods folder. Occasionally staging fails: the mod shows in the Mods tab, but never loads in-game. No error appears — users only notice missing content.

**Workaround:** After deployment, **check your SMAPI log**, not just the Vortex Mods tab, to confirm the mod is actually loading. ([How to create a SMAPI log](/troubleshooting.md#-how-to-create-a-smapi-log))

* If the mod is missing from the SMAPI log, **redeploy** or **delete the mod and its archive**, then reinstall it from the **Collection tab** in Vortex.

> This bug appears to be rare. If it occurs, please share logs from `AppData/Roaming/Vortex` on Discord so we can pass them to the Vortex team.

### Mods with incorrect folder structure may not deploy properly

Mods with improper folder layouts may not deploy correctly. This mostly affects manually added mods or content packs, not curated collections. The files aren't lost — they're just misplaced.

**Workaround:** Ensure the mods you use follow the proper folder structure from the [official Stardew Valley Wiki guide](https://stardewvalleywiki.com/Modding%3AContent_packs).

### Red errors from "an empty Vortex folder"

Red errors from "an empty Vortex folder" may be caused by old folders left over from disabled mods, or the configuration of mods being installed without the associated mods. This happens most often if recommended mods are not installed and is non-harmful. It is recommend you enable the recommended files or customize your configurations.

### Generic Mod Manager version compatibility

Generic Mod Manager is intentionally not updated to the newest version. The newest version will cause a soft lock if you access the configuration menus of certain mods such as Dynamic Reflections.

---

## Getting Help

### Where can I get support for collection issues?

For questions about the collections, mod compatibility, or gameplay issues:

- **Community Discord**: [Join Here](https://discord.com/invite/de2NrHXuty) – Find us in the *Stardew Valley* channel
- **Collection Documentation**: [Read Here](https://jenna-juffuffles.gitbook.io/svve/)

### Where can I get help with Vortex?

If you run into Vortex-specific issues, start with these resources:

- **Official Vortex Discord**: [Join Here](https://discord.com/invite/nexusmods)
- **Support Hours**: 9 AM – 5 PM GMT, Monday–Thursday
- **Vortex Wiki**: [Read Here](https://wiki.nexusmods.com/index.php/Category:Vortex)
- **Stardew Setup Guide**: [Read Here](https://wiki.nexusmods.com/index.php/Modding_Stardew_Valley_with_Vortex)

*The official Stardew Valley Discord does not support Vortex or JennaJuffuffles' collections. Please use the links above for help and troubleshooting.*

### How do I share my SMAPI log?

*Important: Your computer username may appear in the log. If your username is your full name, please be aware of this before uploading it and consider replacing it if you are concerned.*

**Solution:**
1. Open this page: https://smapi.io/log
2. Follow the instructions at the top of the page to upload the log file. (Don't copy & paste from the console window!)
3. After uploading, it will show a green box with a URL to share. Post that URL here.

*If the issue didn't occur in your last session, load the game until the issue occurs, then upload a new log.*

---

## Quick Links

- [Start Page](/start.md)  
- [Installation Guide](/install.md)  
- [Manual Installation Guide](/manual-install.md)  
- [Updating Collections](/updating.md)  
- [Combining Collections](/combining.md)  
- [Personalization & Custom Configurations](/personalization.md)  
- [Keybinds & Controllers](/keybinds.md)  
- [Troubleshooting](/troubleshooting.md)  
- [FAQ & Known Issues](/faq-and-known-issues.md)
