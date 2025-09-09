# FAQ & Known Issues

> 📂 **Docs** / [Start](/start.md) / **FAQ & Known Issues**

*Last updated:* 2025-09-09  
*Applies to Stardew Valley:* **1.6.15+**

> 📖 This guide will be available right on the Nexus Collection page soon!

This page covers **frequently asked questions**, **common issues**, and **gameplay notes** for *Stardew Valley VERY Expanded* (svVe) and its companion collections.

---

## ❓ Frequently Asked Questions (FAQ)

### Do I need the optional mods?
**Yes!** Some mods are marked as "optional" to make 'collection stacking' simple, but if you are only using one collection you should absolutely install the optional mods. This will include the interface, the map, and more!

### Should I update individual mods myself?
Please wait for collection updates. Updating individual mods is not recommended.

### Can I combine your collections?
Absolutely! My *Aesthetic Valley* collections were designed to add a fun theme on top of *Stardew Valley VERY Expanded*. You can even use all three together, though you'll have to make more choices when resolving which mods to use from each. 

### Can I use this expansion if it's my first time playing Stardew Valley?
Yes, you can use the expansion, even if it's your first time playing *Stardew Valley*. However, be aware that the collections add a lot of content and features to the game, so it may be overwhelming for first-time players. Experiencing vanilla *Stardew Valley* is recommended but absolutely not required.

### Do all players need the collection for co-op?
It is recommended that all players have matching mods and configurations for co-op. This may not be strictly necessary, but should lead to the best results.

### Where to download? Is there a faster way?
Nexus is the only official source. Premium users get one-click download. Avoid unauthorized sources to ensure updates and support mod creators.

### Can I add more mods?
Absolutely! These collections make excellent jumping-off points for your modding journey! Feel free to experiment and add your favorite mods - just remember to test as you go and thoroughly read mod pages for compatibility notes. 

It's recommended to create a private collection for your additions to make updates even easier! 

*Note: If you add mods that aren't in a collection created by JennaJuffuffles, this community may not be able to offer as much support, but we'll always try our best to help!*

### Can I disable a mod that the collection requires?
No worries! You have full control over your mod setup. You can disable the collection in the **Mods view** without disabling any recommended mods. This will stop Vortex from trying to manage the collection and allow you to make any modifications you wish!

*💡 Tip: Add the "Collections" column in Vortex Mods tab (⚙️ → Collections) to easily find and manage your collection files.*

### Why won't the Community Center cutscene trigger?
The Community Center cutscene has very specific requirements that are easy to miss! Here's what you need:

- Enter **Pelican Town from the Bus Stop**  
- On or after **Spring 5**, between **8:00 AM–1:00 PM**  
- On a sunny day (not a festival)  
- Host must trigger in multiplayer

*This isn't a change from the vanilla game, but these specific requirements trip up a lot of players!*

### How do I get the Rusty / Sewer Key?
Thanks to changes made by the mod *Stardew Valley Expanded*, **Gunther no longer gives the Rusty Key**.

<details><summary>💡 Click to reveal spoiler details</summary>

Instead, reach 5 hearts with **Marlon**, who will mail it to you in a cutscene.

**Details:**
- **Time:** Any
- **Map:** Adventurer Summit  
- **Season:** Any
- **Weather:** Any
- **Extra:** In year 1, player must have 5 hearts with Marlon. In year 2 or later, there is no friendship requirement, but the player must have reached the bottom of the mines at least once

**Description:** Marlon tells you that you've proven your worth and it's time to meet Krobus! Krobus is a friendly shadow person who lives in the Pelican Town sewers, protected by the Guild and hidden from the town. While Krobus can speak human language, they have to stay hidden since humans are generally hostile toward shadow people. After this heartwarming introduction, Marlon gives you the key to the sewers so you can visit your new friend Krobus whenever you want!

