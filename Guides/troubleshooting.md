---
description: Comprehensive troubleshooting and FAQ for Stardew Valley mod collections. Covers installation issues, gameplay problems, mod manager errors, SMAPI errors, and common fixes.
keywords: troubleshooting, SMAPI errors, mod installation, Vortex troubleshooting, Nexus Mods App issues, Stardrop, manual installation, duplicate mods, corrupted farm map, crafting issues, Better Crafting, mod conflicts, collection updates
tags: [troubleshooting, faq, installation, errors, fixes, SMAPI, Vortex, NMA]
---

# Troubleshooting & FAQ

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* 1.6.15+

---

## Table of Contents

- [Quick Fix](#quick-fix-try-restarting-first)
- [Problem-Symptom Index](#problem-symptom-index)
- [Find the Right Troubleshooting Guide](#find-the-right-troubleshooting-guide)
- [Getting Started FAQs](#getting-started-faqs)
- [Gameplay FAQs](#gameplay-faqs)
- [Setup & Customization FAQs](#setup--customization-faqs)
- [Installation-Specific FAQs](#installation-specific-faqs)
- [Common Issues](#common-issues)
- [Known Technical Issues](#known-technical-issues)
- [Vortex-Specific Troubleshooting](#vortex-specific-troubleshooting)
- [How to Create a SMAPI Log](#how-to-create-a-smapi-log)
- [Need More Help?](#need-more-help)

---

## Quick Fix: Try Restarting First!

Before diving into complex troubleshooting steps, restart your computer and try again. Many issues with Vortex, SMAPI, or the game itself can be resolved with a simple restart.

**For Vortex users:** If restarting doesn't help, try the [Vortex Quick Fix Process](../Installation/Vortex/troubleshooting.md#quick-fix-process) which includes game installation checks, profile verification, and mod folder cleanup.

---

## Problem-Symptom Index

Quick reference guide to find solutions based on what you're experiencing:

| Symptom / Problem | Quick Link | Category |
|-------------------|------------|----------|
| **Game won't start / SMAPI errors** | [SMAPI Log Guide](#how-to-create-a-smapi-log) | Installation |
| **Missing mods in game** | [Duplicate Mods](#duplicate-mods) or [NMA Installation Bug](../Installation/nma.md#known-issues) | Installation |
| **Can't craft items despite having ingredients** | [Better Crafting Quality Filters](#setup--customization-faqs) | Gameplay |
| **Corrupted farm map / Can't exit house** | [Farm Map Issues](#cant-exit-house--corrupted-farm-map) | Gameplay |
| **Mods not updating** | [Updating Collections](updating-collections.md) | Installation |
| **Vortex file conflicts / loops** | [Vortex Troubleshooting](../Installation/Vortex/troubleshooting.md#common-error-messages) | Installation |
| **Game loading very slowly** | [Slow Loading](#why-is-my-game-loading-slowly) | Performance |
| **Multiplayer desync** | [Multiplayer Issues](#multiplayer--split-screen-desync) | Multiplayer |
| **Community Center cutscene won't trigger** | [svVe FAQ](../Collections/Stardew%20Valley%20VERY%20Expanded/faq.md#community-center-cutscene-wont-trigger) | Gameplay |
| **Minecart blocking mine entrance** | [svVe FAQ](../Collections/Stardew%20Valley%20VERY%20Expanded/faq.md#minecart-blocks-the-mine-entrance) | Gameplay |
| **Can't find Rusty/Sewer Key** | [svVe FAQ](../Collections/Stardew%20VALLEY%20VERY%20Expanded/faq.md#rustysewer-key-changes-in-sve) | Gameplay |
| **Expansion NPCs stuck in house on first day** | [svVe FAQ](../Collections/Stardew%20Valley%20VERY%20Expanded/faq.md#expansion-npcs-not-leaving-house-on-first-day) | Gameplay |
| **SMAPI log shows "Empty Vortex folder"** | [Vortex Troubleshooting](../Installation/Vortex/troubleshooting.md#empty-vortex-folder-is-the-mod-disabled-in-vortex) | Installation |
| **Vortex "write-protected" error** | [Vortex Troubleshooting](../Installation/Vortex/troubleshooting.md#vortex-needs-access-to-file-but-its-write-protected) | Installation |
| **NMA mods in wrong folder** | [NMA Known Issues](../Installation/nma.md#known-issues) | Installation |
| **MacOS SMAPI security issues** | [MacOS Installation](#macos-installation) | Installation |

---

## Find the Right Troubleshooting Guide

Use this table to find the most relevant troubleshooting or FAQ page for your issue:

| Issue Type | Resource | Description |
|------------|----------|-------------|
| **Vortex Issues** | [Vortex FAQ & Troubleshooting](../Installation/Vortex/troubleshooting.md) | Vortex-specific questions, installation problems, profile issues, and mod deployment errors |
| **svVe Gameplay** | [svVe FAQ & Troubleshooting](../Collections/Stardew%20Valley%20VERY%20Expanded/faq.md) | Gameplay questions and issues specific to Stardew Valley VERY Expanded (community center, minecart, crafting, etc.) |
| **NMA Issues** | [NMA Guide](../Installation/nma.md) | Questions and troubleshooting for Nexus Mods App |
| **Stardrop Issues** | [Stardrop Guide](../Installation/stardrop.md) | Questions and troubleshooting for Stardrop mod manager |
| **Manual Installation** | [Manual Guide](../Installation/manual.md) | Questions and limitations for manual installation |

---

## Getting Started FAQs

### Do I need the optional mods?
> Yes! While some mods are marked as "optional" to make it easier when combining collections, you should install them when using a single collection. These optional mods include:
> - Essential interface improvements 
> - Map enhancements that improve the visual experience
> - Additional content that enhances gameplay
> - Expansions that have been carefully curated for quality
> - Compatibility files for combining collections (only needed when stacking multiple collections)
> 
> The optional designation exists mainly to help with collection stacking (combining multiple collections). When using just one collection, these mods are designed to be part of the intended experience.

### Should I update individual mods myself?
> It's recommended to wait for the collection to be updated instead of updating individual mods yourself. The collection curator tests all mod versions together to ensure compatibility. Updating mods individually can cause version conflicts, breaking changes, missing compatibility patches, and unstable gameplay. When a collection update is released, it includes tested versions of all mods that work together.

### Can I combine your collections?
> Yes! Any Aesthetic Valley collection (Fairycore, Witchcore, or future Aesthetic Valley collections) is designed to work alongside Stardew Valley VERY Expanded (svVe). You can install them into the same Vortex profile.
> 
> For detailed instructions on how to combine collections, including which optional mods to install and how to manage conflicts, see the [Combining Collections](../Collections/combining-collections.md) guide.

### Can I play svVe if I haven't played Stardew Valley before?
> It's absolutely fine to start with svVe even if you're new to Stardew Valley! The collection is designed to enhance the game while preserving the vanilla feel. However, keep in mind that svVe is quite large with many new areas, NPCs, and content.
> 
> **Recommendation:** Playing vanilla Stardew Valley first will help you appreciate the additions svVe brings, but it's not required. If you're eager to dive in with the collection, go for it - just be prepared for a lot more content to explore!

### Co-op
> All players in a multiplayer game must have matching mods and configurations for everything to work correctly. This means:
> - All players need the same collection(s) installed
> - All players need the same mod versions
> - All players need matching configurations (especially for mods that affect gameplay)
> 
> Consider using a multiplayer manager or keeping careful documentation of your mod setup so everyone can stay in sync. Version mismatches can cause desyncs, crashes, or missing content.

### Where can I download these collections?
> **Download collections:** [JennaJuffuffles Collections on Nexus Mods](https://next.nexusmods.com/profile/JennaJuffuffles/collections)
> 
> These collections are only available and updated through **Nexus Mods**. This is the official source and ensures you always get the latest tested versions. All collections must be installed through Nexus so each mod download is properly attributed to its creator.
> 
> Using **Nexus Premium** helps support Nexus Mods and the mod creators on the platform. Nexus Premium also enables one-click installation through Vortex, making collection setup much easier and faster. However, you can still use Vortex for free to download and install, it just requires a bit more clicking.

### Can I get all the mods in a zip file?
> While this would be convenient, I can't provide a zip file with all mods. Collections work differently from modpacks - they reference mods hosted on Nexus Mods rather than bundling them together. This ensures each mod download is properly attributed to its creator. Providing a zip file would redistribute mods without creators' permission, which is mod piracy. Collections must be installed through Nexus so each mod download is tracked correctly and creators receive proper credit for their work.

### Why is my game loading slowly?
> Large collections can take several minutes to load, especially on the first launch or when starting a new save. This is normal due to the amount of content being loaded.
> 
> **⚠️ Important:** During loading, please don't alt-tab, click away, or interact with the game window. Doing so can cause crashes or freezes. Just let it load - you'll see progress in the SMAPI console window. The game will be ready when the console stops showing loading messages.

### Mobile support
> The status of mobile support can change rapidly. It's recommended to try with the [1.5.6 version collection](https://www.nexusmods.com/games/stardewvalley/collections/9sf9yn), but support is not guaranteed or known. Mobile modding has significant limitations and compatibility issues that may prevent collections from working properly. Stardew Valley on iOS cannot be modded. 

---

## Gameplay FAQs

For svVe-specific gameplay questions including Community Center cutscenes, Rusty/Sewer Key changes, minecart blocking the mine entrance, duplicated NPCs, East Scarp festival attendance, crafting issues, and performance problems, see the [svVe FAQ](../Collections/Stardew%20Valley%20VERY%20Expanded/faq.md).

### Can't exit house / corrupted farm map

**Symptom:** Unable to exit your house or see a corrupted farm map (missing textures, black areas, or errors)

**Cause:** Farm map mod is disabled or failed to load properly

**Solution:**
1. Open your mod manager 
2. Find your farm map mod 
3. Make sure it's **Enabled** 
4. Check that no other farm map mods are enabled - only one farm map should be active at a time
5. Click **Deploy** to apply the changes
6. Restart the game and load your save

**Important:** Farm maps cannot be switched mid-save without special tools. If you want to change your farm map, you'll need to start a new save file, or use a tool like [Easy Farm Switcher](https://www.nexusmods.com/stardewvalley/mods/16873) which can handle the transition (though this should be done carefully and with backups).

**See Also:**
- [Vortex Troubleshooting](../Installation/Vortex/troubleshooting.md) - If using Vortex
- [Duplicate Mods](#duplicate-mods) - If mods aren't loading

---

## Setup & Customization FAQs

### Can I add more mods?
> Yes! These collections are designed as solid bases that you can build upon. However, there are some important things to keep in mind:
> 
> - **Test additions individually** - Add one mod at a time and test thoroughly before adding another. This helps you identify any conflicts quickly.
> - **Review compatibility notes** - Check mod pages for compatibility warnings, especially with major expansions like SVE, Ridgeside Village, or East Scarp.
> - **Create a private collection** - Once you've found mods that work well, create a private collection containing just your additions. This makes it easy to reinstall them after collection updates. See the [Personalization guide](personalization.md) for details.
> - **Check load order** - Some mods may need specific load orders. Use Vortex's "Manage Rules" to adjust if needed.
> 
> Remember that adding mods can introduce conflicts or bugs, and collection updates may not account for your additions. Keep backups of working configurations!

### Can I disable a required mod?
> You can disable a required mod, but it requires manual management since the collection expects it to be enabled.
> 
> **For Vortex users:**
> 1. Go to the **Mods** tab
> 2. Find the mod you want to disable and toggle it off
> 3. The collection will show a warning - this is expected
> 4. Click **Deploy** to apply the change
> 
> **Tip:** Add the **Collections** column in Mod view to help track which mods belong to which collection. This makes it easier to see what you've modified and manage visibility.
> 
> **For Nexus Mods App users:**
> You'll need to create a collection clone to disable required mods, as NMA doesn't allow disabling required mods directly in a collection. Create a clone of the collection and modify it to remove or disable the required mods you don't want.
> 
> **Warning:** Disabling required mods can break functionality, cause crashes, or create gameplay issues. Only disable mods if you understand what they do and are prepared to troubleshoot problems. Some mods are required because others depend on them.

---

## Installation-Specific FAQs

For mod-manager-specific questions and troubleshooting:

- [Vortex FAQ & Troubleshooting](../Installation/Vortex/troubleshooting.md)
- [Nexus Mods App Guide](../Installation/nma.md)
- [Stardrop Guide](../Installation/stardrop.md)
- [Manual Installation Guide](../Installation/manual.md)

### MacOS Installation

#### Mod Managers
> Nexus Mods App has planned support for MacOS, but currently no mod manager with collection support exists. Mac users may use the [Manual Installation](../Installation/manual.md) guide or the [Stardrop](../Installation/stardrop.md) guide and transfer from a Windows machine.

#### MacOS SMAPI Security Issues

> **Important:** Certain MacOS versions flag SMAPI as malware and forcibly move it to the trash, preventing installation.
> 
> *The following solutions are based on community findings, derivded from the Stardew community Discord, and may change as Apple updates MacOS security behaviors.*

#### Problem 1: Unable to Run SMAPI Installer
> When you receive a security message, go to Settings > Security (or Privacy & Security) and hit "Open Anyways" where it lists the blocked file.

#### Problem 2: MacOS reports "Malware Blocked and Moved to Trash"
> Enable MacOS security permissions:
> 
> 1. Go to System Settings > Privacy and Security
> 2. Make sure Developer Tools is visible. If you don't see it, open Terminal through Spotlight and enter:
>    ```
>    spctl developer-mode enable-terminal
>    ```
> 3. Click Developer Tools
> 4. Add Terminal to the list and enable it
> 5. If you have other terminal programs (iTerm2, Hyper, Kitty, Alacritty), add them to Developer Tools as well
> 6. Restart your computer
> 7. Force close Steam if using it
> 8. Download and reinstall SMAPI
> 
> **Note:** This solution may change over time as Apple updates MacOS security behaviors. If this doesn't work:
> - Restart your computer again
> - Force close Steam, then try installing SMAPI
> - Check the [SMAPI Mac installation wiki](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Mac) for updated solutions
> 
> *For the most current solutions and community discussions, visit the the [SMAPI GitHub repository](https://github.com/Pathoschild/SMAPI).*

For Vortex-specific troubleshooting, see the [Vortex Troubleshooting](../Installation/Vortex/troubleshooting.md) guide.

---

## Common Issues

### Duplicate Mods

**Symptom:** SMAPI shows red errors about duplicate mods, or mods aren't loading

**Cause:** Two copies of a mod exist, or mods are nested inside subfolders. When two copies of a mod exist, neither will load. This includes if a mod is inside of a subfolder inside of the `Mods/` folder.

**Solution:**
- Check your `Mods/` folder for any duplicate mod directories
- Look for mods nested inside subfolders - mods should be directly in `Mods/` (e.g., `Mods/ModName/manifest.json`, not `Mods/Folder/ModName/manifest.json`)
- Remove any duplicate or incorrectly placed mod folders
- Restart the game and check the SMAPI log to confirm the mod loads correctly

**Important:** It is recommended that the mod folder be clear when installing a new collection (unless deliberately stacking collections). For more information on adding mods and managing your setup, see the [Can I add more mods?](#can-i-add-more-mods) section above.

**See Also:**
- [SMAPI Log Guide](#how-to-create-a-smapi-log) - To verify mods are loading correctly
- [Vortex Troubleshooting](../Installation/Vortex/troubleshooting.md) - If using Vortex
- [NMA Known Issues](../Installation/nma.md#known-issues) - If using Nexus Mods App

---

## Known Technical Issues

### Multiplayer / split-screen desync

**Symptom:** Players seeing different things, actions not registering, or players getting stuck in multiplayer

**Cause:** Usually a temporary network or mod state issue, or mod/version mismatch between players

**Solution:**
1. **Relaunch the game** - All players should quit and restart the game completely
2. **Restart the session** - The host should save, close the game, and start a new multiplayer session
3. **Check mod sync** - Ensure all players have the exact same mods enabled and the same versions
4. **Verify configurations match** - Important mod configurations should be identical across all players

**Note:** Split-screen co-op may exhibit unusual behavior while modded. Feedback via [Discord](https://discord.gg/MPcgJUXeeY) is always appreciated to help improve mod compatibility with split-screen multiplayer.

Persistent desync issues may indicate mod conflicts or version mismatches. Check the SMAPI logs from all players for errors.

**See Also:**
- [Co-op FAQ](#co-op) - General multiplayer requirements
- [SMAPI Log Guide](#how-to-create-a-smapi-log) - To diagnose mod conflicts

### Failed to Store Cache Entry (SinZational Speedy Solutions)

**Symptom:** Error message in SMAPI log: "Failed to Store Cache Entry" related to SinZational Speedy Solutions

**Cause:** Informational message, not an actual error

**Solution:** **No action needed** - This is completely safe to ignore.

**Details:**
- It does **not** indicate a crash or conflict
- It does **not** affect gameplay
- Your game will run normally despite this message
- This is communicating that the mod failed to cache the map, but functionally this means the map still will load normally

You can safely continue playing!

### Is JennaJuffuffles affiliated with Nexus Mods?
> No. JennaJuffuffles is an independent collection curator and is not affiliated with or employed by Nexus Mods. As such, JennaJuffuffles is not responsible for:
> - Changes to the Nexus Mods website or platform
> - How Nexus Premium works, its pricing, or its features
> - Issues with Nexus Mods services, servers, or account access
> - Mod manager updates or changes (Vortex, Nexus Mods App, etc.)
> - Decisions made by Nexus Mods or its staff
> 
> For questions or issues related to Nexus Mods services, account access, Premium subscriptions, or platform features, please contact [Nexus Mods Support](https://help.nexusmods.com/).

---

## Vortex-Specific Troubleshooting

For Vortex-specific troubleshooting steps including game installation checks, profile verification, and mod folder management, see the [Vortex Troubleshooting](../Installation/Vortex/troubleshooting.md) guide.

**See Also:**
- [Problem-Symptom Index](#problem-symptom-index) - Quick reference for common Vortex issues
- [Common Issues](#common-issues) - General mod installation problems
- [Installation-Specific FAQs](#installation-specific-faqs) - Mod manager comparisons

---

## Additional Resources for Expansion Mods

**Important:** Please avoid troubleshooting in these Discords unless you can show (via log) a repeatable error from their mod without the rest of the collection active. Please be respectful of other's time, and understand that many helpers are not comfortable with mod managers other than Stardrop.

If you're experiencing issues with specific expansion mods, these resources may help:

### Stardew Valley Expanded
- [Installation Guide](https://github.com/FlashShifter/StardewValleyExpanded/wiki/Install-guide)
- [Troubleshooting](https://github.com/FlashShifter/StardewValleyExpanded/wiki/Troubleshooting)
- [Wiki](https://stardew-valley-expanded.fandom.com/wiki/Stardew_Valley_Expanded_Wiki)
- [Discord](https://discord.com/invite/svexpanded)

### Ridgeside Village
- [Installation Guide](https://github.com/Rafseazz/Ridgeside-Village-Mod/blob/main/Installation%20Guide.md)
- [Wiki](https://ridgeside.fandom.com/wiki/Ridgeside_Village_Wiki)
- [Discord](https://discord.gg/4SRbjEQG2D)

### East Scarp and Sword & Sorcery, Lurking in the Dark, Nora, etc
- [Wiki](https://eastscarp.fandom.com/wiki/East_Scarp_Wiki)
- [Discord](https://discord.com/invite/QFtDA3CJwJ)

---

## How to Create a SMAPI Log

A SMAPI log is a text file that shows what mods loaded and any errors that occurred.
Share the link in the [Discord](https://discord.gg/MPcgJUXeeY) for help!

### Windows Users:
1. Press the **Windows** and **R** keys at the same time.
2. In the 'Run' box that appears, enter:
   ```
   %appdata%\StardewValley\ErrorLogs
   ```
3. The log file is `SMAPI-crash.txt` if it exists, otherwise `SMAPI-latest.txt`. Upload it to [smapi.io/log](https://smapi.io/log).

### Linux Users:
1. Open the Files app.
2. Click the options menu (might be labeled Go or ⋮).
3. Choose Enter Location.
4. Enter this exact text:
   ```
   ~/.config/StardewValley/ErrorLogs
   ```
5. The log file is `SMAPI-crash.txt` if it exists, otherwise `SMAPI-latest.txt`. Upload it to [smapi.io/log](https://smapi.io/log) 

### Mac Users:
1. Open the Finder app.
2. Click Go at the top, then Go to Folder.
3. Enter this exact text:
   ```
   ~/.config/StardewValley/ErrorLogs
   ```
4. The log file is `SMAPI-crash.txt` if it exists, otherwise `SMAPI-latest.txt`. Upload it to [smapi.io/log](https://smapi.io/log) 


**Tip:** The log will show a lot of information about your setup, exactly which mods loaded successfully and highlight any problems in red. This information can help in troubleshooting even when a crash isn't specifically displayed.

---

## Need More Help?

If you run into issues that aren't solved here, you can:
- Reach out to the community on **[Discord](https://discord.gg/MPcgJUXeeY)** for live assistance
- Create and share a SMAPI log so others can help diagnose your issue

### Additional Support Resources

**For Vortex support:**
- **Official Vortex Discord**: [Join Here](https://discord.com/invite/nexusmods) (Support hours: 9 AM – 5 PM GMT, Monday–Thursday)
- **Vortex Wiki**: [Read Here](https://wiki.nexusmods.com/index.php/Category:Vortex)
- **Stardew Setup Guide**: [Read Here](https://wiki.nexusmods.com/index.php/Modding_Stardew_Valley_with_Vortex)

> **Note:** The **official Stardew Valley Discord** does *not* support Vortex. Please respect their policy.

---

## See Also

- [Updating Collections](updating-collections.md) - If issues started after an update
- [Personalization Guide](personalization.md) - If you've customized your setup
- [Combining Collections](../Collections/combining-collections.md) - If using multiple collections
- [Mod Managers Overview](../Installation/index.md) - To compare installation methods
