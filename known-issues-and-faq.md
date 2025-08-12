# Known Issues & FAQ

> 📂 **Docs** / [Start](/start.md) / **Known Issues & FAQ**

*Last updated:* 2025-08-09  
*Applies to Stardew Valley:* **1.6.15+**

This page covers **common issues**, **frequently asked questions**, and **gameplay notes** for Stardew Valley VERY Expanded (SVVE) and its companion collections.

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

---

## ⚙️ Missing Configurations

The collection includes preset load order rules that should apply automatically. If Vortex shows conflict warnings, it means the configuration files didn't load properly.

1. In **Vortex → Rules Manager**, check that configurations load ***after*** the mods they impact.  
2. Click **Deploy**.  
3. If unresolved, download and apply configs manually from [Nexus](https://www.nexusmods.com/stardewvalley/mods/20870).  

**Manage Conflicts:** If Vortex shows a conflict warning, make sure the configuration, compatibility, or translation file is set to load after the actual mod.

#### Minecart Blocks the Mine Entrance

- Toggle in GMCM: `Stardew Valley Expanded → Original Mine Entrance`.

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

## ❓ Frequently Asked Questions (FAQ)

### Should I update individual mods myself?
Please wait for collection updates. Updating individual mods is not recommended.

### Can I combine your collections?
Absolutely! My Aesthetic Valley collections were designed to add a fun theme on top of Stardew Valley VERY Expanded. You can even use all three together, though you'll have to make more choices when resolving which mods to use from each. If you add mods that are not in a collection created by JennaJuffuffles, this community may not be able to offer much support.

### Can I use this expansion if it's my first time playing Stardew Valley?
Yes, you can use the expansion, even if it's your first time playing Stardew Valley. However, be aware that the collections add a lot of content and features to the game, so it may be overwhelming for first-time players. Experiencing vanilla Stardew Valley is recommended but absolutely not required.

### Do all players need the collection for co-op?
It is recommended that all players have matching mods and configurations for co-op. This may not be strictly necessary, but should lead to the best results.

### Where to download? Is there a faster way?
Nexus is the only official source. Premium users get one-click download. Avoid unauthorized sources to ensure updates and support mod creators.

### Why won't the Community Center cutscene trigger?
- Enter **Pelican Town from the Bus Stop**  
- On or after **Spring 5**, between **8:00 AM–1:00 PM**  
- On a sunny day (not a festival)  
- Host must trigger in multiplayer

### How do I get the Rusty / Sewer Key?
In SVVE, **Gunther no longer gives the Rusty Key**. Instead, reach 4–5 hearts with **Marlon**, who will mail it to you in a cutscene.

---

## 💬 Need More Help?

Upload your SMAPI log to [smapi.io/log](https://smapi.io/log) and share in our **[Discord](https://discord.gg/de2NrHXuty)** support channel.

---

## 📚 Quick Links

- 🌾 [Start Page](/start.md)  
- 🚀 [Installation Guide](/install.md)  
- 🧩 [Manual Installation Guide](/manual-install.md)  
- 🔀 [Combining Collections](/combining.md)  
- 🎮 [Keybinds & Controllers](/keybinds.md)  
- 🛠️ [Troubleshooting](/troubleshooting.md)  
- ❓ [Known Issues & FAQ](/known-issues-and-faq.md)

