---
title: Manual Installation Guide
description: Install Stardew Valley mod collections manually without Vortex. Learn how to install mods directly, set up files, and configure collections for advanced users.
keywords: [manual installation, manual mod installation, without Vortex, direct installation, manual setup, configuration files, advanced installation]
tags: [installation, manual, advanced]
---

# Manual Installation

*Last updated:* 2026-01-19  
*Applies to Stardew Valley:* 1.6.15+

{% hint style="info" %}
**Vortex Mod Manager** is strongly recommended for most players because it automatically applies the correct configuration files, manages mod order, provides bundled patches, and handles updates automatically. However, if you are experienced with modding and still prefer to handle installation manually, or are playing on systems without Vortex support, follow this guide.
{% endhint %}

Manual installation is available for users who cannot use Vortex or prefer direct control over their mod files. This method requires manually applying configuration files and patches. This guide walks you through the complete manual installation process step by step.

---

Before downloading any mods, check the **last update date** for the collection. **Important:** Be cautious about downloading mods released **after** the collection's last update date! They may not be compatible and could cause instability.

---

## Step 1 — Download the Mods

1. Visit [Jenna Juffuffles' collections](https://www.nexusmods.com/profile/JennaJuffuffles/collections) page and select the collection you want to install.  
2. Open the **Mods** tab.  
3. Download each mod manually from its individual Nexus page (mouse-over the mod, click "Read more").  
4. **Extract each mod's zip file** - Zip files cannot be placed directly into the Mods folder. Extract them first, then place the mod folders into your **Stardew Valley/Mods/** directory.
   - **Windows:** Right-click the zip and select "Extract All", or double-click to open and copy the folder out.
   - **Mac/Linux:** Double-click to extract, or use an archive utility.
   - **Important:** After extracting, look inside the extracted folder. The actual mod folder (usually named like `[CP] ModName` or `ModName`) should be placed in Mods/, not the extraction folder itself, named for the zip file. 
   - **Complete mod structure:** Mods should be contained in a top parent folder, but may contain multiple subfolders. Copy the complete parent folder with all its subfolders into Mods/. Do not copy individual files—the entire mod folder structure must be preserved.

> On Windows: `%appdata%/StardewValley/Mods`  
> On Mac: `~/.config/StardewValley/Mods`  
> On Linux: `~/.local/share/StardewValley/Mods`

---

## Step 2 — Apply Configuration Files

Download the official configuration package that matches the collection you are using:  
[Configuration Files on Nexus](https://www.nexusmods.com/stardewvalley/mods/20870)  

**Extract the files:**

{% hint style="danger" %}
Zip files cannot be placed directly into the Mods folder. You must extract them first. These may also be called "compressed" files.
{% endhint %}

**Windows:**
- Windows has native zip file support. Right-click the zip file and select **"Extract All"**.
- Extract to a temporary location first, then **copy the files and folders inside** the extracted configuration folders to merge with the matching mod folders in your **Mods/** directory.
- **Important:** You must copy the files inside the configuration folders, not place the configuration folder itself in Mods/. Open the extracted configuration folder and copy its contents into the corresponding mod folder.

**Mac:**
- macOS has native zip file support. Double-click the zip file to extract it automatically (or use [The Unarchiver](https://theunarchiver.com/) for other archive formats).
- Use **Option + drag** to merge folders when copying configuration files into your mod folders.

You can modify settings later in-game via **Generic Mod Configuration Menu (GMCM)**.

{% hint style="info" %}
If installing AVF or AVW, disable in configuration any "Larger Greenhouse" option your chosen farm may have if using the greenhouse included with that collection.
{% endhint %}

---

## Step 3 — Apply Required Patches

**For Aesthetic Valley | Witchcore installations:**
- [Grandpa's Tools Patch (Unofficial)](https://www.nexusmods.com/stardewvalley/mods/40320): Replace the relevant files in the Grandpa's Tools mod folder with the patched versions.

**For Witchcore installations only:**
- [Aurora Vineyard Refurbished Patch](https://drive.google.com/file/d/1ekcuFIlk5gEZry8_Gabh9204065LE22Y/view)  
- [Way Back Pelican Town Fix](https://www.nexusmods.com/stardewvalley/mods/7332?tab=posts): Follow the instructions in the first post.

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

### Fix for [FS] Yomi's Golden Princess Hairstyle 112 hairstyle not loading

1. Open folder `Hairs\111`.
2. Copy the file **`hair.json`**.
3. Go to **Hairs\112**.
4. Paste the file there and **overwrite** the existing **`hair.json`**.
5. Open the pasted **`hair.json`** in a text editor.
6. At the very top of the file, change `111` → `112`.
7. Save the file.

**Why this works:** The original `hair.json` in folder `112` contains a hidden character that stops the game from loading it. Copying the file from the working `111` and changing the number removes that problem.

---

## Step 5 — Launch with SMAPI

1. Install SMAPI from https://smapi.io/
2. Launch the game using the SMAPI executable.  
3. Check the SMAPI console for errors. If you see missing mods, review the Mods tab on the website to verify all were installed.

---

## Step 6 — Update Notices in SMAPI

Some mods may show an update notification in SMAPI even when no update is actually needed. If you wish to suppress a notice, edit the mod's `manifest.json` and set the `"Version"` to match the version shown on Nexus.

{% hint style="info" %}
When should you update? See the FAQ section below: [I see update notifications in SMAPI: should I update?](#i-see-update-notifications-in-smapi-should-i-update)
{% endhint %}

---

## FAQ

### What are the main limitations?
> - **No automatic updates**: You must manually download and update each mod
> - **No automatic configuration**: You must manually apply config files from the configuration package
> - **Load order management**: You must manually manage mod load order (mod folder names affect loading or false requirements in manifest)
> - **Patch management**: You must manually apply required patches when collections update
> - **Error detection**: Harder to identify missing or incorrectly installed mods
> - **Collection updates**: Requires re-downloading and reinstalling mods when the collection updates

### How do I update mods manually?
> 1. Check the collection's last update date on Nexus
> 2. Compare your mod versions requesting update with the collection's change log
> 3. Download updated mods from their individual Nexus pages
> 4. Delete old mod folders, then add the new ones to your Mods directory (but check for config files before deleting old mod folders!)
> 5. Re-apply configuration files and patches if needed

### How do I manage load order?
If you need a specific load order:
> 1. **Add a false requirement to the manifest** (recommended): Edit the mod's `manifest.json` and add a dependency on another mod to control load order. This method persists through mod updates.
> 2. **Rename mod folders** (alternative): > Mods load alphabetically by folder name. Add prefixes like `001_`, `002_`, etc. to folder names. 

### What if a mod isn't working?
> 1. Check the [SMAPI console](../Troubleshooting/your-smapi-log.md) for error messages
> 2. Verify the mod folder structure matches the mod's requirements
> 3. Ensure all components (subfolders) of the mod fully extracted
> 4. Ensure all dependencies are installed
> 5. Check that configuration files were merged correctly
> 6. Verify you're using the correct mod version (matching the collection's last update date)
> 7. Check the mod's individual Nexus page for known issues

### I see update notifications in SMAPI: should I update?
> Not necessarily. Only update mods when the collection itself updates. Individual mod updates may break compatibility with other mods in the collection. Check the collection's last update date before updating anything.

### Can I mix manual installation with a mod manager?
> No. Do not run a mod manager and manually install mods to the same game installation. This will cause conflicts and potential corruption.

---

## Common Issues

### Missing mods in SMAPI console
> - Verify all mods were downloaded, extracted fully, and placed correctly
> - Ensure mod folders are directly in the Mods directory, not nested incorrectly

### Configuration not applying
> - **Most common issue:** Verify you copied the files inside the extracted configuration folder, not the folder itself. Open the extracted configuration folder and copy its contents into the corresponding mod folder in Mods/.
> - Verify you extracted and merged config files correctly
> - On Mac, use Option + drag to merge folders properly
> - Check that config files are in the correct mod folders


---

## See Also

- [New Player Install Instructions](index.md) - Recommended installation method
- [Troubleshooting & FAQ](../Troubleshooting/index.md) - For installation and gameplay issues
- [Installing Multiple Collections](multiple-collections.md) - If using multiple collections
