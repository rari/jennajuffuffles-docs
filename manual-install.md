# Manual Installation Guide

> 📂 **Docs** / [Start](/start.md) / **Manual Install**

*Last updated:* 2025-08-09  
*Applies to Stardew Valley:* **1.6.15+**  
> We recommend **Vortex Mod Manager** for most players because it automatically applies the correct configuration files, manages mod order, and makes updates easy.  
> However, if you prefer to handle installation manually, or are playing on systems without Vortex support, follow this guide.

---

## 📅 Check Collection Update Date

Before downloading any mods, check the **last update date** for the collection:  
[SVVE Collection Changelog](https://www.nexusmods.com/games/stardewvalley/collections/tckf0m/revisions/87/changelog)  

> ⚠️ Do **not** download mods released **after** the collection’s last update date — they may not be compatible and could cause instability.

---

## 📥 Step 1 — Download the Mods

1. Visit the [Stardew Valley VERY Expanded collection page](https://next.nexusmods.com/stardewvalley/collections/tckf0m).  
2. Open the **Mods** tab.  
3. Download each mod manually from its individual Nexus page.  
4. Place all mod folders into your **Stardew Valley/Mods/** directory.

> On Windows: `%appdata%/StardewValley/Mods`  
> On Mac: `~/.config/StardewValley/Mods`  
> On Linux: `~/.local/share/StardewValley/Mods`

---

## ⚙️ Step 2 — Apply Configuration Files

Download the official configuration package:  
[SVVE Configuration Files on Nexus](https://www.nexusmods.com/stardewvalley/mods/20870)  

This page includes configurations for:
- Stardew Valley VERY Expanded  
- Aesthetic Valley | Fairycore  
- Aesthetic Valley | Witchcore  
- Shared configurations used across collections

Unzip and merge the configuration files into the **Mods/** folders they match.  
On Mac, use **Option + drag** to merge folders.

You can modify settings later in-game via **Generic Mod Configuration Menu (GMCM)**.

---

## 🎨 Step 3 — Aesthetic Valley Compatibility Files

If installing **Fairycore** or **Witchcore**, make sure to also download and install the **appropriate compatibility files** for the UI mod included in that collection.

**Witchcore users also need to apply:**
- [Aurora Vineyard Refurbished Patch](https://drive.google.com/file/d/1ekcuFIlk5gEZry8_Gabh9204065LE22Y/view)  
- [Way Back Pelican Town Fix](https://www.nexusmods.com/stardewvalley/mods/7332?tab=posts) — follow the instructions in the first post.

---

## 🩹 Step 4 — Apply Grandpa's Tools Patch

If you are using **Grandpa’s Tools**, apply this patch:  
[Grandpa’s Tools Patch (Google Drive)](https://drive.google.com/file/d/1F7OcaaxAqz8B8ifIGGSgqWYe9dOMI5wH/view)  

Replace the relevant files in the Grandpa’s Tools mod folder with the patched versions.

---

## 🧪 Step 5 — Launch with SMAPI

1. Install SMAPI: [Official SMAPI Guide](https://stardewvalleywiki.com/Modding:Installing_SMAPI)  
2. Launch the game using the SMAPI executable.  
3. Check the SMAPI console for errors — if you see missing mods, return to Step 1 and verify all were installed.

---

## 🛠️ Step 6 — Update Notices in SMAPI

Some mods may show an update notification in SMAPI even when no update is actually needed.  
If you wish to suppress the notice, edit the mod’s `manifest.json` and set the `"Version"` to match the version shown on Nexus.

---

## 📚 Quick Links

- 🌾 [Start Page](/start.md)  
- 🚀 [Installation Guide](/install.md)  
- 🧩 [Manual Installation Guide](/manual-install.md)  
- 🔀 [Combining Collections](/combining.md)  
- 🎮 [Keybinds & Controllers](/keybinds.md)  
- 🛠️ [Troubleshooting](/troubleshooting.md)  
- ❓ [Known Issues & FAQ](/known-issues-and-faq.md)  

