---
title: Customizing Stardew Valley Mod Collections
description: Personalize your Stardew Valley mod collections. Learn how to add mods, create custom configurations, and preserve personalizations through collection updates.
keywords: [personalization, custom configurations, adding mods, custom patches, private collections, GMCM, mod customization, collection personalization]
tags: [personalization, customization, mods, configuration, patches]
---

# How to Customize Collections

*Last updated:* 2026-01-15  
*Applies to Stardew Valley:* 1.6.15+

Want to make your Stardew Valley experience truly your own? This guide will show you how to customize your collections by adding or disabling mods, adjusting configurations, and making personal tweaks - all while keeping your customizations safe through collection updates!

**Need more advanced customization?**
- **[Creating Personal Mods](creating-personal-mods.md)** - Create custom mods and patches
- **[Creating Collections](creating-collections.md)** - Create your own mod collections

---

## Table of Contents

- [Overview](#overview)
- [Adding and Disabling Mods](#adding-and-disabling-mods)
- [Adjusting Configurations](#adjusting-configurations)
- [Using the Collection Configuration Manager FOMOD](#using-the-collection-configuration-manager-fomod)
- [What Configs Actually Change](#what-configs-actually-change)
- [When Mods Cause Trouble](#when-mods-cause-trouble)

---

## Overview

Customization allows you to personalize your collection while maintaining compatibility with collection updates. You can:

* Add or disable mods from your collection
* Customize mod configurations (settings, keybinds, etc.)
* Adjust UI and visual preferences
* Make gameplay tweaks and adjustments

The best part? When done correctly, your customizations will persist even when the collection updates!

---

## Adding and Disabling Mods

{% hint style="info" %}
Always read the mod page before adding or disabling any mod. Mod pages contain crucial information about compatibility, conflicts, and requirements.
{% endhint %}

You can absolutely add or disable mods from your collection! However, it's important to be informed about the mods you're working.

### Learning About Mods in Your Collection

To learn more about a mod before removing it:

1. In Vortex, go to the **Mods** tab
2. Right-click on any mod in the collection
3. Select **"View on Nexus Mods"** to open the mod's page
4. Read the mod description, requirements, and compatibility notes

### Understanding Mod Conflicts

Most mods will mention if they conflict with major mods in the collection (like Stardew Valley Expanded). When adding mods:

- **Check for conflicts** - Read the mod page for known incompatibilities
- **Similar functionality** - Adding any mod that does something similar to an existing mod (like managing time, or replacing portraits) will require that the existing mod in the collection be disabled
- **Vortex alerts** - Vortex may alert you if a required mod is disabled, but you should be able to still deploy and play normally
- **Be cautious** - Test thoroughly and be prepared to disable conflicting mods if needed. Check the [SMAPI log](../Troubleshooting/your-smapi-log.md) if you encounter issues

---

## Adjusting Configurations

You can customize mod settings and configurations in two main ways:

### In-Game Configuration (GMCM)

Many mods support **Generic Mod Config Menu (GMCM)**, which provides an in-game menu for adjusting mod settings:

- Press the configured hotkey (usually shown in the mod's description) to open the config menu
- Adjust settings directly in-game without editing files
- Changes are saved automatically
- Some mods may require restarting the game for changes to take effect

### Backing Up Configuration Files

Before updating your collection or making major changes, it's important to back up your configuration files. This ensures you can restore your settings if something goes wrong during updates or modifications.

#### Using Sync Mod Configurations

Vortex provides a built-in feature to backup and restore your mod configurations:

1. In Vortex, locate the **"Sync Mod Configurations"** button
2. Click the button to create a backup of your current configuration files
3. This will save your current configurations and prevent them from being lost

The Sync Mod Configurations feature creates a virtual "configuration mod" in Vortex that contains a snapshot of your current config files. When you update your collection or mods, you can use this backup to restore your personal settings so your customizations stay intact.

{% hint style="danger" %}
The Sync Mod Configurations feature may occasionally attempt to back up `smapi-internal` in error. See [Sync Mod Configurations Backs Up smapi-internal](../Troubleshooting/known-issues.md#sync-mod-configurations-backs-up-smapi-internal) for the fix.
{% endhint %}

---

## Using the Collection Configuration Manager FOMOD

The Collection Configuration Manager FOMOD allows you to customize which configuration files are deployed and remove premade configurations you don't need. This is especially useful when combining multiple collections or when you want more control over your configuration setup.

**How to use it:**

1. Install the **Collection Configuration Manager** from [Nexus Mods](https://www.nexusmods.com/Core/Libs/Common/Widgets/DownloadPopUp?id=151099&game_id=1303&nmm=1)
2. The FOMOD installer will open during installation, allowing you to:
   - Select which configuration files to deploy
   - Remove premade configurations you don't need
   - Customize your configuration setup

**Automatic greenhouse configuration:**

The FOMOD includes automatic handling for greenhouse configuration. When you select your farm map and greenhouse preferences, it will automatically disable conflicting greenhouse options to prevent conflicts. This is particularly helpful when combining collections with different farm maps and greenhouse mods.

{% hint style="info" %}
If you're combining multiple collections, using the FOMOD can help you avoid configuration conflicts and ensure your preferred settings are applied correctly.
{% endhint %}

---

## What Configs Actually Change

Configuration files control:
- **Mod settings** - How mods behave (automation ranges, display options, etc.)
- **Keybinds** - Keyboard shortcuts and controller mappings
- **Visual preferences** - UI scaling, color schemes, display options
- **Gameplay tweaks** - Difficulty settings, quality-of-life features

Most configs can be changed safely without breaking saves. However, some changes can affect save compatibility.

---

## When Mods Cause Trouble

Some changes can cause major issues with existing saves. Adding or disabling major expansion mods, NPC mods, farm map mods, or core gameplay mods may require special cleanup tools or starting a new save.

{% hint style="info" %}
Test changes on a test save before applying to your main save. For detailed information about installing collections to existing saves and the cleanup tools needed, see [Installing Collections to Existing Saves](../Installation/installing-to-existing-saves.md).
{% endhint %}

---

## See Also

- [Troubleshooting & FAQ](../Troubleshooting/index.md) - For issues with personalizations
- [Creating Collections](creating-collections.md) - For creating your own collections
- [Installing Multiple Collections](../Installation/multiple-collections.md) - For combining collections
