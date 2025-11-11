# Vortex — FAQ & Troubleshooting

> 📂 Docs / Installation / Vortex / FAQ & Troubleshooting

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* **1.6.15+**

This page covers frequently asked questions and troubleshooting for Vortex-related setup issues with the collections.

---

## Quick Fix Process

Follow these steps in order to resolve common Vortex installation issues.

### Part 1 - Game Installation Check (Game itself is healthy)

> 1. Use your store launcher to verify integrity of game files:
>    - Steam: Library → Stardew Valley → Properties → Installed Files → Verify  
>    - GOG: More → Manage Installation → Verify / Repair  
>    - Xbox / Game Pass: Right-click game → Manage → Files → Verify and Repair

### Part 2 - Vortex Profile Check (Only collection mods selected)

> 1. Go to the Collections tab and **Remove** the current version of the collection. Do not check any checkboxes so this removes only the collection entry, not the mods themselves.
> 2. On the appropriate Nexus Mods collection page, click Add Collection.
> 3. When prompted, click Install Now, and Yes to switch to profile.
> 4. If prompted to install optional mods, click Ok/Install. If you click other buttons (such as "View Optional Mods"), you may need to install those mods from the Collections panel later.
> 5. In the Mods panel, filter for the name of the collection. Disable it, then re-enable and select "Enable Recommended Mods" in the pop-up. This ensures your optional mods are properly enabled, as updates often disable them.

### Part 3 - Game Mods Folder Check (Only mods Vortex knows about)

> 1. In Vortex → Mods tab, click Purge to remove all active mods from the game folder.
> 2. Click Open → Game Mods Folder and manually delete any files/folders left behind.
> 3. Back in Vortex, click Deploy to put the clean set of mods back.

---

## FAQ

### Can I use Vortex with another mod manager?
Do not run two mod managers on the same game simultaneously — you may corrupt installs.

### Where should I install Stardew Valley and Vortex?
For best results, it's recommended to install both Stardew Valley and Vortex on `C:\`. This helps avoid potential issues with symbolic links and deployment.

### Best practices for combining collections
Install to the same profile. Let the chosen recolor/theme config load last in Rules Manager. See Combining Collections: [Combining Collections](../../Collections/combining-collections.md)

---

## Vortex-Specific Tips

- Set SMAPI as the Primary Tool in Dashboard; re-add if missing.  
- SMAPI can be added as a mod from Nexus and Vortex will automatically install it
- Manage Rules: ensure configuration/compat/translation mods load after the mods they affect; avoid Use Suggested if it creates loops.  
- After Deploy, confirm mods actually loaded in the SMAPI log (not just the Mods tab).  
- If a mod is missing: Redeploy, or delete the mod and its archive, then reinstall from the Collection tab.

### Mod Not Installing as Expected / Incorrect Folder Structure
**Reinstall or Redownload**
- Right-click the mod and select **Reinstall** to correct issues with improper unpacking
- If there's an issue with the archive itself, remove the mod and its archive, then redownload. Both steps can easily be done from the Collections panel
- If the file cannot be installed as-is due to structural issues, it may attempt to reinstall and then display as uninstalled.

**Resolving Structural Issues**
If a mod doesn't unpack with all its files, its folder structure may not be constructed per SMAPI guidelines. Vortex may filter out extra folders, missing top-level folders, or struggle with mods that contain multiple manifests.

**Step 1: Use "Unpack As-Is"**
- Go to Downloads → View All Downloads, find the mod file, right-click it and select **"Unpack As-Is"**
- This will deposit the entire file contents regardless of the mod's folder structure, ensuring all files are included

