# Manual Installation
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

{% hint style="warning" %}
Manual installation is not recommended. You will miss bundled features, binary patches, and more.
{% endhint %}

Use a supported manager with collection support when you can. JennaJuffuffles' collections include fixes and adjustments you will not benefit from by just treating them like a reference list. However, this page is kept for a manual install when you cannot use a manager.

## Step 1: Download the Mods

{% hint style="warning" %}
Before downloading any mods, check the collection's last update date. Mods released after that date may not be compatible and can cause instability.
{% endhint %}

1. Visit [Jenna Juffuffles' collections](https://www.nexusmods.com/profile/JennaJuffuffles/collections) page and select the collection you want to install.  
2. Open the **Mods** tab.  
3. Download each mod manually from its individual Nexus page (mouse-over the mod, click "Read more").  
4. Extract each mod's zip file. Zip files cannot be placed directly into the Mods folder. Extract them first, then place the mod folders into your **Stardew Valley/Mods/** directory.
   - **Windows:** Right-click the zip and select "Extract All", or double-click to open and copy the folder out.
   - **Mac/Linux:** Double-click to extract, or use an archive utility.

{% hint style="warning" %}   
Copy the complete parent folder with all its subfolders into Mods/. Do not copy individual files. The entire mod folder structure must be preserved.
{% endhint %}   

---

## Step 2: Apply Configuration Files

Download the official configuration package that matches the collection you are using:  
[Configuration Files on Nexus](https://www.nexusmods.com/stardewvalley/mods/20870)  

**Extract the files:**

{% hint style="danger" %}
Zip files cannot be placed directly into the Mods folder. You must extract them first. These may also be called "compressed" files.
{% endhint %}

**Windows:**
- Windows has native zip file support. Right-click the zip file and select **"Extract All"**.
- Extract to a temporary location first, then copy the files and folders inside the extracted configuration folders to merge with the matching mod folders in your **Mods/** directory.
- **Important:** You must copy the files inside the configuration folders, not place the configuration folder itself in Mods/. Open the extracted configuration folder and copy its contents into the corresponding mod folder.

**Mac:**
- macOS has native zip file support. Double-click the zip file to extract it automatically (or use [The Unarchiver](https://theunarchiver.com/) for other archive formats).
- Use **Option + drag** to merge folders when copying configuration files into your mod folders.

**Linux:**
- Extract the zip from your file manager (**Extract Here**) or with `unzip`.
- Copy the files and folders inside the extracted configuration folder into the matching mod folder in **Mods/**, and merge when asked.
- Do not place the configuration folder itself in Mods/.

You can modify settings later in-game via **Generic Mod Configuration Menu (GMCM)**.

{% hint style="info" %}
If installing AVF or AVW along with svVe, disable in configuration any "Larger Greenhouse" option for Frontier Farm may have if using the greenhouse included with that collection.
{% endhint %}

---

## Step 3: Apply Required Patches

**For Stardew Valley VERY Expanded:**
- Merge the Various ore-producing patch with the [Additional Farm Caves](https://www.nexusmods.com/stardewvalley/mods/14109?tab=files) parent folder. That overwrite replaces the existing Farm Type Management module.

**For Aesthetic Valley | Witchcore installations:**
- [Grandpa's Tools Patch (Unofficial)](https://www.nexusmods.com/stardewvalley/mods/40320): Replace the relevant files in the Grandpa's Tools mod folder with the patched versions.

**For Witchcore installations only:**
- [Aurora Vineyard Refurbished Patch](https://drive.google.com/file/d/1ekcuFIlk5gEZry8_Gabh9204065LE22Y/view)  
- [Way Back Pelican Town Fix](https://www.nexusmods.com/stardewvalley/mods/7332?tab=posts): Follow the instructions in the first post.

---

## Step 4: Aesthetic Valley Compatibility Files

If installing **Fairycore** or **Witchcore**, make sure to also download and install the appropriate compatibility files for the UI mod included in that collection.

**For Fairycore installations:**
- **Overgrown Flowery Interface**: Download compatibility files from [Overgrown Flowery Interface optional files](https://www.nexusmods.com/stardewvalley/mods/6166?tab=files) for:
  - World Navigator
  - Fashion Sense
  - Generic Mod Config Menu
  - Never Ending Adventures & Circle of Thorns (rename folder to match Sword & Sorcery)

**For Witchcore installations:**
- **Earthy Interface**: Download compatibility files from [DaisyNiko's Earthy Interface optional files](https://www.nexusmods.com/stardewvalley/mods/13658?tab=files) for:
  - Generic Mod Config Menu
  - World Navigator

### Fix for [FS] Yomi's Golden Princess Hairstyle 112 hairstyle not loading

1. Open folder `Hairs\111`.
2. Copy the file **`hair.json`**.
3. Go to **Hairs\112**.
4. Paste the file there and overwrite the existing **`hair.json`**.
5. Open the pasted **`hair.json`** in a text editor.
6. At the very top of the file, change `111` to `112`.
7. Save the file.

**Why this works:** The original `hair.json` in folder `112` contains a hidden character that stops the game from loading it. Copying the file from the working `111` and changing the number removes that problem.

---

## Step 5: Launch with SMAPI

1. Install SMAPI from https://smapi.io/
2. Launch the game using the SMAPI executable.  
3. Check the SMAPI console for errors. If you see missing mods, review the Mods tab on the website to verify all were installed.

---

## Step 6: Update Notices in SMAPI

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
> 4. Delete old mod folders, then add the new ones to your Mods directory
> 5. Re-apply configuration files and patches as needed. Sometimes you can keep your old configurations, though not always!

### How do I manage load order?
If you need a specific load order:
> 1. **Add a false requirement to the manifest** (recommended): Edit the mod's `manifest.json` and add a dependency on another mod to control load order. This method persists through mod updates.
> 2. **Rename mod folders** (alternative): > Mods load alphabetically by folder name. Add prefixes like `001_`, `002_`, etc. to folder names. 

### What if a mod isn't working?
> 1. Check [Your SMAPI Log](../Troubleshooting/your-smapi-log.md) for error messages
> 2. Verify the mod folder structure matches the mod's requirements
> 3. Ensure all components (subfolders) of the mod fully extracted
> 4. Ensure all dependencies are installed
> 5. Check that configuration files were merged correctly
> 6. Verify you're using the correct mod version (matching the collection's last update date)
> 7. Check the mod's individual Nexus page for known issues

### I see update notifications in SMAPI: should I update?
> Not necessarily. Only update mods when the collection itself updates. Individual mod updates may break compatibility with other mods in the collection. Check the collection's last update date before updating a mod.

### Can I mix manual installation with a mod manager?
> This may cause conflicts and potential corruption.

---

## Common Issues

### Missing mods in SMAPI console
> - Verify all mods were downloaded, extracted fully, and placed correctly
> - Ensure mod folders are directly in the Mods directory, not nested incorrectly
> - Check for red errors in SMAPI by uploading your log to [smapi.io/log](https://smapi.io/log) and check for red loading errors.

### Configuration not applying
> Open the extracted configuration folder and copy its contents into the corresponding mod folder in Mods. 
> - Verify you extracted and merged the mod folders containing config files correctly
> - Check that config files are in the correct mod folders

---

## Related

- [Install with Vortex](vortex.md)
- [Your SMAPI Log](../Troubleshooting/your-smapi-log.md)
