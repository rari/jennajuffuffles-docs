# Known Issues & FAQ

> 📂 **Docs** / [Start](/start.md) / **Known Issues & FAQ**

*Last updated:* 2025-08-03  
*Applies to Stardew Valley:* **1.6.15**  
*SVVE Revision:* **86+**

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
- Follow the [Install Guide](/install) → PC → SMAPI section.

### Stuck on 74 / 75 Introductions

Enable the **Debug Mode** mod temporarily and run:

```bash
debug wtc lumajunimo
debug wh
```

Disable Debug Mode after fixing.

---

## ⚙️ Missing Configurations

If the collection’s configuration files do **not** apply, you may see blocked paths, missing overlays, or color mismatches.

1. In **Vortex → Rules Manager**, check that configurations load ***after*** the mods they impact.  
2. Click **Deploy**.  
3. If unresolved, download and apply configs manually from [Nexus](https://www.nexusmods.com/stardewvalley/mods/20870).  

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

## ❓ FAQ Highlights

### Rusty / Sewer Key Change
In SVVE, **Gunther no longer gives the Rusty Key**. Instead, reach 4–5 hearts with **Marlon**, who will mail it to you in a cutscene.

### Community Center Cutscene Won’t Trigger
- Enter **Pelican Town from the Bus Stop**  
- On or after **Spring 5**, between **8:00 AM–1:00 PM**  
- On a sunny day (not a festival)  
- Host must trigger in multiplayer

### Rain Cancels Events & Cutscenes
Certain events (like the Community Center) won’t trigger on rainy days. Try again on a sunny day.

---

## 🧼 After Updating

If problems occur after an update:

1. In **Collections** tab, click **Remove** (the poster).  
2. Do **not** delete mods when asked.  
3. Reinstall from the website into a **New Profile**.  
4. Click **Deploy**.

See the manual installation guide for a full wipe.

---

## 💬 Need More Help?

Upload your SMAPI log to [smapi.io/log](https://smapi.io/log) and share in our **[Discord](https://discord.gg/de2NrHXuty)** support channel.

---

## 📚 Quick Links

- 🌾 [Start Page](/start)  
- 🚀 [Installation Guide](/install)  
- 🧩 [Manual Installation Guide](/manual-install)  
- 🔀 [Combining Collections](/combining)  
- 🎮 [Keybinds & Controllers](/keybinds)  
- 🛠️ [Troubleshooting](/troubleshooting)  
- ❓ [Known Issues & FAQ](/known-issues-and-faq)  

