# Manual Installation Guide

> 📂 Docs / Installation / Manual / Installation

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* **1.6.15+**

> We recommend **Vortex Mod Manager** for most players because it automatically applies the correct configuration files, manages mod order, and makes updates easy.  
> However, if you prefer to handle installation manually, or are playing on systems without Vortex support, follow this guide.

---

## Check Collection Update Date

Before downloading any mods, check the **last update date** for the collection:  
[svVe Collection Changelog](https://www.nexusmods.com/games/stardewvalley/collections/tckf0m/revisions/87/changelog)  

> **Important:** Do **not** download mods released **after** the collection's last update date — they may not be compatible and could cause instability.

---

## Step 1 — Download the Mods

1. Visit the [Stardew Valley VERY Expanded collection page](https://next.nexusmods.com/stardewvalley/collections/tckf0m).  
2. Open the **Mods** tab.  
3. Download each mod manually from its individual Nexus page (mouse-over the mod, click "Read more").  
4. Place all mod folders into your **Stardew Valley/Mods/** directory.

> On Windows: `%appdata%/StardewValley/Mods`  
> On Mac: `~/.config/StardewValley/Mods`  
> On Linux: `~/.local/share/StardewValley/Mods`

---

## Step 2 — Apply Configuration Files

Download the official configuration package:  
[svVe Configuration Files on Nexus](https://www.nexusmods.com/stardewvalley/mods/20870)  

This page includes configurations for:
- Stardew Valley VERY Expanded  
- Aesthetic Valley | Fairycore  
- Aesthetic Valley | Witchcore  
- Shared configurations used across collections

> **Tip:** Use CTRL+F and search "AVF" or "AVW" if installing an Aesthetic Valley!

**Extract the 7zip files** using [7-Zip](https://www.7-zip.org/) (Windows) or [The Unarchiver](https://theunarchiver.com/) (Mac), then merge the configuration files into the **Mods/** folders they match.  
On Mac, use **Option + drag** to merge folders.

You can modify settings later in-game via **Generic Mod Configuration Menu (GMCM)**.

---

## Step 3 — Apply Required Patches

**For Stardew Valley VERY Expanded and Aesthetic Valley | Witchcore installations:**
- [Grandpa's Tools Patch (Google Drive)](https://drive.google.com/file/d/1F7OcaaxAqz8B8ifIGGSgqWYe9dOMI5wH/view) — Replace the relevant files in the Grandpa's Tools mod folder with the patched versions.

**For Witchcore installations only:**
- [Aurora Vineyard Refurbished Patch](https://drive.google.com/file/d/1ekcuFIlk5gEZry8_Gabh9204065LE22Y/view)  
- [Way Back Pelican Town Fix](https://www.nexusmods.com/stardewvalley/mods/7332?tab=posts) — follow the instructions in the first post.

---

## Step 4 — Aesthetic Valley Compatibility Files

If installing **Fairycore** or **Witchcore**, make sure to also download and install the **appropriate compatibility files** for the UI mod included in that collection.

**For Fairycore installations:**
- **Overgrown Flowery Interface**: Download compatibility files from [Overgrown Flowery Interface optional files](https://www.nexusmods.com/stardewvalley/mods/6166?tab=files) for:
  - Event Lookup
  - Fashion Sense
  - Generic Mod Config Menu
  - Never Ending Adventures & Circle of Thorns (rename folder to match Sword & Sorcery)

**For Witchcore installations:**
- **Earthy Interface**: Download compatibility files from [DaisyNiko's Earthy Interface optional files](https://www.nexusmods.com/stardewvalley/mods/13658?tab=files) for:
  - Generic Mod Config Menu
  - Event Lookup

> **Note:** If installing AVF or AVW, disable in configuration any "Larger Greenhouse" option your chosen farm may have if using the greenhouse included with that collection.

**Manual hair.json fix for Fairycore and Witchcore:**
- Copy the contents of the `hair.json` file in folder `111` into `[FS] Yomi's Golden Princess Hairstyle\Hairs\112`
- Open that file in Notepad++ and change the name at the top from `111` to `112`
- There's a hidden character in the file preventing it from working, so this manual edit is necessary.

---

## Step 5 — Launch with SMAPI

1. Install SMAPI: [Official SMAPI Guide](https://stardewvalleywiki.com/Modding:Installing_SMAPI)  
2. Launch the game using the SMAPI executable.  
3. Check the SMAPI console for errors — if you see missing mods, review the Mods tab on the website to verify all were installed.

---

## Step 6 — Update Notices in SMAPI

Some mods may show an update notification in SMAPI even when no update is actually needed.  
If you wish to suppress the notice, edit the mod's `manifest.json` and set the `"Version"` to match the version shown on Nexus.