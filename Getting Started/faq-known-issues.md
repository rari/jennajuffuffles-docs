# FAQ & Known Issues

> 📂 Docs / Getting Started / FAQ & Known Issues

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* **1.6.15+**

This page addresses general questions and issues that apply across all collections. For Stardew Valley VERY Expanded (SVVE) specific gameplay questions and troubleshooting, see the [SVVE FAQ](Collections/Stardew%20Valley%20VERY%20Expanded/faq.md).

---

## Getting Started FAQs

**Do I need the optional mods?**
> Yes! While some mods are marked as "optional" to make it easier when combining collections, you should install them when using a single collection. These optional mods include:
> - Essential interface improvements 
> - Map enhancements that improve the visual experience
> - Additional content that enhances gameplay
> - Expansions that have been carefully curated for quality
> - Compatibility files for combining collections (only needed when stacking multiple collections)
> 
> The optional designation exists mainly to help with collection stacking (combining multiple collections). When using just one collection, these mods are designed to be part of the intended experience.

**Should I update individual mods myself?**
> No. Always wait for the collection to be updated instead of updating individual mods yourself. The collection curator tests all mod versions together to ensure compatibility. Updating mods individually can cause version conflicts, breaking changes, missing compatibility patches, and unstable gameplay. When a collection update is released, it includes tested versions of all mods that work together.

**Can I combine your collections?**
> Yes! Any Aesthetic Valley collection (Fairycore, Witchcore, or future Aesthetic Valley collections) is designed to work alongside Stardew Valley VERY Expanded (SVVE). You can install them into the same Vortex profile.
> 
> For detailed instructions on how to combine collections, including which optional mods to install and how to manage conflicts, see our [Combining Collections](Collections/combining-collections.md) guide.

**First-time players**
> It's absolutely fine to start with SVVE even if you're new to Stardew Valley! The collection is designed to enhance the game while preserving the vanilla feel. However, keep in mind that SVVE is quite large with many new areas, NPCs, and content.
> 
> **Recommendation:** Playing vanilla Stardew Valley first will help you appreciate the additions SVVE brings, but it's not required. If you're eager to dive in with the collection, go for it - just be prepared for a lot more content to explore!

**Co-op**
> All players in a multiplayer game must have matching mods and configurations for everything to work correctly. This means:
> - All players need the same collection(s) installed
> - All players need the same mod versions
> - All players need matching configurations (especially for mods that affect gameplay)
> 
> Consider using a multiplayer manager or keeping careful documentation of your mod setup so everyone can stay in sync. Version mismatches can cause desyncs, crashes, or missing content.

**Where to download**
> Always download from **Nexus Mods** - this is the official source for these collections. The collections are only updated and maintained through Nexus.
> 
> **Nexus Premium** enables one-click installation through Vortex, making setup much easier. If you're installing manually, you can still use Nexus for free, though it takes more time.
> 
> Avoid unauthorized mirrors or repackaged versions, as these may be outdated, incomplete, or contain malware. Sticking to Nexus Mods ensures you get the latest, tested, and safe version.

---

## Gameplay FAQs

For SVVE-specific gameplay questions including Community Center cutscenes, Rusty/Sewer Key changes, minecart blocking the mine entrance, duplicated NPCs, East Scarp festival attendance, crafting issues, and performance problems, see the [SVVE FAQ](Collections/Stardew%20Valley%20VERY%20Expanded/faq.md).

**Can't exit house / corrupted farm map**
> If you find yourself unable to exit your house or see a corrupted farm map (missing textures, black areas, or errors), this usually means your farm map mod is disabled or failed to load properly.
> 
> To fix this:
> 1. Open your mod manager 
> 2. Find your farm map mod 
> 3. Make sure it's **Enabled** 
> 4. Check that no other farm map mods are enabled - only one farm map should be active at a time
> 5. Click **Deploy** to apply the changes
> 6. Restart the game and load your save
> 
> **Important:** Farm maps cannot be switched mid-save without special tools. If you want to change your farm map, you'll need to start a new save file, or use a tool like [Easy Farm Switcher](https://www.nexusmods.com/stardewvalley/mods/16873) which can handle the transition (though this should be done carefully and with backups).

---

## Setup & Customization FAQs