*Read more about Marlon on the [official Stardew Valley Expanded wiki](https://stardew-valley-expanded.fandom.com/wiki/Marlon).*

</details>

---

## 🔁 General Issues

### Very Slow Load Time

Large collections can take **3–5 minutes** (or longer on low-spec PCs) to start a new save or load from the title screen.

> 🖐️ **Hands-up method:** Keep your hands off the mouse/keyboard until the screen fades in and music starts. Input during loading can crash the game.

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

If you go to the bottom of settings in game (or the ⚙️ menu from the main menu) you can open the config menu, Generic Mod Config Menu (GMCM).

- Toggle in GMCM: `*Stardew Valley Expanded* → Original Mine Entrance`.

> This may be a sign that configurations were not merged properly.

---

## ⚙️ Unresolved File Conflicts (Manage Rules)

The collection includes preset load order rules that should apply automatically. If Vortex shows conflict warnings, it means the load order was not applied by the collection for some reason.

1. In **Vortex → Mods panel → Manage Rules (button)**, check that configuration, compatibility, or translation files load ***after*** the mods they impact.  
2. Click **Deploy**.  

> Do not use **Use Suggested** as this may create loops or additional conflicts.

---

## 🛠️ Visual & UI Conflicts

### Can't Exit House / Corrupted Farm Map

Occurs when your **farm map mod becomes disabled or fails to load**.  
Maps cannot be switched mid-save unless using a mod like [Easy Farm Switcher](https://www.nexusmods.com/stardewvalley/mods/16873).

**Fix:**  
- Exit game.  
- Re-enable farm map mod in Vortex.  
- Click **Deploy**.

---

## 🧪 NPC Bugs

### Duplicated NPCs

A rare bug causing some NPCs to appear twice.

**Fix:**  
1. Load save.  
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

## 🧼 Trouble After Updating

Ensure all mods are Enabled in the mod panel in Vortex. 
If problems still occur after an update:

1. In **Collections** tab, click **Remove** (the poster).  
2. Do **not** delete mods when asked.  
3. Reinstall from the website into a **New Profile**.  
4. Click **Deploy**.

---

## Known Vortex Behavior & Workarounds

Vortex has improved a lot, but certain quirks still confuse users. When people say “Vortex eats files,” they’re usually running into one of these issues:

### Updating can overwrite or delete custom configs

Vortex may delete your custom `config.json` (or other settings files) during an update. This is a known behavior and seems to be a main source of the "Vortex eats files" myth. Configs bundled with collections aren’t affected.

**Workaround:** Use the [**Add Custom Mod Button**](https://www.nexusmods.com/site/mods/863) Vortex extension to create a persistent "My Configs" mod that always loads after your main mods:

1. Configure mods as desired in-game (GMCM recommended).
2. In Vortex, click **Create new mod** via the Add Custom Mod Button.
3. Copy the target mod folders into "My Configs" and delete everything inside except your config files.
4. In **Manage Rules**, set "My Configs" to load **after** those mods.

This ensures your personal settings are reapplied automatically. even after updates.

### Mod staging may fail silently 

Vortex stores mods in a compressed library, extracts them to staging, then deploys them to the Mods folder. Occasionally staging fails: the mod shows in the Mods tab, but never loads in-game. No error appears — users only notice missing content.

**Workaround:** After deployment, **check your SMAPI log**, not just the Vortex Mods tab, to confirm the mod is actually loading. ([How to create a SMAPI log](/troubleshooting.md#-how-to-create-a-smapi-log))

* If the mod is missing missing from the SMAPI log, **redeploy** or **delete the mod and its archive**, then reinstall it from the **Collection tab** in Vortex.

> 📌 This bug seems rare. If it happens, please share logs from `AppData/Roaming/Vortex` on Discord so we can pass them to the Vortex team.

### Mods with incorrect folder structure may not deploy properly

Mods with bad folder layouts may not deploy correctly. This mostly affects manually added mods or content packs, not curated collections. The files aren’t lost — they’re just misplaced.

**Workaround:** Ensure the mods you use follow the proper folder structure from the [official Stardew Valley Wiki guide](https://stardewvalleywiki.com/Modding%3AContent_packs).

---

## 💬 Need More Help?

Upload your SMAPI log to [smapi.io/log](https://smapi.io/log) and share in our **[Discord](https://discord.gg/de2NrHXuty)** support channel.

---

## 📚 Quick Links

- 🌾 [Start Page](/start.md)  
- 🚀 [Installation Guide](/install.md)  
- 🧩 [Manual Installation Guide](/manual-install.md)  
- 🔄 [Updating Collections](/updating.md)  
- 🔀 [Combining Collections](/combining.md)  
- 🎮 [Keybinds & Controllers](/keybinds.md)  
- 🛠️ [Troubleshooting](/troubleshooting.md)  
- ❓ [FAQ & Known Issues](/faq-and-known-issues.md)
