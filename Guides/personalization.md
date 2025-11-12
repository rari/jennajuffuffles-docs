# Personalization & Custom Configurations

> 📂 Docs / Guides / Personalization & Custom Configurations

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* **1.6.15+**

Want to make your Stardew Valley experience truly your own? This guide will show you how to customize your game with your own settings, additional mods, and personal tweaks - all while keeping your customizations safe through collection updates!

---

## Overview

Personalization allows you to customize your game experience while maintaining compatibility with collection updates. You can:

* Customize mod configurations (settings, keybinds, etc.)
* Add your own favorite mods 
* Adjust UI and visual preferences
* Make gameplay tweaks and adjustments

The best part? When done correctly, your personalizations will persist even when the collection updates!

---

## Backing Up Configuration Files

Before updating, it's important to back up your configuration files. This ensures you can restore your settings if something goes wrong during updates or modifications.

### Using Sync Mod Configurations

Vortex provides a built-in feature to backup and restore your mod configurations:

> 1. In Vortex, locate the **"Sync Mod Configurations"** button
> 2. Click the button to create a backup of your current configuration files
> 3. This will save your current configurations prevent them from being lost 

**Important Note:** The Sync Mod Configurations feature may occasionally attempt to back up `smapi-internal` in error. This is a known issue that can be easily fixed.

### Fixing smapi-internal Backup Error

If the Sync Mod Configurations feature incorrectly backs up `smapi-internal`:

> 1. Right-click on Stardew Valley Configurations mod entry created by Vortex
> 2. Select **Open in File Manager** to access the mod folder
> 3. Locate the `smapi-internal` folder within the configuration mod
> 4. Cut the `smapi-internal` folder from the configuration mod location
> 5. Navigate to your main Stardew Valley folder (where the game is installed)
> 6. Paste the `smapi-internal` folder back into its proper location

> **Please report to Vortex staff if this happens** - this issue needs more visibility to be properly addressed.

---

## Personal Customizations and Patches

Creating custom patches allows you to modify mod files (configurations, content patches, translations, etc.) while keeping your changes safe through collection updates. Patches load after the original mods, ensuring your customizations take priority.

### Creating Custom Patches in Vortex

