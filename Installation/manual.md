# Manual Installation

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* 1.6.15+

---

Manual installation is available for users who cannot use Vortex or prefer direct control over their mod files. This method requires manually applying configuration files and patches.

> **Note:** **Vortex Mod Manager** is strongly recommended for most players because it automatically applies the correct configuration files, manages mod order, provides bundled patches, and handles updates automatically. However, if you are experienced with modding and still prefer to handle installation manually, or are playing on systems without Vortex support, follow this guide.

Before downloading any mods, check the **last update date** for the collection. **Important:** Be cautious about downloading mods released **after** the collection's last update date! They may not be compatible and could cause instability.

---

## Step 1 — Download the Mods

1. Visit the [Stardew Valley VERY Expanded collection page](https://next.nexusmods.com/stardewvalley/collections/tckf0m).  
2. Open the **Mods** tab.  
3. Download each mod manually from its individual Nexus page (mouse-over the mod, click "Read more").  
4. **Extract each mod's zip file** - Zip files cannot be placed directly into the Mods folder. Extract them first, then place the mod folders into your **Stardew Valley/Mods/** directory.
   - **Windows:** Right-click the zip and select "Extract All", or double-click to open and copy the folder out.
   - **Mac/Linux:** Double-click to extract, or use an archive utility.

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

**Extract the files:**

> **Important:** Zip files cannot be placed directly into the Mods folder. You must extract them first. These may also be called "compressed" files.

**Windows:**
- Windows has native zip file support. Right-click the zip file and select **"Extract All"**.
- Extract to a temporary location first, then copy the configuration folders to merge with the matching matching mod folders in your **Mods/** directory.

**Mac:**
- macOS has native zip file support. Double-click the zip file to extract it automatically (or use [The Unarchiver](https://theunarchiver.com/) for other archive formats).
- Use **Option + drag** to merge folders when copying configuration files into your mod folders.

You can modify settings later in-game via **Generic Mod Configuration Menu (GMCM)**.

---

## Step 3 — Apply Required Patches

**For Aesthetic Valley | Witchcore installations:**
- [Grandpa's Tools Patch (Google Drive)](https://drive.google.com/file/d/1F7OcaaxAqz8B8ifIGGSgqWYe9dOMI5wH/view): Replace the relevant files in the Grandpa's Tools mod folder with the patched versions.

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

> **Note:** If installing AVF or AVW, disable in configuration any "Larger Greenhouse" option your chosen farm may have if using the greenhouse included with that collection.

**Manual hair.json fix for Fairycore and Witchcore:**
- Copy the contents of the `hair.json` file in folder `111` into `[FS] Yomi's Golden Princess Hairstyle\Hairs\112`
- Open that file in Notepad++ and change the name at the top from `111` to `112`
- There's a hidden character in the file preventing it from working, so this manual edit is necessary.

---

## Step 5 — Launch with SMAPI

1. Install SMAPI: [Official SMAPI Guide](https://stardewvalleywiki.com/Modding:Installing_SMAPI)  
2. Launch the game using the SMAPI executable.  
3. Check the SMAPI console for errors. If you see missing mods, review the Mods tab on the website to verify all were installed.

---

## Step 6 — Update Notices in SMAPI

Some mods may show an update notification in SMAPI even when no update is actually needed.  
If you wish to suppress the notice, edit the mod's `manifest.json` and set the `"Version"` to match the version shown on Nexus.

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
> 2. Compare your installed mod versions with the collection's mod list
> 3. Download updated mods from their individual Nexus pages
> 4. Replace old mod folders with new ones in your Mods directory
> 5. Re-apply configuration files and patches if needed
>
> **Important:** Always check the collection changelog first to avoid updating to possibly untested versions.

### How do I manage load order?
> Mods load alphabetically by folder name. If you need a specific load order:
> - Rename mod folders (add prefixes like `001_`, `002_`, etc.)
> - Be careful because this can break if mods update and you reinstall them

### What if a mod isn't working?
> 1. Check the SMAPI console for error messages
> 2. Verify the mod folder structure matches the mod's requirements
> 3. Ensure all dependencies are installed
> 4. Check that configuration files were merged correctly
> 5. Verify you're using the correct mod version (matching the collection's last update date)
> 6. Check the mod's individual Nexus page for known issues

### Configuration files keep getting overwritten: how do I preserve custom settings?
> Create backups of your custom configuration files. When updates occur:
> 1. Back up your custom config files before updating
> 2. Download and apply the new configuration package
> 3. Manually merge your custom settings back into the updated configs
>
> Alternatively, use in-game configuration via GMCM, which persists through mod updates.

### I see update notifications in SMAPI: should I update?
> Not necessarily. Only update mods when the collection itself updates. Individual mod updates may break compatibility with other mods in the collection. Check the collection's last update date before updating anything.

### Can I mix manual installation with a mod manager?
> No. Do not run a mod manager and manually install mods to the same game installation. This will cause conflicts and potential corruption.

---

## Common Issues

### Missing mods in SMAPI console
> - Verify all mods were downloaded and placed correctly
> - Check folder structure. Some mods require specific subfolder layouts
> - Ensure mod folders are directly in the Mods directory, not nested incorrectly

### Configuration not applying
> - Verify you extracted and merged config files correctly
> - On Mac, use Option + drag to merge folders properly
> - Check that config files are in the correct mod folders


### Incorrect folder structure
> Some mods require specific folder layouts. If SMAPI reports structure issues:
> - Check the mod's Nexus page for installation instructions
> - Ensure you extracted the mod correctly (not double-nested folders)
> - Verify all required files are present in the mod folder
> - Verify all mods have a parent folder. There should be no loose mod assets in the Mods folder.

### SMAPI asking for update to already updated mod.
> Edit the mod's `manifest.json` file and update the `"Version"` field to match the version shown on Nexus. This suppresses update notifications without actually updating the mod.

---

## See Also

- [Mod Managers Overview](index.md) - To compare with mod manager options (Vortex recommended)
- [Troubleshooting & FAQ](../../Guides/troubleshooting.md) - For installation and gameplay issues
- [Updating Collections](../../Guides/updating-collections.md) - How to update manually installed collections
- [Combining Collections](../../Collections/combining-collections.md) - If using multiple collections

