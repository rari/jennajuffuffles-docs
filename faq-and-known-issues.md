# FAQ & Known Issues

> 📂 **Docs** / [Start](/start.md) / **FAQ & Known Issues**

*Last updated:* 2025-18-09  
*Applies to Stardew Valley:* **1.6.15+**

> 📖 This guide will be available right on the Nexus Collection page soon!

This page addresses the most common questions and issues players encounter with *Stardew Valley VERY Expanded* (svVe) and its companion collections.

---

## Frequently Asked Questions

### Do I need the optional mods?
Yes. While some mods are marked as "optional" to simplify collection stacking, you should install them when using a single collection. These include essential interface improvements, map enhancements, and additional content.

### Should I update individual mods myself?
No. Always wait for collection updates rather than updating individual mods. This ensures compatibility and prevents conflicts.

### Can I combine your collections?
Yes. The *Aesthetic Valley* collections are designed to work alongside *Stardew Valley VERY Expanded*. You can use all three together, though this requires more careful mod selection and conflict resolution. 

### Can I use this expansion if it's my first time playing Stardew Valley?
Yes, though first-time players should be aware that these collections add substantial content and features that may feel overwhelming. While experiencing vanilla *Stardew Valley* first is recommended, it's not required.

### Do all players need the collection for co-op?
Yes. All players should have matching mods and configurations for the best co-op experience. Mismatched setups can cause sync issues and gameplay problems.

### Where can I download the collections?
Nexus Mods is the only official source. Premium users benefit from one-click downloads. Avoid unauthorized sources to ensure you receive updates and support the mod creators.

### Can I add more mods?
Yes. These collections serve as excellent foundations for further customization. When adding mods, test them individually and carefully review compatibility notes. Creating a private collection for your additions simplifies future updates.

*Note: While we provide support for the core collections, we may have limited ability to help with mods not included in JennaJuffuffles collections.*

### Can I disable a mod that the collection requires?
Yes. You have full control over your mod setup. Disable the collection in the **Mods view** without affecting recommended mods. This prevents Vortex from managing the collection and allows you to make custom modifications.

*Tip: Add the "Collections" column in Vortex Mods tab (⚙️ → Collections) to easily find and manage your collection files.*

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

## General Issues

### Very Slow Load Time

Large collections can take **3–5 minutes** (or longer on lower-specification PCs) to start a new save or load from the title screen.

> **Important:** Avoid using mouse or keyboard input during loading. Wait until the screen fades in and music starts, as input during loading can cause the game to crash.

### Multiplayer / Split-Screen Desync

Multiplayer sessions may occasionally lag or lose sync. Relaunching the game or restarting the session usually resolves it.

### SMAPI Not Launching

- Re-add **SMAPI** as the primary tool in Vortex Dashboard.  
- Follow the [Install Guide](/install.md) → PC → SMAPI section.

### Stuck on 74 / 75 Introductions

Enable the **Debug Mode** mod temporarily and run:

```bash
debug wtc lumajunimo
debug wh
```

Disable Debug Mode after fixing.

### Minecart Blocks the Mine Entrance

Access the Generic Mod Config Menu (GMCM) through the game's settings menu or the ⚙️ menu from the main menu.

- Toggle in GMCM: `*Stardew Valley Expanded* → Original Mine Entrance`.

> This issue may indicate that configurations were not merged properly.

---

## Unresolved File Conflicts (Manage Rules)

The collection includes preset load order rules that should apply automatically. If Vortex shows conflict warnings, the load order was not applied by the collection.

1. In **Vortex → Mods panel → Manage Rules (button)**, check that configuration, compatibility, or translation files load ***after*** the mods they impact.  
2. Click **Deploy**.  

> Do not use **Use Suggested** as this may create loops or additional conflicts.

---

## Visual & UI Conflicts

### Can't Exit House / Corrupted Farm Map

This occurs when your **farm map mod becomes disabled or fails to load**.  
Maps cannot be switched mid-save unless using a mod like [Easy Farm Switcher](https://www.nexusmods.com/stardewvalley/mods/16873).

**Solution:**  
- Exit the game.  
- Re-enable the farm map mod in Vortex.  
- Click **Deploy**.

---

## NPC Bugs

### Duplicated NPCs

A rare bug that causes some NPCs to appear twice.

**Solution:**  
1. Load your save.  
2. Run in SMAPI console:
```bash
debug removenpc [InternalNPCName]
```
3. Save and exit.

To find internal names:
```bash
patch export "Data/NPCDispositions"
```
---

## Trouble After Updating

Ensure all mods are enabled in the mod panel in Vortex. 
If problems persist after an update:

1. In **Collections** tab, click **Remove** (the poster).  
2. Do **not** delete mods when asked.  
3. Reinstall from the website into a **New Profile**.  
4. Click **Deploy**.

---

## Known Vortex Behavior & Workarounds

Vortex has improved significantly, but certain behaviors still confuse users. Common issues include:

### Updating can overwrite or delete custom configs

Vortex may delete your custom `config.json` (or other settings files) during an update. This is a known behavior that affects personal configurations. Configs bundled with collections aren't affected.

**Solution:** See our [Personalization & Custom Configurations](/personalization.md) guide for detailed instructions on protecting your custom settings.

### Mod staging may fail silently 

Vortex stores mods in a compressed library, extracts them to staging, then deploys them to the Mods folder. Occasionally staging fails: the mod shows in the Mods tab, but never loads in-game. No error appears — users only notice missing content.

**Workaround:** After deployment, **check your SMAPI log**, not just the Vortex Mods tab, to confirm the mod is actually loading. ([How to create a SMAPI log](/troubleshooting.md#-how-to-create-a-smapi-log))

* If the mod is missing from the SMAPI log, **redeploy** or **delete the mod and its archive**, then reinstall it from the **Collection tab** in Vortex.

> This bug appears to be rare. If it occurs, please share logs from `AppData/Roaming/Vortex` on Discord so we can pass them to the Vortex team.

### Mods with incorrect folder structure may not deploy properly

Mods with improper folder layouts may not deploy correctly. This mostly affects manually added mods or content packs, not curated collections. The files aren't lost — they're just misplaced.

**Workaround:** Ensure the mods you use follow the proper folder structure from the [official Stardew Valley Wiki guide](https://stardewvalleywiki.com/Modding%3AContent_packs).

---

## Need More Help?

Upload your SMAPI log to [smapi.io/log](https://smapi.io/log) and share in our **[Discord](https://discord.gg/de2NrHXuty)** support channel.

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
