---
title: Installing Collections on Steam Deck
description: Install Stardew Valley mod collections on Steam Deck. Transfer from a Windows PC, choose Linux or Proton, install matching SMAPI, and launch from Steam.
keywords: [Steam Deck, Steam Deck installation, Linux modding, Steam Deck mods, transferring to Steam Deck, Proton, Steam Deck SMAPI, Linux mods]
tags: [installation, steam-deck, linux, proton]
---

# Sideload to Steam Deck

*Last updated:* 2026-06-10  
*Applies to Stardew Valley:* 1.6.15+

Vortex is Windows-only, so install the collection on a PC first, then transfer your **Mods** folder to Steam Deck. **SMAPI must be installed separately on Steam Deck** using the instructions that match how you run the game. Do not copy SMAPI from your PC.

---

## Quick answers

{% hint style="info" %}
**Do I run `StardewModdingAPI.exe` directly?** No. After SMAPI is installed, launch **Stardew Valley from Steam** as usual. SMAPI attaches automatically and opens its console when working.

**Linux or Proton?** For Stardew on Steam Deck, **native Linux** is the usual choice. If you use Proton instead, install SMAPI for that path. **Your SMAPI install must match your runtime.** Linux SMAPI with a Proton game (or the reverse) will not work.

**Can I copy SMAPI from my PC?** No. Copy **mods and configs** only. Install SMAPI on Steam Deck per the [SMAPI Steam Deck guide](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Steam_Deck).

