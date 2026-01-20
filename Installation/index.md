---
title: Installing Stardew Valley Mod Collections
description: Step-by-step installation guide for Stardew Valley mod collections using Vortex. Learn how to install collections, set up SMAPI, handle optional mods, and resolve conflicts.
keywords: [Vortex installation, mod collection installation, SMAPI setup, new player guide, Nexus Premium, optional mods, conflict resolution, Manage Rules]
tags: [installation, vortex, new-player, getting-started, smapi]
---

# New Player Install Instructions

*Last updated:* 2026-01-19  
*Applies to Stardew Valley:* 1.6.15+

This guide walks you through installing a mod collection using Vortex, step by step. Follow these instructions in order for the best experience.

**Not a new player, or need a different installation method?**
- **[Installing Multiple Collections](multiple-collections.md)** - For combining collections together
- **[Installing to Existing Saves](installing-to-existing-saves.md)** - For installing collections to saves that already have mods
- **[Manual Installation](manual.md)** - For users who can't use mod managers
- **[Sideload to Stardrop](stardrop.md)** - For Stardrop users
- **[Sideload to Steam Deck](steam-deck.md)** - For Steam Deck users
- **[Using a Controller](controller.md)** - For controller-specific setup

---

## Table of Contents

- [Verifying Game Files](#verifying-game-files)
- [Manage Stardew Through Vortex](#manage-stardew-through-vortex)
- [Clearing Your Mod Folder](#clearing-your-mod-folder)
- [Installation Process](#installation-process)
- [Optional Mods](#optional-mods)
- [Installing SMAPI](#installing-smapi)
- [Connecting SMAPI to Your Store](#connecting-smapi-to-your-store)
- [De-SVE-ing a Collection](#de-sve-ing-a-collection)

---

## Verifying Game Files

Before installing mods, make sure your game files are healthy and up to date.

### Why Verify?

- Ensures you have the latest game version (required for mod compatibility)
- Fixes any corrupted game files
- Prevents installation issues

{% hint style="danger" %}
Always verify and run the game before installing mods. This ensures your game is ready for modding.
{% endhint %}

### How to Verify

**Steam:**
1. Open Steam Library
2. Right-click **Stardew Valley**
3. Select **Properties > Installed Files**
4. Click **Verify integrity of game files**

**GOG:**
1. Open GOG Galaxy
2. Right-click **Stardew Valley**
3. Select **Manage Installation > Verify / Repair**

**Xbox / Game Pass:**
1. Open Xbox app
2. Right-click **Stardew Valley**
3. Select **Manage > Files > Verify and Repair**

### After Verifying

1. **Run the game once** through your normal launcher (Steam, GOG, etc.)
2. Let it complete the initial setup
3. Close the game

---

## Manage Stardew Through Vortex

Vortex needs to know you want to manage Stardew Valley mods.

### Initial Setup

1. [Download and install Vortex Mod Manager](https://www.nexusmods.com/site/mods/1?tab=files) if you haven't already
2. Open Vortex
3. Go to the **Games** tab
4. Find **Stardew Valley** in the list
5. Click **Manage** (or **Manage Stardew Valley**)

Vortex will now detect and manage Stardew Valley mods.

### Symbolic Links (Important for Non-C: Drives)

If Stardew Valley is **not** installed on drive `C:\`, you need to enable symbolic links:

1. Go to **Settings** (gear icon in Vortex)
2. Navigate to **Mods** section
3. Enable **Use Symbolic Links**
4. Click **Apply**

Symbolic links allow Vortex to manage mods even when the game is on a different drive. Without this, mods may not deploy correctly.

---

## Clearing Your Mod Folder

Before installing a collection, you need a clean slate. Any existing mods or leftover files can cause conflicts.

1. If you have other Stardew Valley mods managed in Vortex, disable them.
2. In the **Mods** tab, click **Open > Game Mods Folder**
3. **Remove everything** from this folder (files and subfolders)
4. Close the folder window

Old mod files can conflict with collection mods, causing crashes, missing content, or other issues. Starting fresh ensures everything works correctly.

---

## Installation Process

Follow these steps to install a collection. Browse available [Jenna Juffuffles' collections](https://www.nexusmods.com/profile/JennaJuffuffles/collections)

### Step-by-Step Installation

1. Ensure Vortex is open
2. Click **Add Collection** on the collection page
3. Pop-up in browser will ask you to use a Mod Manager, click **Continue**
4. Vortex will display the collection, click **Install Now**
   - **For Premium users:** Vortex handles everything automatically
   - **For Free users:** You'll need to click buttons to download the mods from the pages Vortex opens for you. All mods are hosted on Nexus.
5. When prompted about optional mods, click **OK/Install**
6. Optional mods may have additional instructions, and you may skip or install each

### Installing Multiple Collections

You can combine multiple collections (for example, Stardew Valley VERY Expanded with an Aesthetic Valley collection) by installing them to the same Vortex profile.

{% hint style="info" %}
See [Installing Multiple Collections](multiple-collections.md) for detailed guidance on combining collections, resolving conflicts, and managing optional mods.
{% endhint %}

### Nexus Premium vs Free

The installation process differs based on whether you have Nexus Premium or are using the free version.

**Nexus Premium:**
- **Fully automated downloads** - All mods download automatically
- **Fewer manual steps** - Just click "Add Collection" and let it run
- **Faster installation** - No waiting for individual downloads

**Free Version:**
- **Step-by-step prompts** - Vortex guides you through each mod
- **Manual downloads required** - You'll need to download each mod from Nexus

{% hint style="info" %}
Both methods result in the same installed collection. Premium saves time, but collections are kept small to make them easier for free users to download manually through Vortex.
{% endhint %}

---

## Optional Mods

Collections include **required mods** and **optional mods**. Here's what you need to know:

### Required Mods

These are **essential** and must be installed:
- Core framework mods (like SMAPI)
- Mods that other mods depend on
- Critical gameplay mods

**You cannot skip these** - the collection is intended to be installed with these mods.

### Optional Mods

Optional mods are included for different reasons:

**Performance considerations:**
- **Expansion content** - Large content mods that may impact performance on lower-end systems
- **Memory-heavy visual mods** - Visual enhancements that require more system resources

**Compatibility and conflicts:**
- **Compatibility files** - May not be needed depending on your other installed mods
- **Farm map variations** - Only one farm map can be active at a time (conflicts with other farm maps)
- **Mods that conflict with other collections** - Included so you can choose between conflicting options when combining collections

**What this means:**
- You can skip optional mods if you have performance concerns
- You can skip optional mods if you're combining both Aesthetic Valley collections and want to avoid conflicts
- You can skip optional mods if you don't need specific compatibility files
- The collection will work without them, but you may miss features 

### Recommendation

**For first-time installs:** Click **OK/Install** when prompted about optional mods. This gives you the complete, intended experience. Just **never** enable more than one farm mod.


---

## Installing SMAPI

SMAPI (Stardew Modding API) is the framework that makes mods work. You need to connect it to your game so mods can load.

### Installing SMAPI Through Vortex

**Easiest method:**
1. SMAPI can be installed as a mod from Nexus Mods
2. Vortex will automatically detect and install it
3. SMAPI comes with the collection and should automatically be configured by Vortex.

### Verifying SMAPI Connection
**Check in Vortex:**
1. Dashboard should show SMAPI as the primary tool
2. You should see a **Launch** button in the top left of Vortex that uses SMAPI

**Check in-game:**
1. Launch the game from Vortex (click the Launch button)
2. The game should start with the SMAPI console window
3. You'll see mod loading messages in the console

**If SMAPI isn't working:**
1. Make sure it's set as Primary Tool in Dashboard
2. Try disabling and reinstalling SMAPI through Vortex
3. Verify your game files (see [Verifying Game Files](#verifying-game-files))
4. Check the [Troubleshooting guide](../Troubleshooting/index.md) for more help

## Connecting SMAPI to Your Store

You need to connect SMAPI to your store launcher if you wish to launch from your store, get achievements, and play co-op. Highly recommended for all users, but technically optional.

{% hint style="info" %}
SMAPI is installed through the collection, so you don't need to install it separately. You just need to configure your store launcher to use it.
{% endhint %}

### Getting the SMAPI Path

First, you need to find the path to `StardewModdingAPI.exe`:

1. In Vortex, go to the **Mods** tab
2. Click **Open** (button at the top)
3. Select **Open Game Folder** (second option)
4. Find `StardewModdingAPI.exe` in the game folder
5. Right-click on `StardewModdingAPI.exe` and select **Copy as path**

You'll use this path in the steps below for your store launcher.

### Steam

**Launch SMAPI by default (recommended):**

1. In the Steam client, right-click on **Stardew Valley** and choose **Properties**
2. Click the textbox under **Launch Options**
3. Paste the path you copied, then add ` %command%` at the end
4. The full text should look like: `"C:\Program Files (x86)\Steam\steamapps\common\Stardew Valley\StardewModdingAPI.exe" %command%`
   - **Important:** Include the quotation marks around the path and then a space and then the `%command%` at the end
5. Click **OK**

From now on, launching Stardew Valley through Steam will run SMAPI with the Steam overlay, achievements, and playtime tracking.

**Reference:** [SMAPI Wiki - Steam Configuration](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Windows#Configure_your_game_client)

### GOG Galaxy

1. Open Notepad and paste: `start "" "YOUR_SMAPI_PATH_HERE"`
   - Replace `YOUR_SMAPI_PATH_HERE` with the path you copied (include the quotes)
   - Example: `start "" "C:\Program Files (x86)\GOG Galaxy\Games\Stardew Valley\StardewModdingAPI.exe"`
2. Click **File > Save As**
3. Navigate to your Stardew Valley game folder
4. Change **Save as type** to **All Files**
5. Name the file `start.bat` and click **Save**
6. In GOG Galaxy, click on **Stardew Valley > settings icon > Manage installation > Configure**
7. Enable the **"Custom executables / arguments"** checkbox
8. Click **Add another executable / arguments**
9. Select `start.bat` and click **Open**
10. Enable the **Default Executable** radio button under the section you just added
11. Click **OK**

From now on, launching Stardew Valley through GOG Galaxy will run SMAPI with playtime tracking.

**Reference:** [SMAPI Wiki - GOG Galaxy Configuration](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Windows#Configure_your_game_client)

### Xbox App

Mods work with the Xbox app, but require a few extra steps:

1. In your game folder (found via Vortex: Mods > Open > Open Game Folder):
   - Rename `Stardew Valley.exe` to `Stardew Valley original.exe`
   - Make a copy of `StardewModdingAPI.exe` and name the copy `Stardew Valley.exe`
2. Launch the game through the Xbox app to play with mods

{% hint style="danger" %}
When the game updates, you'll need to redo these steps (rename the original back and recreate the copy).
{% endhint %}

**Reference:** [SMAPI Wiki - Xbox App Configuration](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Windows#Configure_your_game_client)

---

---

## De-SVE-ing a Collection

If you want to remove Stardew Valley Expanded (SVE) from a collection while keeping other active mods for a new save:

### Step 1: Identify SVE-Related Mods

In Vortex, filter your mods to identify:
- Stardew Valley Expanded (main mod)
- SVE-related compatibility patches
- SVE-specific configuration
- Any mods that depend on SVE

For Stardew Valley VERY Expanded this will include:
- Stardew Valley Expanded
- Stardew Valley Expanded Grampleton Fields
- Immersive Farm 2k Remastered
- Frontier Farm
- Seasonal Cute Characters SVE
- Schedule Viewer - SVE Add-on
- Animated Fish for SVE

For Aesthetic Valley, the fastest way to tell is to disable Stardew Valley Expanded and watch in SMAPI for what can no longer load.

{% hint style="info" %}
Stardew Valley Expanded farm maps will not be usable without Stardew Valley Expanded: Frontier Farm, Grandpa's Farm, Immersive Farm Remastered 2K
{% endhint %}

It is not recommended that you remove Stardew Valley Expanded from an existing save.

---

*Happy farming!*