**Step 2: Fix Folder Structure Manually**
- Right-click the mod in Vortex → **Open in File Manager** to inspect its structure
- Check the mod's Nexus page or documentation for the correct folder structure
- Compare with the [official modding guide](https://stardewvalleywiki.com/Modding:Modder_Guide/Get_Started#Mod_structure) structure requirements
- Fix the folder structure manually (ensure the mod's files are directly in the mod folder, not nested too deep)
- Click **Deploy** in Vortex to apply the changes

---

## Vortex Behaviors & Workarounds

### Updates can overwrite/delete custom configs
When a collection updates, Vortex may overwrite or delete your custom mod configurations. This is frustrating, but there are ways to protect your settings. For information on updating collections, see the [Updating Collections](updating.md) guide.

**Option 1: Sync Mod Configurations**
- Use the "Sync Mod Configurations" button in Vortex to backup and restore your settings
- This saves your configurations and can restore them after updates
- This may try to "back-up" smapi-internal in error. If this happens, right-click on the created configuration mod, extract the created folder and return those files to their proper place. **Please report to Vortex staff if this happens, this issue needs more visibility.**

**Option 2: Create a Custom Config Mod (Recommended)**
- This is a reliable method, but more hands-on. Create a custom mod that contains only your configuration files
- Your custom configs will load after the collection mods, so they won't be overwritten
- See our [Personalization & Custom Configurations](../../Guides/personalization.md) guide for step-by-step instructions

Using the custom config mod method ensures your settings persist through all updates automatically!

### Unresolved file conflicts (aka Manage Rules)
Vortex may show file conflicts in the "Manage Rules" section. Manage Rules is how load order is handled. These typically occur when multiple mods modify the same files. Here's how to resolve them properly:

**For configuration/compatibility/translation files:**
- These files should **load after** the mods they affect
- Set them to load after their parent mod in Manage Rules
- Click **Deploy** to apply the changes

**Avoid using "Use Suggested":**
- Sometimes Vortex's suggested resolutions can create dependency loops
- Manually set load orders instead
- If you see a loop warning, you'll need to resolve it manually or remove one of the conflicting mods

**Testing:**
- After resolving conflicts, test your game thoroughly
- Check the SMAPI log for any errors related to the conflicting mods
- If issues persist, you may need to choose which mod's version of the conflicting file takes priority

### Loop Errors
A loop error indicates that a Rule is either self-referential or part of a larger group that is.

**To solve for the group version:**
- Open the Manage Rules panel and replan the rules so they no longer form a loop

**To fix a single rule loop:**

> 1. Enable the **Dependencies** column from the ⚙️ **Toggle Columns** menu on the Mods panel
> 2. This should show a red lightning bolt ⚡ next to the offending rule
> 3. Remove the bad rule by clicking on the **Network** icon and clicking the ⛔ icon next to the red rule(s)

### Redundant Files Error
This error indicates that the files in two mods are identical. This may indicate you have created a variation and can disable one. This may also (temporarily) activate Manage Rules until it is resolved.

### SMAPI not launching via Vortex
If SMAPI isn't launching when you try to start the game:

> 1. Open Vortex
> 2. Go to the **Dashboard** tab
> 3. Find the Stardew Valley entry
> 4. Make sure SMAPI is set as the **Primary Tool** (there should be a "Set as Primary" button if it's not)
> 5. Try launching the game again from Vortex

If this doesn't work, you may need to reinstall SMAPI through Vortex. SMAPI can be added as a mod from Nexus and Vortex will automatically install it. See our [Installation guides](../index.md) for detailed instructions.

---

## Common Issues

### Unresolved file conflicts (Manage Rules)
Ensure compatibility/config/translation mods load after the mods they affect. Open Mods → Manage Rules, set the relationship, then Deploy. Avoid "Use Suggested" if it creates loops. For more information on combining collections and managing conflicts, see the [Combining Collections](../../Collections/combining-collections.md) guide.

### Mod staging may fail silently
After Deploy, verify in the SMAPI log that the mod actually loaded (don't rely only on the Mods tab). If missing, Redeploy, or delete the mod and its archive, then reinstall from the Collection tab.

### Mods with incorrect folder structure
Some manual additions have improper layouts and won't deploy correctly. Fix structure per the official wiki, then Deploy.

### Red errors from an empty Vortex folder
Often due to leftover folders from disabled mods, or installing configuration without associated mods. Non-harmful; enable the recommended files or customize configs.

---

## Common Error Messages

### "Vortex needs access to [file] but it's write-protected"
This error message is misleading. Vortex locks files it's already accessing as a safety feature to prevent file corruption. The error doesn't clearly indicate this and can lead you down a rabbit hole of file permissions troubleshooting.

**Solution:** Simply restart Vortex. This will release the file locks and allow Vortex to access the files normally. No file permission changes or administrator rights are needed.

### "Empty Vortex folder (is the mod disabled in Vortex?)"
SMAPI may display this error for any file. This typically indicates one of two situations:

**Situation 1: Vortex didn't properly clean up when a mod was disabled**
- This is common if mods are disabled while the game is active
- **Solution:** Running through the [Quick Fix Process](#quick-fix-process) above will solve this issue

**Situation 2: Collection-distributed additional files are still present**
- Collections may distribute additional files (configurations, portraits, etc.) so that the folder will persist without a manifest when the mod is disabled
- **Solution:** In this case, the error can be safely ignored, or you can find and disable the additional sources

**If you encounter this with collection configurations:**
- You may wish to disable the collection's configuration mods and opt to use the [Collection Configuration Manager FOMOD](https://www.nexusmods.com/stardewvalley/mods/20870), which is particularly useful for [combining collections](../Collections/combining-collections.md)
- See the [Personalization & Custom Configurations](../../Guides/personalization.md) guide for alternative solutions

### Version mismatch. Your version shows as 4.X.X
This error occurs when your `Stardew Valley.exe` has been replaced by the SMAPI executable. This happens with how some mod managers handle SMAPI installation and is easily solved.

**⚠️ Important Warning:** Take special caution with this error, because editing a collection in this state may prevent you from editing it. Fix this issue before  publishing any collection changes.

**Solution:**

> 1. Verify game files through your store launcher:
>    - Steam: Library → Stardew Valley → Properties → Installed Files → Verify
>    - GOG: More → Manage Installation → Verify / Repair
>    - Xbox / Game Pass: Right-click game → Manage → Files → Verify and Repair
> 2. Ensure SMAPI is properly installed and deployed through Vortex:
>    - In Vortex → Dashboard, make sure SMAPI is set as the Primary Tool
>    - Go to Mods tab and ensure SMAPI is enabled and deployed
>    - Click **Deploy** to ensure SMAPI is properly linked
> 3. If the issue persists, reinstall SMAPI through Vortex. SMAPI can be added as a mod from Nexus and Vortex will automatically install it. See our [Installation guides](../index.md) for detailed instructions.

---

## How to Create a SMAPI Log
### Create a SMAPI Log in Vortex
Vortex makes this SMAPI Log sharing very simple:

> 1. Press the `SMAPI Log` button in the toolbar on the Mods Page
> 2. Pop-up containing log text will appear. Click `Copy & Share Log`.
> 3. Browser will open to [smapi.io/log](https://smapi.io/log) automatically.
> 4. Paste into the 'paste log here' window and then press the `save & parse log` button to generate a sharable link.

### Outside of Vortex

For instructions on creating a SMAPI log without using Vortex (Windows, Linux, and Mac), see the [SMAPI Log creation guide](../../Guides/troubleshooting.md#how-to-create-a-smapi-log) in the general troubleshooting guide.

---

## Need More Help?
- **Community Discord:** [Join Here](https://discord.gg/MPcgJUXeeY)  
- **Official Vortex Discord:** [Join Here](https://discord.com/invite/nexusmods) (Support hours: 9 AM – 5 PM GMT, Mon–Thu)

More help:  
- **Vortex Wiki:** [Read Here](https://wiki.nexusmods.com/index.php/Category:Vortex)  
- **Stardew Setup Guide:** [Read Here](https://wiki.nexusmods.com/index.php/Modding_Stardew_Valley_with_Vortex)

The official Stardew Valley Discord does not support Vortex.
