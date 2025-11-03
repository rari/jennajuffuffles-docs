# Troubleshooting

> 📂 Docs / Guides / Troubleshooting

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* **1.6.15+**

---

## Quick Fix: Try Restarting First!

Before diving into complex troubleshooting steps, restart your computer and try again. Many issues with Vortex, SMAPI, or the game itself can be resolved with a simple restart.

---

## Common Issues

### Duplicate Mods

One common issue we see is **duplicate mods**. When two copies of a mod exist, neither will load. This includes if a mod is inside of a subfolder inside of the `Mods/` folder. When this happens, it will produce a red SMAPI error.

**Important:** It is recommended that the mod folder be clear when installing a new collection (unless deliberately stacking collections). 

**To fix duplicate mods:**
- Check your `Mods/` folder for any duplicate mod directories
- Look for mods nested inside subfolders - mods should be directly in `Mods/` (e.g., `Mods/ModName/manifest.json`, not `Mods/Folder/ModName/manifest.json`)
- Remove any duplicate or incorrectly placed mod folders
- Restart the game and check the SMAPI log to confirm the mod loads correctly

---

## Vortex-Specific Troubleshooting

For Vortex-specific troubleshooting steps including game installation checks, profile verification, and mod folder management, see the [Vortex Troubleshooting](../Installation/Vortex/troubleshooting.md) guide.

---

## Need More Help?

If you run into issues that aren't solved here, you can:
- Reach out to our community on **[Discord](https://discord.com/invite/de2NrHXuty)** for live assistance
- Create and share a SMAPI log so others can help diagnose your issue

## Further Support

For Vortex support:
- **Official Vortex Discord**: [Join Here](https://discord.com/invite/nexusmods)
- **Support Hours**: 9 AM – 5 PM GMT, Monday–Thursday

More help available:
- **Vortex Wiki**: [Read Here](https://wiki.nexusmods.com/index.php/Category:Vortex)
- **Stardew Setup Guide**: [Read Here](https://wiki.nexusmods.com/index.php/Modding_Stardew_Valley_with_Vortex)

The **official Stardew Valley Discord** does *not* support Vortex. Please respect their policy.

---

## Additional Resources for Expansion Mods

**Important:** Please avoid troubleshooting in these Discords unless you can show (via log) a repeatable error from their mod without the rest of the collection active. Please be respectful of other's time, and understand that many helpers are not comfortable with mod managers other than Stardrop.

If you're experiencing issues with specific expansion mods, these resources may help:

### Stardew Valley Expanded
- [Installation Guide](https://github.com/FlashShifter/StardewValleyExpanded/wiki/Install-guide)
- [Troubleshooting](https://github.com/FlashShifter/StardewValleyExpanded/wiki/Troubleshooting)
- [Wiki](https://stardew-valley-expanded.fandom.com/wiki/Stardew_Valley_Expanded_Wiki)
- [Discord](https://discord.com/invite/svexpanded)

### Ridgeside Village
- [Installation Guide](https://github.com/Rafseazz/Ridgeside-Village-Mod/blob/main/Installation%20Guide.md)
- [Wiki](https://ridgeside.fandom.com/wiki/Ridgeside_Village_Wiki)
- [Discord](https://discord.gg/4SRbjEQG2D)

### East Scarp and Sword & Sorcery, Lurking in the Dark, Nora, etc
- [Wiki](https://eastscarp.fandom.com/wiki/East_Scarp_Wiki)
- [Discord](https://discord.com/invite/QFtDA3CJwJ)

---

## How to Create a SMAPI Log

A SMAPI log is a text file that shows what mods loaded and any errors that occurred.
Share the link in our [Discord](https://discord.gg/de2NrHXuty) for help!

### Windows Users:
1. Press the **Windows** and **R** keys at the same time.
2. In the 'Run' box that appears, enter:
   ```
   %appdata%\StardewValley\ErrorLogs
   ```
3. The log file is `SMAPI-crash.txt` if it exists, otherwise `SMAPI-latest.txt`. Upload it to [smapi.io/log](https://smapi.io/log).

### Linux Users:
1. Open the Files app.
2. Click the options menu (might be labeled Go or ⋮).
3. Choose Enter Location.
4. Enter this exact text:
   ```
   ~/.config/StardewValley/ErrorLogs
   ```
5. The log file is `SMAPI-crash.txt` if it exists, otherwise `SMAPI-latest.txt`. Upload it to [smapi.io/log](https://smapi.io/log) 

### Mac Users:
1. Open the Finder app.
2. Click Go at the top, then Go to Folder.
3. Enter this exact text:
   ```
   ~/.config/StardewValley/ErrorLogs
   ```
4. The log file is `SMAPI-crash.txt` if it exists, otherwise `SMAPI-latest.txt`. Upload it to [smapi.io/log](https://smapi.io/log) 


**Tip:** The log will show a lot of information about your setup, exactly which mods loaded successfully and highlight any problems in red. This information can help in troubleshooting even when a crash isn't specifically displayed.