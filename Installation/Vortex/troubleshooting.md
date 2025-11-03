# Troubleshooting - Vortex

> 📂 Docs / Installation / Vortex / Troubleshooting

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* **1.6.15+**

This page focuses on troubleshooting Vortex-related setup issues for the collections.

---

## Quick Fix: Try Restarting First!

Before diving into complex troubleshooting steps, restart your computer and try again. Many issues with Vortex, SMAPI, or the game itself can be resolved with a simple restart.

---

## Part 1 - Game Installation Check (Game itself is healthy)

1. Use your store launcher to verify integrity of game files:
   - Steam: Library → Stardew Valley → Properties → Installed Files → Verify  
   - GOG: More → Manage Installation → Verify / Repair  
   - Xbox / Game Pass: Right-click game → Manage → Files → Verify and Repair

---

## Part 2 - Vortex Profile Check (Only collection mods selected)

1. On the Nexus Mods collection page, click Add Collection.
2. When prompted, install into a New Profile.
3. In Vortex, switch to that profile and confirm only the collection's mods are enabled.
4. Ensure Optional Mods are ticked for full functionality.

---

## Part 3 - Game Mods Folder Check (Only mods Vortex knows about)

1. In Vortex → Mods tab, click Purge to remove all active mods from the game folder.
2. Click Open → Game Mods Folder and manually delete any files/folders left behind.
3. Back in Vortex, click Deploy to put the clean set of mods back.

---

## Vortex-Specific Tips

- Set SMAPI as the Primary Tool in Dashboard; re-add if missing.  
- Manage Rules: ensure configuration/compat/translation mods load after the mods they affect; avoid Use Suggested if it creates loops.  
- After Deploy, confirm mods actually loaded in the SMAPI log (not just the Mods tab).  
- If a mod is missing: Redeploy, or delete the mod and its archive, then reinstall from the Collection tab.

### Mod Not Unpacking with All Files
> If a mod does not unpack with all its files, it may not be constructed per SMAPI guidelines. Vortex may filter out extra folders or struggle with mods that contain multiple manifests.
> 
> **Solution:** Go to Downloads → View All Downloads, find the mod file, right-click it and select **"Unpack As-Is"**. This will deposit the entire file contents regardless of the mod's folder structure, ensuring all files are included.

### Mod Not Installing as Expected
> If a mod does not install as expected, you may wish to right-click the mod and select **Reinstall**. This will correct issues with improper unpacking.
> 
> However, if there is an issue with the archive itself, it may be best to remove the mod and its archive, then redownload. Both steps can easily be done from the Collections panel.

## Common Error Messages

### "Vortex needs access to [file] but it's write protected"
> This error message is misleading. Vortex locks files it's already accessing as a safety feature to prevent file corruption. The error doesn't clearly indicate this and can lead you down a rabbit hole of file permissions troubleshooting.
> 
> **Solution:** Simply restart Vortex. This will release the file locks and allow Vortex to access the files normally. No file permission changes or administrator rights are needed.

### "Empty Vortex folder (is the mod disabled in Vortex?)"
> SMAPI may display this error for any file. This typically indicates one of two situations:
> 
> **Situation 1: Vortex didn't properly clean up when a mod was disabled**
> - This is common if mods are disabled while the game is active
> - **Solution:** Running through the troubleshooting steps above (Game Installation Check, Vortex Profile Check, Game Mods Folder Check) will solve this issue
> 
> **Situation 2: Collection-distributed additional files are still present**
> - Collections may distribute additional files (configurations, portraits, etc.) so that the folder will persist without a manifest when the mod is disabled
> - **Solution:** In this case, the error can be safely ignored, or you can find and disable the additional sources
> 
> **If you encounter this with collection configurations:**
> - You may wish to disable the collection's configuration mods and opt to use the [Collection Configuration Manager FOMOD](https://www.nexusmods.com/stardewvalley/mods/20870), which is particularly useful for [combining collections](../Collections/combining-collections.md)
> - See the [Personalization & Custom Configurations](../../Guides/personalization.md) guide for alternative solutions

---

## Need More Help?
- **Community Discord:** [Join Here](https://discord.com/invite/de2NrHXuty)  
- **Official Vortex Discord:** [Join Here](https://discord.com/invite/nexusmods) (Support hours: 9 AM – 5 PM GMT, Mon–Thu)

More help:  
- **Vortex Wiki:** [Read Here](https://wiki.nexusmods.com/index.php/Category:Vortex)  
- **Stardew Setup Guide:** [Read Here](https://wiki.nexusmods.com/index.php/Modding_Stardew_Valley_with_Vortex)

The official Stardew Valley Discord does not support Vortex.

---

## How to Create a SMAPI Log
### Create a SMAPI Log in Vortex
1. Press the `SMAPI Log` button in the toolbar on the Mods Page
2. Pop-up containing log text will appear. Click `Copy & Share Log`.
3. Browser will open to [smapi.io/log](https://smapi.io/log) automatically.
4. Paste into the 'paste log here' window and then press the `save & parse log` button to generate a sharable link.

### Outside of Vortex

**Windows:**
1. Press Windows+R  
2. Enter: `%appdata%\StardewValley\ErrorLogs`  
3. Open SMAPI-latest.txt (or SMAPI-crash.txt if it crashed)
4. Upload the file to [smapi.io/log](https://smapi.io/log) and share the generated link in Discord

**Linux:**
1. Navigate to `~/.config/StardewValley/ErrorLogs` in your file manager
2. Open SMAPI-latest.txt (or SMAPI-crash.txt if it crashed)
3. Upload the file to [smapi.io/log](https://smapi.io/log) and share the generated link in Discord