> 1. **Create your patch folder structure** - The folder structure must exactly match what is in your mods folder. For example, if you are patching `ModName/[CP] ModName/content.json`, that is the folder structure you would need to create.
> 2. **Add your files** - Place your modified files in the appropriate folders. A patch may contain multiple top level folders if you do not include manifests.
> 3. **Add to your mod manager** - Compress the top level folder as a ZIP file and add it as if it was a mod or add the folder via the [Add Custom Mod Button](https://www.nexusmods.com/site/mods/863)  button add-on in Vortex
> 4. **Set load order** - In Vortex → Mods → Manage Rules, set your patch to load **AFTER** the mod it's patching.
> 5. Click **Deploy** to apply your changes.

If this is done in Vortex, it is recommended you include this custom mod in your private collection.

### Creating Custom Patches in Other Mod Managers

If you're not using Vortex, you can create patches as if they were mods (without a manifest) and add them into your mod manager normally:

> 1. **Create your patch folder structure** - The folder structure must exactly match what is in your mods folder. For example, if you are patching `ModName/[CP] ModName/content.json`, that is the folder structure you would need to create.
> 2. **Add your files** - Place your modified files in the appropriate folders.
> 3. **Add to your mod manager** - Add the patch folder to your mod manager as you would any other mod. Since patches don't require manifests, they can be added directly.
> 4. **Ensure proper load order** - Configure your mod manager's load order settings to ensure the patch loads **AFTER** the mod it's patching.

Your customizations will persist this way and won't be overwritten during collection updates.

---

## Adding Additional Mods

### Installing Mods from Nexus

There are two ways to add mods from Nexus Mods:

### Method 1: Mod Manager Button (Recommended)
1. Go to the mod's files page on Nexus Mods
2. Click the "Mod Manager" button to download directly to your mod manager
3. Ensure you also install any requirements not already present

### Method 2: Manual Download
1. Click the "Manual" button on the mod's files page
2. Download the ZIP file to your computer
3. Import the mod into your mod manager (in Vortex, go to the Mods page and drag the ZIP file onto the drop zone)
4. Follow the installation prompts

> **Important:** Do not extract mods directly into your mods folder while using a mod manager. Always use your mod manager to install mods.

### Creating a Private Collection

If you add mods, it's recommended to create a private collection that contains only the mods you've added. This way you can easily reinstall or redeploy them to a new profile after updating, and you'll never lose track of your additions!

#### Method 1: Create from Profile (Recommended for Updates)

This method is especially useful when updating collections, as it automatically captures all your additional mods:

1. In Vortex, go to the Mods tab and filter for active collection name(s) (e.g., "Stardew Valley VERY Expanded") on your current profile.
2. Disable the collection and when prompted, click to include recommended mods.
3. Go to **Collections > Create a Collection > From Profile**. This creates a DRAFT of your private collection containing your additional mods. You don't need to publish it - it's just for your use.
4. (Optional) Upload to Nexus' server from the Workshop section of the Collection tab and keep it updated for future downloads. Publish only to share the private link with friends.

#### Method 2: Create Empty Collection

For creating a collection from scratch:

1. Create an empty collection in Vortex
2. Right-click "Add to Collection" on each mod in the Mods page
3. (Optional) Upload to Nexus' server from the Workshop section of the Collection tab and keep it updated for future downloads. Publish only to share the private link with friends.

> **Note:** You can share your collection with friends using the private link without making it public. Keeping personal and friends-only collections private is recommended.

For detailed instructions on creating collections, see our [How to Create A Collection](collection-creation.md) guide.

### Modifying Mods

Some mods you add may require restructuring to work within Vortex:

### Making Structural Changes
1. Right-click on the mod in Vortex
2. Select "Open in File Manager" to access the Staging folder
3. Adjust the mod's folder structure as needed
4. Do not modify the top-level folder (with the numeric string)
5. Click "Deploy" in Vortex to apply your changes

### Collection Settings for Modified Mods
- Set to "Exact" and "Replicate" in your private collection if you modify a mod's folder structure
- Use "Binary Patch" for minor content modifications (but you cannot use both this and Replicate methods simultaneously)

### Best Practices
- Read mod pages carefully for compatibility notes 
- Test one mod at a time when adding multiple mods
- Keep backups of working configurations before updating
- Document your setup for easy recreation
- Test thoroughly after making any modifications

---

## In-Game Configuration

### Generic Mod Config Menu (GMCM)

Most mods support the Generic Mod Config Menu for easy in-game configuration:

1. Access GMCM through the game's settings menu (⚙️)
2. Browse available mods and their settings
3. Make changes and they'll be saved automatically
4. Test changes before finalizing your setup

### Manual Configuration

Some mods require manual file editing:

1. Locate the mod's config file (usually `config.json`)
2. Edit with a text editor (Notepad++ recommended)
3. Follow the mod's documentation for proper syntax
4. Backup using the method above
5. Delete and reload Stardew to create a fresh config if you need to start over

---

## Maintaining Personalizations

Don't worry - if you've followed the steps above, your customizations should survive updates! Here's what to do:

### Before Updates

1. **Back up your save files** - Your saves are precious! It's recommended to create a backup before updating. See the [Stardew Valley Wiki Saves page](https://www.stardewvalleywiki.com/Saves) for detailed instructions on locating and backing up your save files.
2. **Your custom configs are already protected** - If you're using the Custom Config Mod method described above, your settings are already safe and will persist through updates!

### After Updates

1. Check that all mods are enabled in Vortex
2. Verify your custom settings are still active
3. Test your game before continuing your save

If you encounter any issues, see our [Troubleshooting Guide](troubleshooting.md) for help.

## Troubleshooting Personalizations

### Settings Not Applying

If your custom settings aren't working:
- **Check load order** - Custom configs must load after the mods they're overriding. This is done with "Manage Rules" in Vortex. Make sure your custom config mod loads after the original mod.
- **Verify file paths** - Ensure config files are placed in a folder structure that matches the mod they alter. The folder names should match exactly.

### Lost Settings?

If something goes wrong after an update:
- Restore from backup if you have one
- Reconfigure manually using GMCM or text editors
- Check if official folder names changed and update your customizations to match

---

## Tips & Best Practices

### Organization
- Use descriptive names for your custom mods (Config for X Mod, My Configs, Patches, etc)
- Group related settings together
- Keep documentation of your changes

### Compatibility
- Test with collection updates before committing to changes
- Read mod compatibility notes carefully
- Avoid conflicting mods when possible

### Backup Strategy
- Regular backups of your Mods folder
- Version control for your custom configs
- Documentation of your setup process
