---
title: Creating Personal Mods and Patches
description: Create personal mods and patches for Stardew Valley collections. Learn how to build standalone mods or patches that modify existing mods and preserve changes through collection updates.
keywords: [personal mods, custom mods, patches, personal patches, load order, Vortex patches, manifest.json, custom modding]
tags: [customization, personal-mods, patches, modding]
---

# Creating Personal Mods

*Last updated:* 2026-01-15  
*Applies to Stardew Valley:* 1.6.15+

{% hint style="danger" %}
If you're using a mod manager like Vortex, avoid making direct changes to mods in your Mods folder. Mod managers manage these files, and your changes can be lost when the manager updates or redeploys mods. Creating a separate personal mod or patch keeps your changes protected and makes it easy to manage them.
{% endhint %}

Want to create your own custom mods or patches? Personal mods and patches allow you to customize your game and modify existing mods while keeping your changes safe through collection updates. This guide will walk you through creating standalone personal mods and personal patches that work alongside your collection, ensuring your personalizations persist even when the collection updates.

Personal mods and patches keep your customizations safe through collection updates. **Personal mods** are standalone changes to the game, and you can add them through your mod manager like other mods to keep them managed alongside your collection! When you create a **personal patch** that applies on top of an existing mod, you get the best of both worlds: the original mod can be updated normally (through collection updates or manual updates), and your custom changes stay safe in your **personal patch**.

---

## Personal Mod vs Personal Patch

Understanding the difference helps you choose the right approach:

**Personal Mod:**
- A standalone mod that changes some aspect of the game
- Has its own `manifest.json` file
- May be coded in C# or use an existing framework (like Content Patcher) to alter the game without C#
- Works independently or alongside other mods
- Examples: New content mods, custom gameplay features, standalone modifications

**Personal Patch:**
- A folder structure that matches an existing mod's structure
- Adds to or overwrites existing files from the original mod
- Typically doesn't have its own `manifest.json` (or uses a minimal one)
- Overrides specific files from the original mod when loaded after it
- Examples: Tweaking textures, modifying content files, fixing issues in existing mods

If you're modifying files from an existing mod, use a **personal patch**. If you're creating something new or standalone, use a **personal mod**. Both approaches keep your changes safe through collection updates!

---

## Creating Personal Mods

Personal mods are standalone mods you create from scratch. They have their own `manifest.json` file and can be coded in C# or use frameworks like Content Patcher to alter the game without C#. For C# mods, you'll need to compile them first. For Content Patcher mods, ensure your `content.json` is properly formatted. See the [Stardew Valley Modding Index](https://stardewvalleywiki.com/Modding:Index) for detailed guides on creating C# mods, content packs, and more.

### Step 1: Create Your Mod Structure

1. Create a new folder for your mod
2. Add a `manifest.json` file with your mod's metadata (UniqueID, Name, Author, Version, etc.)
3. Add your mod's content files (C# code, Content Patcher files, assets, etc.)

**Example `manifest.json` structure:**

```json
{
  "Name": "My Personal Mod",
  "Author": "YourName",
  "Version": "1.0.0",
  "Description": "A personal mod that adds custom features",
  "UniqueID": "YourName.MyPersonalMod",
  "UpdateKeys": []
}
```

See the [Stardew Valley Modding Index](https://stardewvalleywiki.com/Modding:Index) for complete manifest.json documentation.

### Step 2: Add to Your Mod Manager

You can add your personal mod to Vortex in two ways:

**Option A: Compress as ZIP**
1. Compress the folder as a ZIP file
2. Add it to Vortex like any other mod (drag and drop the ZIP file, or use **Add Mod from File**)

**Option B: Use Add Custom Mod Button**
1. Install the [Add Custom Mod Button](https://www.nexusmods.com/site/mods/863) add-on for Vortex
2. Use the **"Add Custom Mod"** button in Vortex to add the folder directly

### Step 3: Deploy

Click **Deploy** in Vortex to apply your changes.

---

## Creating Personal Patches

Personal patches allow you to modify existing mods without editing the original mod files. A personal patch is a folder structure that matches an existing mod's structure and adds to or overwrites existing files. This is useful for making tweaks, fixing issues, or customizing content while keeping the original mod intact. Personal patches override specific files from the original mod when loaded after it.

### Step 1: Create Your Patch Folder Structure

The folder structure must exactly match what is in your mods folder. For example, if you are patching `ModName/[CP] ModName/content.json`, that is the folder structure you would need to create:

- The folder names and paths must match the original mod exactly
- Example: If patching `[CP] ModName/content.json`, create `[CP] ModName/content.json` in your patch
- If you're patching multiple mods, you can include multiple top-level folders in your patch (if you do not include manifests)

### Step 2: Add Your Files

Place your modified files in the appropriate folders. A patch may contain multiple top level folders if you do not include manifests. Only include the files you're modifying—you don't need to copy the entire mod. The patch will override the original files when loaded after the original mod.

### Step 3: Add to Your Mod Manager

You can add your patch to Vortex in two ways:

**Option A: Compress as ZIP**
1. Compress the top level folder as a ZIP file
2. Add it to Vortex like any other mod (drag and drop the ZIP file, or use **Add Mod from File**)

**Option B: Use Add Custom Mod Button**
1. Install the [Add Custom Mod Button](https://www.nexusmods.com/site/mods/863) add-on for Vortex
2. Use the **"Add Custom Mod"** button in Vortex to add the folder directly

### Step 4: Set Load Order

In Vortex, go to **Mods > Manage Rules** and set your patch to load **AFTER** the mod it's patching. This ensures your modified files override the original mod's files.

### Step 5: Deploy

Click **Deploy** in Vortex to apply your changes.
---

## Best Practices

- **Test thoroughly** before committing to changes
- **Keep backups** of working configurations
- **Document your changes** for future reference

---

## See Also

- [How to Customize Collections](index.md) - Main customization guide
- [Creating Collections](creating-collections.md) - For creating your own collections
- [Troubleshooting & FAQ](../Troubleshooting/index.md) - If something goes wrong
