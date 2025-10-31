# Personalization & Custom Configurations

> 📂 Docs / Guides / Personalization & Custom Configurations

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* **1.6.15+**

This guide covers how to personalize your Stardew Valley experience with custom configurations and settings that persist through updates.

---

## Overview

Personalization allows you to customize your game experience while maintaining compatibility with collection updates. This includes:

- Custom mod configurations (settings, keybinds, etc.)
- Personal mod additions 
- UI and visual preferences
- Gameplay tweaks and adjustments

---

## Personal Customizations and Patches

Use the [Add Custom Mod Button](https://www.nexusmods.com/site/mods/863) Vortex extension to create persistent customizations and patches that always load after your main mods:

### Creating Personal Customizations

**Step 1: Configure Your Settings**
1. Configure mods as desired in-game (GMCM recommended)
2. Test your settings to ensure they work as expected

**Step 2: Create Custom Config Mod**
1. In Vortex, click Create new mod via the Add Custom Mod Button
2. Name it something like "My Configs" or "Personal Settings"

**Step 3: Copy Configuration Files**
1. Navigate to your Stardew Valley Mods folder
2. Find the mods you've customized
3. Copy the entire mod folders into your "My Configs" mod folder
4. Delete everything inside except your config files (usually `config.json`)

**Step 4: Set Load Order**
1. In Vortex → Mods → Manage Rules
2. Set "My Configs" to load after the mods it's overriding
3. Click Deploy

### Creating Patches and Local Mods

The same process can be used to create persistent patches and minor local mods:

1. Create a custom mod using the Add Custom Mod Button
2. Add your custom files, patches, or other mods
3. Set the load order to ensure your changes take priority
4. Your customizations will persist through updates

This method ensures your personal settings and mods are reapplied automatically, even after collection updates.

---

## Adding Additional Mods

### Installing Mods from Nexus

There are two ways to add mods from Nexus Mods:

### Method 1: Mod Manager Button (Recommended)
1. Go to the mod's files page on Nexus Mods
2. Click the "Mod Manager" button to download directly to Vortex
3. Follow the installation prompts in Vortex

### Method 2: Manual Download
1. Click the "Manual" button on the mod's files page
2. Download the ZIP file to your computer
3. Go to Vortex Mods page and drag the ZIP file onto the drop zone
4. Follow the installation prompts

### Creating a Private Collection
If you add mods, it's recommended to create a private collection that contains only the mods you've added. This way you can easily reinstall or redeploy them to a new profile after updating:

1. Create an empty collection in Vortex
2. Right-click "Add to Collection" on each mod in the Mods page
3. Upload to Nexus' server from the Workshop section of the Collection tab and keep it updated for future downloads
4. Share the private link with friends

Note: You can share your collection with friends using the private link without making it public. Keeping personal collections private is recommended.

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
- Use "Binary Patch" for minor content modifications (but you cannot use both methods simultaneously)

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

### Before Updates

1. Back up your save files - It's recommended to create a backup of your Stardew Valley saves before updating. See the [Stardew Valley Wiki Saves page](https://www.stardewvalleywiki.com/Saves) for detailed instructions on locating and backing up your save files
2. Back up your custom configs (they're already protected if using the Custom Config Mod method)

### After Updates
1. Check that all mods are enabled in Vortex
2. Verify your custom settings are still active
3. Test before continuing your save

### Lost Settings
- Restore from backup if you have one
- Reconfigure manually using GMCM or text editors
- Check if official folder names changed and updated your customizations to match

---

## Troubleshooting Personalizations

### Settings Not Applying
- Check load order - custom configs must load after the mods they're overriding. This is done with "Manage Rules".
- Verify file paths - ensure config files are placed in a folder structure that matches the mod they alter.

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
