# Installing to an Existing Save
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

Stardew Valley VERY Expanded is best experienced on a new save. Installing on an advanced save may effect progress, confuse quest flags, or have other unexpected effects.

If you still want to install a collection to a save file that already has mods, this guide covers what to expect, compatibility issues, and the cleanup tools necessary to successfully install collections to existing saves.

The cleanup steps below were written for Vortex, but the tools and save warnings apply no matter which manager you use. Install the collection with [Install with Vortex](vortex.md), [Install with Stardrop](stardrop.md), or [Install with Amethyst](amethyst.md).

## Before You Begin

**Important:** Back up your save files before making changes. See the [Stardew Valley Wiki Saves page](https://www.stardewvalleywiki.com/Saves) for instructions.

---

## Important Considerations

This guide assumes:
- You are not using a previously modded save or that your modded save was using mods that are present in the collection
- You do not have unmanaged mods in your mods folder (mods installed outside of Vortex)
- You are installing the collection to a new Vortex profile

{% hint style="info" %}
This works best when your save was un-modded or created with mods included in the collection. If your save was created with different mods, switching major expansion mods, or changing farm maps, you may encounter issues that require cleanup tools or starting a new save.
{% endhint %}

---

## Clean-up Process

### Step 1: Clean Save File and Mod Folder

{% hint style="info" %}
If you have an unmodded save, skip Step 1 entirely and proceed directly to [Step 2: Verify Game Files](#step-2-verify-game-files).
{% endhint %}

If you have a modded save (mods currently installed), you need to clean up your save file before removing mods. This prevents null items, broken NPCs, and save corruption.

{% hint style="danger" %}
Do not remove mods that modify Community Center bundles on existing saves. The game's bundle system doesn't support mid-save changes. If your save has bundle modifications, you'll need to start a new save or keep those mods.
{% endhint %}

1. Remove mod-related items from your inventory and chests (items from mods will be in the collection are fine to keep)
2. Remove mod-related animals (animals from mods that will be in the collection are fine to keep
3. Remove mod-related crops (crops from mods that will be in the collection are fine to keep)
4. Divorce any NPCs from mods that will be in the collection

{% hint style="info" %}
Vortex users should remove any unmanaged mods:
1. In Vortex, go to the **Mods** tab
2. Click **Purge Mods** to remove all active mods
3. Click **Open > Game Mods Folder**
4. Remove everything from the Mods folder (files and subfolders)
5. Click **Deploy** in Vortex only once that folder is completely empty  
{% endhint %}

This will remove any outdated, leftover files from the mods folder that aren't managed by Vortex.

### Step 2: Install the Collection

Follow [Install with Vortex](vortex.md), [Install with Stardrop](stardrop.md), or [Install with Amethyst](amethyst.md) to install the collection fresh.

---

### Step 3: Testing and Clean-Up

1. Test the collection on a new save before making further customizations (adding extra mods, adjusting mod config files, etc.)
2. Launch the game and check [Your SMAPI Log](../Troubleshooting/your-smapi-log.md) for errors
3. Launch your existing save and check your inventory and chests for 🚫 symbol items (null items from removed mods)
4. Check interior spaces like sheds, basements, and greenhouses for misplaced items or crops
5. If you see errors or issues, review the [Common Issues You May Encounter](#common-issues-you-may-encounter) section above
6. Use appropriate cleanup tools if needed (see [Clean-up Tools](#clean-up-tools) section below)
7. Add any additional desired mods back in methodically, reviewing each mod's About page and loading to the main menu to check for compatibility
8. Some saves may need to be started fresh if they had incompatible mods

## What to Expect After Installation

### Common Issues You May Encounter

When installing or removing mods on existing saves, you may encounter issues that require cleanup tools. Common problems include:

- **Null items** (🚫 symbol) - Items from removed mods appearing in your inventory, chests, or in the world (e.g., null trees from removing SVE)
- **Items in wrong locations** - Items, crops, or furniture misplaced when mods that changed building layouts are removed
- **Characters or items in "voids"** - NPCs or objects in inaccessible areas after farm map changes
- **Farm map mismatches** - Buildings and terrain features not matching the new farm map
- **Broken NPCs** - Missing characters, broken relationships, or dialogue errors after removing NPC mods

## Clean-up Tools

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

## Related

- [Install with Vortex](vortex.md)
- [Your SMAPI Log](../Troubleshooting/your-smapi-log.md)
- [Known Issues](../Troubleshooting/known-issues.md)
- [Vortex Notifications](../Troubleshooting/vortex-notifications.md)