**Can I add more mods?**
> Yes! These collections are designed as solid bases that you can build upon. However, there are some important things to keep in mind:
> 
> - **Test additions individually** - Add one mod at a time and test thoroughly before adding another. This helps you identify any conflicts quickly.
> - **Review compatibility notes** - Check mod pages for compatibility warnings, especially with major expansions like SVE, Ridgeside Village, or East Scarp.
> - **Create a private collection** - Once you've found mods that work well, create a private collection containing just your additions. This makes it easy to reinstall them after collection updates. See our [Personalization guide](Guides/personalization.md) for details.
> - **Check load order** - Some mods may need specific load orders. Use Vortex's "Manage Rules" to adjust if needed.
> 
> Remember that adding mods can introduce conflicts or bugs, and collection updates may not account for your additions. Keep backups of working configurations!

**Can I disable a required mod?**
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

### MacOS Installation

**Mod Managers**
> Nexus Mods App has planned support for MacOS, but currently no mod manager with collection support exists. Mac users may use our [Manual Installation](Installation/Manual/installation.md) guide or our [Stardrop](Installation/Stardrop/installation.md) guides and transfer from a Windows machine.

**MacOS SMAPI Security Issues**

**Important:** Certain MacOS versions flag SMAPI as malware and forcibly move it to the trash, preventing installation.

*The following solutions are based on community findings, derivded from the Stardew community Discord, and may change as Apple updates MacOS security behaviors.*

**Problem 1: Unable to Run SMAPI Installer**
> When you receive a security message, go to Settings → Security (or Privacy & Security) and hit "Open Anyways" where it lists the blocked file.

**Problem 2: MacOS reports "Malware Blocked and Moved to Trash"**
> Enable MacOS security permissions:

1. Go to System Settings > Privacy and Security
2. Make sure Developer Tools is visible. If you don't see it, open Terminal through Spotlight and enter:
   ```
   spctl developer-mode enable-terminal
   ```
3. Click Developer Tools
4. Add Terminal to the list and enable it
5. If you have other terminal programs (iTerm2, Hyper, Kitty, Alacritty), add them to Developer Tools as well
6. Restart your computer
7. Force close Steam if using it
8. Download and reinstall SMAPI

**Note:** This solution may change over time as Apple updates MacOS security behaviors. If this doesn't work:
- Restart your computer again
- Force close Steam, then try installing SMAPI
- Check the [SMAPI Mac installation wiki](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Mac) for updated solutions

