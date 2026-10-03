# Install with Vortex
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

Vortex is the recommended way to install these collections on Windows. Multiple collections may be installed on one profile.

---

Using a different manager? See [Install with Stardrop](stardrop.md) or [Install with Amethyst](amethyst.md).

Already playing a save you want to keep? Read [Installing to an Existing Save](installing-to-an-existing-save.md) before you install.

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

{% hint style="info" %}
If Stardew Valley and Vortex are not both installed on drive `C:\` as recommended, enable **Use Symbolic Links** now: **Settings** (gear icon) > **Mods** > **Use Symbolic Links** > **Apply**. 
{% endhint %}

---

## Clearing Your Mod Folder

Before installing a collection, you need a clean slate. Any existing mods or leftover files can cause conflicts.

1. If you have other Stardew Valley mods managed in Vortex, disable them.
2. In the **Mods** tab, click **Open > Game Mods Folder**
3. **Remove everything** from this folder (files and subfolders)
4. Close the folder window

{% hint style="warning" %}
Old, unmanaged mod files can conflict with collection mods! This can cause crashes, conflicts, and other issues. Starting fresh ensures everything works correctly.
{% endhint %}

---
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

## Installation Process

Follow these steps to install a collection. Browse available [Jenna Juffuffles' collections](https://www.nexusmods.com/profile/JennaJuffuffles/collections).

### Step-by-Step Installation

1. Ensure Vortex is open
2. Click **Add Collection** on the collection page
3. Pop-up in browser will ask you to use a Mod Manager, click **Continue**
4. Vortex will display the collection, click **Install Now**
   - **For Premium users:** Vortex handles everything automatically
   - **For Free users:** You'll need to click buttons to download the mods from the pages Vortex opens for you. All mods are hosted on Nexus.
5. When Vortex prompts about optional mods, follow the on-screen instructions for each one.

### Installing Multiple Collections

Install the first collection as normal, then add the next from its Nexus page and choose **Current profile** on the first pop-up. "Current profile" is a Vortex choice.

**New profile (start here)**

* [Stardew Valley VERY Expanded](https://www.nexusmods.com/games/stardewvalley/collections/tckf0m): Create a **new profile**. This is the default.

**Add to your SVVE profile**

* [Oops! All Portraits: Nyapu](https://www.nexusmods.com/games/stardewvalley/collections/falitk)
* [Aesthetic Valley Fairycore](https://next.nexusmods.com/stardewvalley/collections/tjvl0j) or [Aesthetic Valley Witchcore](https://next.nexusmods.com/stardewvalley/collections/g14kxi): Pick **one**.

**Add to any working profile**

* [Controller Support](https://www.nexusmods.com/games/stardewvalley/collections/crx9cn)
* [Aesthetic Valley Fairycore Extra Textures](https://www.nexusmods.com/games/stardewvalley/collections/i8ulwo/)
* [Aesthetic Valley Witchcore Extra Textures](https://www.nexusmods.com/games/stardewvalley/collections/ufo0fl/)

{% hint style="danger" %}
**Aesthetic Valley Fairycore** and **Aesthetic Valley Witchcore** are mutually exclusive. Install **one** per profile, not both.
{% endhint %}

Only enable **one** farm map at a time. If Vortex prompts you during install or update, finish [Vortex Notifications and Solutions](../Troubleshooting/vortex-notifications.md#when-vortex-asks-you-to-set-rules) before you play.

---

## Optional Mods

Collections may include optional mods. Install the required mods. When Vortex prompts about optional mods during installation, follow the on-screen instructions for each one.

---

## Installing SMAPI

SMAPI (Stardew Modding API) is the framework that makes mods work. You need to connect it to your game so mods can load.

### Installing SMAPI Through Vortex

**Easiest method:**
1. SMAPI can be installed as a mod from Nexus Mods
2. Vortex will automatically detect and install it
3. SMAPI comes with the collection and should automatically be configured by Vortex.

### Verifying SMAPI Connection

After setup, launch the game the first time from within Vortex.

**Check in Vortex:**
1. Dashboard should show SMAPI as the primary tool
2. You should see a **Launch** button in the top left of Vortex that uses SMAPI

**Check in-game:**
1. Click **Launch** in Vortex
2. The game should start with the SMAPI console window
3. You'll see mod loading messages in the console

**If SMAPI isn't working:**
1. Make sure it's set as Primary Tool in Dashboard
2. Try disabling and reinstalling SMAPI through Vortex
3. Verify your game files. See [Reset Your Content Files](../Troubleshooting/reset-your-content-files.md).
4. Check [Launch Problems](../Troubleshooting/launch-problems.md) if it still will not start

## Connecting SMAPI to Your Store

You need to connect SMAPI to your store launcher if you wish to launch from your store, get achievements, and play co-op. Highly recommended for all users, though technically optional.

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
- Frontier Farm
- Seasonal Cute Characters SVE
- Animated Fish for SVE

For Aesthetic Valley, the fastest way to tell is to disable Stardew Valley Expanded and watch in SMAPI for what can no longer load.

{% hint style="info" %}
Stardew Valley Expanded farm maps will not be usable without Stardew Valley Expanded: Frontier Farm, Grandpa's Farm, Immersive Farm Remastered 2K
{% endhint %}

{% hint style="danger" %}
It is not recommended that you add or remove Stardew Valley Expanded from an existing save.
{% endhint %}

## Related

- [Installing to an Existing Save](installing-to-an-existing-save.md)
- [Update with Vortex](../Update/vortex.md)
- [Vortex Notifications and Solutions](../Troubleshooting/vortex-notifications.md)
- [Manual Installation](manual-installation.md) 
