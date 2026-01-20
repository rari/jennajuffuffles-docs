---
title: Installing Collections to Existing Saves
description: Install Stardew Valley collections to existing save files safely. Learn about compatibility issues, cleanup tools, and considerations for saves with existing mods.
keywords: [existing saves, installing to existing saves, save compatibility, cleanup tools, save migration, mod installation, removing mods, save safety]
tags: [installation, saves, existing-saves, compatibility]
---

# Installing Collections to Existing Saves

*Last updated:* 2026-01-19  
*Applies to Stardew Valley:* 1.6.15+

If you want to install a collection to a save file that already has mods, there are important considerations and tools you'll need. This guide covers what to expect, compatibility issues, and the cleanup tools necessary to successfully install collections to existing saves.

---

## Table of Contents

- [Before You Begin](#before-you-begin)
- [Important Considerations](#important-considerations)
- [Clean-up Process](#clean-up-process)
  - [Step 1: Remove Existing Mods](#step-1-remove-existing-mods)
  - [Step 2: Verify Game Files](#step-2-verify-game-files)
  - [Step 3: Install the Collection](#step-3-install-the-collection)
  - [Step 4: Testing and Clean-Up](#step-4-testing-and-clean-up)
- [What to Expect After Installation](#what-to-expect-after-installation)
- [Cleanup Tools](#cleanup-tools)
- [See Also](#see-also)

---

## Before You Begin

**Important:** Back up your save files before making changes. See the [Stardew Valley Wiki Saves page](https://www.stardewvalleywiki.com/Saves) for instructions.

---

## Important Considerations

This guide assumes:
- You are **not using a previously modded save**, OR your modded save was using mods that are present in the collection
- You do **not have unmanaged mods** (mods installed outside of Vortex)
- You are installing the collection to a **new Vortex profile**

Installing a collection to an existing save means you want to continue playing your save file with the collection. Some changes cannot be safely made to existing saves, and you may need cleanup tools to fix issues that arise.

{% hint style="info" %}
This works best when your save was un-modded or created with mods included in the collection. If your save was created with different mods, switching major expansion mods, or changing farm maps, you may encounter issues that require cleanup tools or starting a new save.
{% endhint %}

---

## Clean-up Process

### Step 1: Remove Existing Mods

{% hint style="info" %}
If you have an unmodded save, skip Step 1 entirely and proceed directly to [Step 2: Verify Game Files](#step-2-verify-game-files).
{% endhint %}

**If you have a modded save** (mods currently installed), you need to clean up your save file BEFORE removing mods. This prevents null items, broken NPCs, and save corruption.

{% hint style="danger" %}
Do not remove mods that modify Community Center bundles on existing saves. The game's bundle system doesn't support mid-save changes. If your save has bundle modifications, you'll need to start a new save or keep those mods.
{% endhint %}

1. **Remove mod-related items** from your inventory and chests (items from mods that won't be in the collection)
2. **Remove mod-related animals** (animals from mods that won't be in the collection)
3. **Remove mod-related crops** (crops from mods that won't be in the collection)
4. **Divorce any NPCs** from mods that won't be in the collection

**Now remove any unmanaged mods:**
1. In Vortex, go to the **Mods** tab
2. Click **Purge Mods** to remove all active mods
3. Click **Open > Game Mods Folder**
4. **Remove everything** from the Mods folder (files and subfolders)

This will remove any outdated, leftover files from the mods folder that aren't managed by Vortex.

### Step 2: Verify Game Files
Use your store launcher to verify game file integrity. How this is done will vary from store to store. 
See [Verifying Game Files](index.md#verifying-game-files) for detailed instructions.

This ensures your game is in a clean state before installing the collection


### Step 3: Install the Collection

Follow the [Step-by-Step Installation](index.md#step-by-step-installation) instructions to install the collection fresh

---

## What to Expect After Installation

### Common Issues You May Encounter

When installing or removing mods on existing saves, you may encounter issues that require cleanup tools. Common problems include:

- **Null items** (🚫 symbol) - Items from removed mods appearing in your inventory, chests, or in the world (e.g., null trees from removing SVE)
- **Items in wrong locations** - Items, crops, or furniture misplaced when mods that changed building layouts are removed
- **Characters or items in "voids"** - NPCs or objects in inaccessible areas after farm map changes
- **Farm map mismatches** - Buildings and terrain features not matching the new farm map
- **Broken NPCs** - Missing characters, broken relationships, or dialogue errors after removing NPC mods

If you encounter issues after installation, see the [Troubleshooting guide](../Troubleshooting/index.md) for help. The [Cleanup Tools](#cleanup-tools) section below lists specific tools to address these problems.

---

### Step 4: Testing and Clean-Up

1. Test the collection on a new save before making further customizations (adding extra mods, adjusting mod config files, etc.)
2. Launch the game and check the [SMAPI log](../Troubleshooting/your-smapi-log.md) for errors
3. Launch your existing save and check your inventory and chests for 🚫 symbol items (null items from removed mods)
4. Check interior spaces like sheds, basements, and greenhouses for misplaced items or crops
5. If you see errors or issues, review the [Common Issues You May Encounter](#common-issues-you-may-encounter) section above
6. Use appropriate cleanup tools if needed (see [Cleanup Tools](#cleanup-tools) section below)
7. Add any additional desired mods back in methodically, reviewing each mod's About page and loading to the main menu to check for compatibility
8. Some saves may need to be started fresh if they had incompatible mods


## Cleanup Tools

When installing collections or removing mods from existing saves, you may need these tools:

- **[CJB Cheats Menu](https://www.nexusmods.com/stardewvalley/mods/4)** - Pause time and fix relationships
- **[CJB Item Spawner](https://www.nexusmods.com/stardewvalley/mods/93)** - Delete null items 🚫 and replace missing items
- **[Noclip Mode](https://www.nexusmods.com/stardewvalley/mods/3900)** - Move outside of boundaries (keybind toggle F11)
- **[Let's Move it](https://www.nexusmods.com/stardewvalley/mods/20943)** - Easily move trees, crops, and other objects
- **[Destroyable Bushes](https://www.nexusmods.com/stardewvalley/mods/6304)** - Allows players to destroy bushes with an axe. This can be a quick way of removing bushes that were placed by the original mod setup and are now blocking paths
- **[Farm Switcher](https://www.nexusmods.com/stardewvalley/mods/16873)** - Allows player to switch farm maps mid-play **Note:** Convert in single player mode before using in co-p.
- **[Reset Terrain Tool](https://github.com/Lake1059/ResetTerrainFeatures_NET6/releases/download/1.0.3-unofficial.3-Lake1059/SDV_1.6.10_RTF-1.0.3-unofficial.3-Lake1059.zip)** - Update terrain features per-map. Clear, reset, or regenerate terrain features (trees, rocks, bushes, debris) that auto-spawn on maps. Useful when maps are out of place after installing or removing map mods
- **Console Commands** - See [SMAPI Console Commands](https://stardewvalleywiki.com/Modding:Console_commands) for available debug commands

After you are finished using these cleanup tools and your game has saved, you can safely exit and disable these mods.

---

## See Also

- [New Player Install Instructions](index.md) - Installation guide
- [Troubleshooting & FAQ](../Troubleshooting/index.md) - For issues after installation
- [Your SMAPI Log](../Troubleshooting/your-smapi-log.md) - To verify everything loaded correctly
- [Vortex Troubleshooting](../Troubleshooting/vortex-troubleshooting.md) - For load order issues and conflict notifications
- [Installing Multiple Collections](multiple-collections.md) - If combining collections
