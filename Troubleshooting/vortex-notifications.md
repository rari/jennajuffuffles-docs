# Vortex Notifications and Solutions
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

Most Vortex notifications are informational, not errors. Find the message you see and the solution, or start with the [Quick Fix Process](#quick-fix-process):

- [Install Options Pop-ups (During Collection Updates)](#install-options-pop-ups-during-collection-updates)
- [Unresolved File Conflict Notifications](#unresolved-file-conflict-notifications)
- [Cyclical Rules / Circular Dependencies](#cyclical-rules--circular-dependencies)
- ["Vortex needs access to [file] but it's write-protected"](#vortex-needs-access-to-file-but-its-write-protected)
- ["Version mismatch. Your version shows as 4.X.X"](#version-mismatch-your-version-shows-as-4xx)
- [Dependency Notifications](#dependency-notifications)
- [External Changes Detected](#external-changes-detected)
- [Update Notifications](#update-notifications)
- [Deployment Notifications](#deployment-notifications)
- ["Empty Vortex folder (is the mod disabled in Vortex?)"](#empty-vortex-folder-is-the-mod-disabled-in-vortex)

Load order is covered in [Manage Rules](#manage-rules).

## Quick Fix Process

Start here before a full reinstall.

1. Restart the computer. This clears temporary files and file locks.
2. [Reset your content files](reset-your-content-files.md). Verify Stardew Valley in Steam, GOG, or the Xbox app, then launch the game once.
3. Purge and redeploy:
   1. Click **Purge Mods**.
   2. Click **Open > Game Mods Folder** (the third option) and delete leftover files and folders.
   3. Click **Deploy**.
4. If it still fails, install the collection on a fresh profile:
   1. On the **Collections** tab, remove the collection. Do not remove the mods.
   2. On the Nexus collection page, click **Add Collection**, then confirm in Vortex.
   3. On the **Mods** tab, disable the collection.
   4. Re-enable it with the recommended mods so installed optional mods turn back on.

## Vortex Pop-ups

These are the notifications, dialogs, and pop-ups Vortex displays, grouped by severity.

### Install Options Pop-ups During Collection Updates

{% hint style="info" %}
These pop-ups appear for every mod during large collection updates. This is expected behavior.
{% endhint %}

**What it means:** When updating a collection, Vortex may ask how to handle each mod that's already installed:

- **Replace existing file** - Overwrites your current version
- **Re-install as variant** - Keeps both versions
- **Remove mod** - Removes the existing version so it can be replaced with the newer version

**What to do:**

- For collection updates, choose **Replace existing file** for consistency

{% hint style="warning" %}
When Vortex asks to remove mods, allow it to remove them. Failure to remove can result in duplicates that will prevent either mod from loading.
{% endhint %}

- There's currently no way to disable these prompts for mass updates
- For cleaner updates, you can remove the collection and reinstall fresh
- If a collection update still fails, see [Collection / Update Issues](collection-update-issues.md)

### Unresolved File Conflict Notifications

**What it means:** Multiple mods are trying to modify the same files. Vortex shows a red lightning bolt icon in the Dependencies column when file conflicts are unresolved.

**What to do:**

- Most conflicts resolve automatically when you click **Deploy**
- The collections have some mods flagged to not be used together to prevent errors. In these cases, just disable one of the mods in the pair.
- Collections are pre-configured with rules to handle conflicts
- If conflicts persist after deployment, you can manually set rules in **Manage File Conflicts** / **Manage Rules** (see [Managing Load Order Rules](#managing-load-order-rules) below)

**How to manually resolve conflicts:**

1. Go to the **Mods** tab
2. Click **Manage Rules** (or look for the rules icon)
3. Find the mods with conflicts
4. Set one mod to **Load Before** or **Load After** the other
5. Click **Deploy** to apply changes

See [Managing Load Order Rules](#managing-load-order-rules) for how rules work and when to change them.

### Cyclical Rules / Circular Dependencies

**What it means:** Your mod rules have contradictions (for example, Mod A loads after Mod B, but Mod B also loads after Mod A). This breaks Vortex's ability to sort the load order.

**What to do:**

- Click **More** in the notification to see which mods are involved
- Remove or adjust the conflicting rules
- Collections should not have cyclical rules. If you see this, it may be due to custom mods you've added
- Please report this to JennaJuffuffles's Discord or the collection comments

**How to fix cyclical rules:**

1. Go to the **Mods** tab
2. Click **Manage Rules**
3. Find the conflicting rules
4. Remove one of the conflicting rules
5. Manually set the correct load order if needed
6. Click **Deploy** to apply changes

If this does not correct the cyclical rule, try removing the collection from the Collections tab (do not remove mods here), then right-click and reinstall the specific mods involved from the Mods tab.

{% hint style="warning" %}
Avoid using "Use Suggested" when fixing loops, as Vortex may suggest rules that create new loops. Manually set rules instead.
{% endhint %}

See [Managing Load Order Rules](#managing-load-order-rules) for more on avoiding and fixing rule loops.

### Error Notifications

Most errors have straightforward solutions. Check the notification details for the specific error, then review [Your SMAPI Log](your-smapi-log.md) for additional context.

**What it means:** Something went wrong with a mod installation, download, or deployment.

**What to do:**

- Check the notification details for specific error messages
- Review [Your SMAPI Log](your-smapi-log.md) for errors
- Common causes: missing files, corrupted downloads, insufficient disk space

### "Vortex needs access to [file] but it's write-protected"

**Quick fix:** Restart Vortex. This releases file locks and resolves the issue.

**Symptom:** Error message: "Vortex needs access to [file] but it's write-protected"

**Cause:** Vortex locks files it's already accessing as a safety feature to prevent file corruption. This error message is misleading and doesn't clearly indicate this.

**Solution:** Restart Vortex. This releases the file locks and allows Vortex to access the files normally. No file permission changes or administrator rights are needed.

**When this occurs:** This typically happens when Vortex is already accessing files and tries to access them again.

### "Version mismatch. Your version shows as 4.X.X"

{% hint style="warning" %}
Fix this issue before publishing any collection changes. Editing a collection in this state may prevent you from editing it.
{% endhint %}

**Quick fix:** Verify game files through your store launcher, then ensure SMAPI is set as Primary Tool in the Vortex Dashboard.

**Symptom:** Error message: "Version mismatch. Your version shows as 4.X.X"

**Cause:** Your `Stardew Valley.exe` has been replaced by the SMAPI executable. This happens with how some mod managers handle SMAPI installation.

**When this occurs:** This typically happens after SMAPI installation when the executable replacement isn't properly recognized.

**Solution:**

1. Verify game files through your store launcher:
   - **Steam:** Library > Stardew Valley > Properties > Installed Files > Verify
   - **GOG:** More > Manage Installation > Verify / Repair
   - **Xbox / Game Pass:** Right-click the game > Manage > Files > Verify and Repair
2. Ensure SMAPI is properly installed and deployed through Vortex:
   - In Vortex > Dashboard, make sure SMAPI is set as the Primary Tool
   - Go to the Mods tab and ensure SMAPI is enabled and deployed
   - Click **Deploy** to ensure SMAPI is properly linked
3. If the issue persists, reinstall SMAPI through Vortex. SMAPI can be added as a mod from Nexus Mods and Vortex will automatically install it. See [Install with Vortex](../Install/vortex.md).

### Dependency Notifications

{% hint style="info" %}
These are warnings, not errors. They're safe to ignore if you've intentionally disabled the mod.
{% endhint %}

**What it means:** The collection requires a mod or framework that isn't installed or enabled.

**What to do:**

- These warnings alert you that your collection is incomplete
- Install the missing dependency if it's genuinely missing
- These warnings can typically be ignored for experienced modders, and if you've intentionally disabled the mod then the warning may be ignored

### External Changes Detected

{% hint style="info" %}
If you see this from SinZational Speedy Solutions, this is expected behavior when it clears its cache.
{% endhint %}

**What it means:** Vortex detected that files it manages have been modified outside of Vortex. This happens when files are edited, deleted, or replaced by another tool or manually.

**Why it happens:**

- You manually edited a mod file (config, texture, etc.)
- Another program modified files (antivirus, system tools, etc.)
- Files were moved or deleted outside of Vortex
- Hard links between Vortex's staging folder and game folder were broken

**What to do:**

- **Read the dialog carefully.** It will show which files were affected
- **If you did not make changes:** It is typically safe to **Save/Apply changes**. Some mods (like SinZational Speedy Solutions) trigger this detection when clearing their own cache, and saving is the correct action
- **If you intentionally edited files:** Use **Save/Apply changes** to keep your edits permanently
- **Revert/Undo changes** - Use this if you want to discard external changes and restore the original mod files from Vortex's staging folder
- **Use Newer File** - If available, this chooses the version with the most recent timestamp
- **Important:** Once you confirm your choice, you cannot undo it

**Best practices:**

- Avoid editing mod files directly in the game folder. Edit them in Vortex's staging folder if possible
- If you get this notification frequently without making changes, and the source is not SinZational Speedy Solutions, it may indicate problems

#### Update Notifications

**What it means:** A mod or collection has an update available.

**What to do:**

- **Always update collections, not individual mods.** Collections are tested together for compatibility. Updating individual mods outside of collection updates can break compatibility with other mods in the collection.
- Use the collection's Update button rather than updating mods individually
- See [Collection / Update Issues](collection-update-issues.md)

### Deployment Notifications

{% hint style="info" %}
You'll see this notification after installing or updating mods. This is expected behavior.
{% endhint %}

**What it means:** Mods need to be deployed to your game folder before they'll work.

**What to do:**

- **Click Deploy.** This applies your mods to the game folder
- This appears after installing or updating mods
- Mods won't work until they're deployed

### "Empty Vortex folder (is the mod disabled in Vortex?)"

**Quick fix:** For Situation 1, follow the [Quick Fix Process](#quick-fix-process). For Situation 2, the error can be safely ignored.

**Symptom:** SMAPI error: "Empty Vortex folder (is the mod disabled in Vortex?)"

**Cause:** This typically indicates one of two situations:

**Situation 1: Vortex didn't properly clean up when a mod was disabled**

- This is common if mods are disabled while the game is active

**Situation 2: Collection-distributed additional files are still present**

- Collections may distribute additional files (configurations, portraits, etc.) so that the folder will persist without a manifest when the mod is disabled

**Solution:**

- **For Situation 1:** The [Quick Fix Process](#quick-fix-process) covers the shared cleanup that solves this
- **For Situation 2:** The error can be safely ignored, or you can find and disable the additional sources

**Expected behavior:** Often due to leftover folders from disabled mods or collection-distributed files. Non-harmful. Enable recommended files or customize configs.

**If you encounter this with collection configurations:**

- See [Adjusting Configurations](../Customize/adjusting-configurations.md) for editing a collection's VERY Configured files in Vortex

**Reference:** This error is also mentioned in [Your SMAPI Log](your-smapi-log.md). The longer fix is here.

## Vortex Behavior

How Vortex behaves with these collections, and what to do when a mod does not unpack as expected.

### Vortex-Specific Tips

- **SMAPI installation** - SMAPI can be added as a mod from Nexus Mods and Vortex will automatically install it
- **Set SMAPI as Primary Tool** - In Dashboard, ensure SMAPI is set as the Primary Tool; re-add if missing
- **Where to install** - For best results, install both Stardew Valley and Vortex on `C:\` to avoid symbolic link issues
- **Mod manager conflicts** - Do not run two mod managers on the same game simultaneously. You may corrupt installs
- **Manage Rules** - Ensure configuration, compatibility, and translation mods load after the mods they affect. Avoid "Use Suggested" if it creates loops
- **Verify mod deployment** - After Deploy, confirm mods actually loaded in the SMAPI log (not just the Mods tab). Mod staging may fail silently. Always verify in [Your SMAPI Log](your-smapi-log.md)
- **Missing mods** - If a mod is missing in-game despite being enabled in Vortex: Redeploy, or delete the mod and its archive, then reinstall from the Collection tab
- **Combining collections** - Install to the same profile. Pick **Fairycore or Witchcore**, not both (see [About the Collections](../Reference/about-the-collections.md)). If Manage Rules requires attention, set **VERY Configured** to **After All** (**svVe** last among them)

### Mod Not Installing as Expected / Incorrect Folder Structure

If a mod isn't installing correctly or has an incorrect folder structure, try these solutions.

#### Reinstall or Redownload

- **Right-click the mod** and select **Reinstall** to correct issues with improper unpacking
- **Remove the mod and archive**, then redownload from the Collections panel if there's an issue with the archive itself
- If the file cannot be installed as-is due to structural issues, it may attempt to reinstall and then display as uninstalled

#### Resolving Structural Issues

If a mod doesn't unpack with all its files, its folder structure may not be constructed per SMAPI guidelines. Vortex may filter out extra folders, missing top-level folders, or struggle with mods that contain multiple manifests.

**Step 1: Use "Unpack As-Is"**

1. Go to **Downloads > View All Downloads** (bottom of the screen)
2. Find the mod file
3. Right-click it and select **"Unpack As-Is"**
4. This deposits the entire file contents regardless of the mod's folder structure, so all files are included

**Step 2: Fix the folder structure manually**

1. Right-click the mod in Vortex > **Open in File Manager** to inspect its structure
2. Check the mod's Nexus page or documentation for the correct folder structure
3. Compare with the [official modding guide structure requirements](https://stardewvalleywiki.com/Modding:Modder_Guide/Get_Started#Folder_structure)
4. Fix the folder structure manually (the mod's files should be directly in the mod folder, not nested too deep)
5. Click **Deploy** in Vortex to apply the changes

## Manage Rules

Load order management and rules. This page owns that explanation.

### Managing Load Order Rules

**Manage Rules** controls the **load order** of your mods from staging to deployment. This matters for mods that modify the same files.

Think of load order like layers: mods that load first are the base layer, and mods that load after can override or modify what came before. This is how configuration mods work. They load after the mods they configure so they can change settings.

**What you'll see in Manage Rules:**

- A list of all your mod conflict pairs, listed in both directions
- Set your **VERY Configured** to load **After All** (for multiple collections, set svVe last)
- Visual indicators showing which mods have rules set
- A button to hide resolved rules

### What Are Rules?

Rules tell Vortex:

- "Load Mod A before Mod B"
- "Load Mod B after Mod A"
- "Mod A and Mod B conflict - choose one"

### When You Need to Change Rules

Collections ship with correct load orders already set. In normal play you rarely touch **Manage Rules**.

During **install** or a **collection update**, Vortex may still open **Manage Rules** and ask you to finish unresolved rules. If that happens, follow [When Vortex asks you to set rules](#when-vortex-asks-you-to-set-rules) below before you play.

### When Vortex asks you to set rules

{% hint style="warning" %}
If Vortex prompts you to set rules during install or update, finish this step. Skipping it can prevent collection configuration from applying (for example, a missing mine entrance after install).
{% endhint %}

When Vortex asks you to set rules, apply the **VERY Configured** rule from above:

1. Go to the **Mods** tab
2. Click **Manage Rules**
3. Scroll through the list and find each **VERY Configured** entry (you may see one per collection, for example Stardew Valley VERY Expanded, Aesthetic Valley Fairycore)
4. Set each **VERY Configured** to load **After All**
5. **Multi-collection profiles:** If you have more than one **VERY Configured**, set **Stardew Valley VERY Expanded (svVe)** to load **last** among them (other collection configs first, then svVe)
6. Click **Deploy**

**Never use "Use Suggested"** for this. Suggested rules can create loops or the wrong load order.

**How to tell configuration did not apply:** If your mine entrance is missing, right-click **Stardew Valley VERY Configured - Stardew Valley VERY Expanded** in the Mods panel and select **Reinstall**, then confirm the **After All** rule is still set and **Deploy** again.

### How Rules Work

**Load Before / Load After:**

- Mods that load **before** apply their changes first
- Mods that load **after** can override those changes
- This is how configuration mods work. They load after the mods they configure

**Example:**

- Base mod loads first
- Translation mod loads after mod (applies language into the mod's folder)
- Configuration mod loads after (overwrites the base mod's config if it exists)

### How to Change Rules (other mods)

For rules outside **Stardew Valley VERY Configured**, or if you added custom mods:

1. Go to the **Mods** tab
2. Click **Manage Rules** (or look for the rules icon)
3. Find the mod you want to adjust
4. Set it to **Load Before** or **Load After** the other mod (or **After All** when that option fits)
5. Click **Deploy** to apply changes

**What you'll see:** After clicking Deploy, Vortex reorganizes your mods according to the new rules.

### Important Warnings

#### Avoid "Use Suggested"

- Vortex may suggest rules that create loops
- Manually set rules instead
- If you see a loop error, remove the problematic rule

#### Don't Create Loops

- A loop means "A loads before B, B loads before A", which is impossible
- Vortex will warn you about loops
- Fix loops by removing or adjusting rules

#### Test After Changes

- After changing rules, test your game
- Check [Your SMAPI Log](your-smapi-log.md) for errors
- Revert changes if issues occur

## Need More Help?

Before seeking help, check [Your SMAPI Log](your-smapi-log.md). It often contains the information needed to resolve the issue.

**Community resources:**

- **Community Discord:** [Join here](https://discord.gg/MPcgJUXeeY)
- **Official Vortex Discord:** [Join here](https://discord.gg/vortex) (support hours: 9 AM - 5 PM GMT, Mon-Thu)

**Official documentation:**

- **Vortex Wiki:** [Read here](https://wiki.nexusmods.com/index.php/Vortex)
- **Stardew setup guide:** [Read here](https://stardewvalleywiki.com/Modding:Installing_SMAPI)

{% hint style="info" %}
The official Stardew Valley Discord does not support Vortex.
{% endhint %}

## Related

- [Install with Vortex](../Install/vortex.md)
- [Your SMAPI Log](your-smapi-log.md)
- [Collection / Update Issues](collection-update-issues.md)