*For the most current solutions and community discussions, visit the the [SMAPI GitHub repository](https://github.com/Pathoschild/SMAPI).*

---

## Vortex Behaviors & Workarounds

**Updates can overwrite/delete custom configs**
> When a collection updates, Vortex may overwrite or delete your custom mod configurations. This is frustrating, but there are ways to protect your settings:
> 
> **Option 1: Sync Mod Configurations**
> - Use the "Sync Mod Configurations" button in Vortex to backup and restore your settings
> - This saves your configurations and can restore them after updates
> 
> **Option 2: Create a Custom Config Mod (Recommended)**
> - This is the most reliable method. Create a custom mod that contains only your configuration files
> - Your custom configs will load after the collection mods, so they won't be overwritten
> - See our [Personalization & Custom Configurations](Guides/personalization.md) guide for step-by-step instructions
> 
> Using the custom config mod method ensures your settings persist through all updates automatically!

**Mod staging may fail silently**
> Sometimes Vortex may show a mod as installed and enabled, but it might not actually be loaded in the game. This is called "silent staging failure."
> 
> To verify mods are actually loaded:
> 1. Launch the game and check the **SMAPI log** (the console window that appears)
> 2. Look for the mod in the "Loaded X mods" list at the start of the log
> 3. Compare this with what's shown in the Vortex Mods tab
> 
> If a mod is missing from the SMAPI log:
> - Try clicking **Deploy** in Vortex to force redeployment
> - If that doesn't work, delete the mod and reinstall it from the Collection tab
> - Check the SMAPI log for any errors related to that specific mod

**Incorrect mod folder structures**
> Some mods may have incorrect folder structures that prevent them from loading properly. This usually happens with manually downloaded mods or older mod versions.
> 
> To fix this:
> 1. Check the mod's Nexus page or documentation for the correct folder structure
> 2. Compare with the [official modding guide](https://stardewvalleywiki.com/Modding:Modder_Guide/Get_Started#Mod_structure) structure requirements
> 3. Right-click the mod in Vortex → **Open in File Manager** to inspect its structure
> 4. Fix the folder structure manually (ensure the mod's files are directly in the mod folder, not nested too deep)
> 5. Click **Deploy** in Vortex to apply the changes
> 
> The correct structure is usually: `Mods/[ModName]/[ModName].dll` or `Mods/[ModName]/manifest.json`

**Red errors from an "empty Vortex folder"**
> If you see red error messages in Vortex about an "empty Vortex folder," this typically means:
> - There are leftover files from a previous installation
> - A mod was installed but only contains configuration or translation files (no actual mod content)
> - A mod archive was extracted incorrectly
> 
> To resolve:
> 1. Check what's actually in the problematic mod folder (right-click → **Open in File Manager**)
> 2. If it's a config-only install, you may need to enable additional files from the mod's archive
> 3. If it's leftovers, delete the mod and reinstall it cleanly
> 4. Sometimes you can safely ignore these errors if the mod is working correctly - check your SMAPI log to confirm

**Generic Mod Config Menu (GMCM) version compatibility**
> Use the version of Generic Mod Config Menu (GMCM) that's recommended in the collection. Newer versions may introduce compatibility issues or cause certain menus to soft-lock (freeze when opened).
> 
> If you've updated GMCM manually and are experiencing menu freezes:
> 1. Check which version the collection recommends
> 2. Reinstall that specific version from the collection
> 3. Test if the issue is resolved
> 
> Collection curators test specific mod versions together, so sticking to the recommended versions ensures stability.

---

## Known Technical Issues

**Multiplayer / split-screen desync**
> If you experience desynchronization in multiplayer (players seeing different things, actions not registering, or players getting stuck), this is usually a temporary network or mod state issue.
> 
> Quick fixes to try:
> 1. **Relaunch the game** - All players should quit and restart the game completely
> 2. **Restart the session** - The host should save, close the game, and start a new multiplayer session
> 3. **Check mod sync** - Ensure all players have the exact same mods enabled and the same versions
> 4. **Verify configurations match** - Important mod configurations should be identical across all players
> 
> Persistent desync issues may indicate mod conflicts or version mismatches. Check the SMAPI logs from all players for errors.

**Failed to Store Cache Entry (SinZational Speedy Solutions)**
> This error message appears in your SMAPI log related to SinZational Speedy Solutions, but **it's completely safe to ignore**. It's an informational message, not an actual error.
> 
> - It does **not** indicate a crash or conflict
> - It does **not** affect gameplay
> - Your game will run normally despite this message
> - No action is needed
> 
> This is a known quirk of the mod and doesn't impact functionality. You can safely continue playing!

**Unresolved file conflicts (Manage Rules)**
> Vortex may show file conflicts in the "Manage Rules" section. These typically occur when multiple mods modify the same files. Here's how to resolve them properly:
> 
> **For configuration/compatibility/translation files:**
> - These files should **load after** the mods they affect
> - Set them to load after their parent mod in Manage Rules
> - Click **Deploy** to apply the changes
> 
> **Avoid using "Use Suggested":**
> - Sometimes Vortex's suggested resolutions can create dependency loops
> - Manually set load orders instead
> - If you see a loop warning, you'll need to resolve it manually or remove one of the conflicting mods
> 
> **Testing:**
> - After resolving conflicts, test your game thoroughly
> - Check the SMAPI log for any errors related to the conflicting mods
> - If issues persist, you may need to choose which mod's version of the conflicting file takes priority

**SMAPI not launching**
> If SMAPI isn't launching when you try to start the game:
> 1. Open Vortex
> 2. Go to the **Dashboard** tab
> 3. Find the Stardew Valley entry
> 4. Make sure SMAPI is set as the **Primary Tool** (there should be a "Set as Primary" button if it's not)
> 5. Try launching the game again from Vortex
> 
> If this doesn't work, you may need to reinstall SMAPI. See our [Installation guides](../../Installation/index.md) for detailed instructions.

---

## Getting Help

- [Community Discord](https://discord.com/invite/de2NrHXuty)
- [Vortex Support Discord](https://discord.com/invite/nexusmods)
- [Vortex Wiki](https://wiki.nexusmods.com/index.php/Category:Vortex)

