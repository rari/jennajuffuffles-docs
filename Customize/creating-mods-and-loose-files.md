# Creating Mods and Loose Files
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

{% hint style="danger" %}
If you use a mod manager such as Vortex, avoid editing mods directly in your Mods folder. The manager owns those files, and your edits can be lost when it updates or redeploys. A separate mod, or a folder of loose files, keeps your changes protected.
{% endhint %}

A mod can change the game, or change files and assets added by another mod. Keep that work in its own folder so a collection update does not wipe it.

Loose files are real files whose paths match an existing mod. Build that folder, include only the files you are replacing, and set it to load after that mod in Vortex. Vortex deploys your copies on top, and they win the file conflict. The original mod's files stay in its own folder.

## Creating a Mod

A mod has its own `manifest.json`. SMAPI loads it. It can change the game, or change files and assets from another mod. Learn how to make one from these guides.

**Stardew Valley Wiki**

The [Modding Index](https://stardewvalleywiki.com/Modding:Index) is the main hub. From there, creating mods splits into content packs and C# SMAPI mods.

- [Creating content packs](https://stardewvalleywiki.com/Modding:Content_packs)
- [Content Patcher](https://stardewvalleywiki.com/Modding:Content_Patcher)
- [Modder Guide: Get Started](https://stardewvalleywiki.com/Modding:Modder_Guide/Get_Started) for C# mods
- [Modder Guide: Release](https://stardewvalleywiki.com/Modding:Modder_Guide/Release) for publishing

**Stardew Modding Wiki**

[Getting Started](https://stardewmodding.wiki.gg/wiki/Getting_Started) is for people making mods. [Tutorials](https://stardewmodding.wiki.gg/wiki/Category:Tutorials) is the tutorial index.

**Content Patcher on GitHub**

The [author guide](https://github.com/Pathoschild/StardewMods/blob/develop/ContentPatcher/docs/author-guide.md) starts from the pack structure and covers `manifest.json`, `content.json`, actions, and conditions. The [docs index](https://github.com/Pathoschild/StardewMods/blob/develop/ContentPatcher/docs/README.md) lists the rest of the docs. [Tokens](https://github.com/Pathoschild/StardewMods/blob/develop/ContentPatcher/docs/author-guide/tokens.md) is the token reference.

## Loose Files

Loose files are real files on disk. The folder structure matches the mod you are changing. Include only the files you are replacing.

- Paths match the existing mod
- Adds or replaces specific files from that mod
- Often has no `manifest.json` of its own (or uses a minimal one)
- Wins the Vortex file conflict when set to load after that mod
- Examples: tweaking textures, modifying content files, fixing issues in existing mods

### Create the folder structure

The folder structure must exactly match what is in your mods folder. If you are replacing `ModName/[CP] ModName/content.json`, create that same path:

- The folder names and paths must match the original mod exactly.
- Example: To replace `[CP] ModName/content.json`, create `[CP] ModName/content.json` in your loose files folder.
- If you are replacing files in multiple mods, you can include multiple top-level folders (if you do not include manifests).

### Add your files

Place your modified files in the matching folders. Include only the files you are replacing. A loose files folder may contain multiple top-level folders if you do not include manifests.

## Add and deploy in Vortex

Use these steps for a mod or for loose files.

{% stepper %}
{% step %}
#### Add it in Vortex

Use one of these options.

**Option A: Compress as ZIP**

1. Compress the top-level folder as a ZIP file (right-click the folder).
2. Add it to Vortex like any other mod (drag and drop the ZIP file, or use **Add Mod from File**).

**Option B: Use Add Custom Mod Button**

1. Install the [Add Custom Mod Button](https://www.nexusmods.com/site/mods/863) add-on for Vortex.
2. Use the **Add Custom Mod** button in Vortex to add the folder directly.
{% endstep %}

{% step %}
#### Set load order for loose files

For loose files, go to **Mods > Manage Rules** and set them to load **after** the mod they replace. 
{% endstep %}

{% step %}
#### Deploy in Vortex

Click **Deploy** in Vortex to apply your changes.
{% endstep %}
{% endstepper %}

## Sharing on Nexus

{% hint style="info" %}
Nexus may update its guidelines. This site is not the authority. Read the full rules and guidelines on Nexus before you upload: the [Terms of Service](https://help.nexusmods.com/article/18-terms-of-service) and the [File Submission Guidelines](https://help.nexusmods.com/article/28-file-submission-guidelines).
{% endhint %}

Creating a mod and releasing it are separate steps. Before you upload, follow [Modder Guide: Release](https://stardewvalleywiki.com/Modding:Modder_Guide/Release).

## Best Practices

- Test thoroughly before committing to changes.
- Keep backups of working versions.
- Document your changes for future reference.

## Related

- [Adding and Disabling Mods](adding-and-disabling-mods.md)
- [Adjusting Configurations](adjusting-configurations.md)
- [Creating a Collection](../Collection-Creation/creating-a-collection.md) 
- [Your SMAPI Log](../Troubleshooting/your-smapi-log.md)