**Co-op with a PC or Mac?** Mod **content** is cross-platform, but each player needs SMAPI installed locally and the same mod versions and configs. See [Multiplayer Support](../About/index.md#multiplayer-support) on the About page.
{% endhint %}

---

## Prerequisites

- A Windows PC with Vortex installed
- A USB drive, cloud storage, or network connection to transfer files
- Stardew Valley installed on both PC and Steam Deck

{% hint style="danger" %}
Copy from your PC's game **Mods** folder only **after** Vortex has deployed mods successfully. Use **hardlink** deployment in Vortex, not symbolic links. Symbolic links often break when copied to a USB drive or cloud folder, leaving empty or missing mod folders on Steam Deck.
{% endhint %}

---

## Table of Contents

- [On PC: Install the Collection](#on-pc-install-the-collection)
- [On PC: Prepare for Transfer](#on-pc-prepare-for-transfer)
- [On Steam Deck: Install Stardew Valley](#on-steam-deck-install-stardew-valley)
- [On Steam Deck: Choose Your Runtime](#on-steam-deck-choose-your-runtime)
- [On Steam Deck: Install SMAPI](#on-steam-deck-install-smapi)
- [On Steam Deck: Transfer Mods](#on-steam-deck-transfer-mods)
- [On Steam Deck: Launch and Verify](#on-steam-deck-launch-and-verify)
- [Troubleshooting](#troubleshooting)
- [See Also](#see-also)

---

## On PC: Install the Collection

1. Follow the [New Player Install Instructions](index.md) to install the collection using Vortex on your PC
2. Launch the game once on PC and confirm mods load in the SMAPI console
3. Check your [SMAPI log](../Troubleshooting/your-smapi-log.md) for red errors before transferring

---

## On PC: Prepare for Transfer

1. In Steam on PC: right-click **Stardew Valley** > **Manage** > **Browse local files**
2. Copy the entire **Mods** folder to a USB drive, cloud folder, or network share
3. Include any config changes you made (usually inside **Mods** or mod subfolders)

---

## On Steam Deck: Install Stardew Valley

1. Switch to **Desktop Mode**
2. Install Stardew Valley through Steam
3. Launch the game once to finish first-time setup, then quit

---

## On Steam Deck: Choose Your Runtime

Pick **one** path before installing SMAPI. You can change later, but you must **reinstall SMAPI** if you switch.

### Native Linux (recommended on Steam Deck)

1. In Steam (Desktop or Game Mode): **Stardew Valley** > **Properties** > **Compatibility**
2. **Disable** "Force the use of a specific Steam Play compatibility tool" (no Proton)
3. The game runs as the **Linux** build

**Mods folder on Steam Deck:** `~/.local/share/StardewValley/Mods`

### Proton (Windows build on Steam Deck)

1. In Steam: **Stardew Valley** > **Properties** > **Compatibility**
2. **Enable** a Proton version (e.g. Proton Experimental)
3. The game runs as the **Windows** build under Proton

**Mods folder on Steam Deck:** inside the game install folder (e.g. `.../steamapps/common/Stardew Valley/Mods`), next to `Stardew Valley.exe`

{% hint style="warning" %}
If mods worked on PC but not on Steam Deck, check for a **runtime mismatch**: Linux SMAPI installed while the game still uses Proton, or the opposite. Match runtime and SMAPI, then reinstall SMAPI if needed.
{% endhint %}

---

## On Steam Deck: Install SMAPI

1. Open the [SMAPI Installation Guide for Steam Deck](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Steam_Deck)
2. Follow the section that matches your runtime:
   - **Native Linux:** use the **Linux** instructions on that page
   - **Proton:** use the **Windows / Proton** instructions on that page
3. Let the installer configure Steam to launch through SMAPI
4. Do **not** copy `StardewModdingAPI.exe` or other SMAPI files from your Windows PC

---

## On Steam Deck: Transfer Mods

1. Connect your USB drive or download from cloud storage
2. Copy the **Mods** folder from your PC into the correct location for your runtime:

| Runtime | Where to put `Mods` |
|---------|---------------------|
| **Native Linux** | `~/.local/share/StardewValley/Mods` (create the folder if needed) |
| **Proton** | `.../steamapps/common/Stardew Valley/Mods` (browse local files from Steam to open this folder) |

3. Merge or replace so each mod is a subfolder inside **Mods**, same layout as on PC
4. If you use collection config packs from Nexus, ensure those files are included in the transferred folders

---

## On Steam Deck: Launch and Verify

1. Launch **Stardew Valley from your Steam library** (Game Mode or Desktop). Do **not** double-click `StardewModdingAPI.exe` in the game folder.
2. Confirm the SMAPI console appears and lists your mods
3. If anything fails, upload your log from [your SMAPI log](../Troubleshooting/your-smapi-log.md) page steps (on Linux: `~/.config/StardewValley/ErrorLogs`)

---

## Troubleshooting

### Nothing happens when I open `StardewModdingAPI.exe`

You should not launch SMAPI manually. Start the game from **Steam**. If SMAPI is installed correctly, it runs when Stardew starts.

### Mods missing or SMAPI shows an empty mod list

- Confirm **Mods** is in the folder for your runtime (see table above). Native Linux uses `~/.local/share/StardewValley/Mods`, not only the Steam game directory.
- Confirm **runtime and SMAPI match** (Linux + Linux SMAPI, or Proton + Proton/Windows SMAPI).
- Reinstall SMAPI after changing Proton settings.
- Verify every mod folder copied completely from PC (no broken symbolic links).

### Game won't start

- Re-run the [SMAPI Steam Deck guide](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Steam_Deck) for your runtime
- Verify game files in Steam: **Properties** > **Installed Files** > **Verify**
- Check the SMAPI log for red errors

### Linux-specific log errors

If your SMAPI log shows **`Failed parsing new quests.`**, install [Ridgeside Village Quest Fix For Linux and Mac](https://www.nexusmods.com/stardewvalley/mods/36004). See [Ridgeside Village](../Troubleshooting/mod-issues.md#ridgeside-village) in Mod-Specific Known Issues for more context.

### Performance issues

- Large collections can be heavy on Steam Deck; lower in-game settings if needed
- Disable optional performance-heavy mods if you added any on PC
- Check Steam Deck power settings in Game Mode

---

## See Also

- [New Player Install Instructions](index.md) - Install the collection on PC first
- [Manual Installation](manual.md) - Mod folder paths for Windows, Mac, and Linux
- [Using a Controller](controller.md) - Controller and GMCM keybinds
- [Troubleshooting & FAQ](../Troubleshooting/index.md) - Quick fixes and deeper guides
- [Your SMAPI Log](../Troubleshooting/your-smapi-log.md) - Find and read error logs
- [SMAPI Steam Deck Guide](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Steam_Deck) - Official SMAPI install steps
