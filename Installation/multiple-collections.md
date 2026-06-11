---
title: Installing Multiple Collections Together
description: Combine multiple Stardew Valley mod collections safely. Learn how to install Aesthetic Valley with svVe, resolve conflicts, and manage optional mods strategy.
keywords: [combining collections, multiple collections, collection conflicts, optional mods, Aesthetic Valley, svVe, conflict resolution, mod incompatibilities, Vortex rules]
tags: [combining-collections, conflicts, optional-mods, compatibility]
---

# Installing Multiple Collections

*Last updated:* 2026-06-10  
*Applies to Stardew Valley:* 1.6.15+

When installing multiple collections by JennaJuffuffles, add them to the same Vortex profile.

---

## Table of Contents

- [The Key Principle](#the-key-principle)
- [When Conflicts Happen](#when-conflicts-happen)
- [Important Configuration Tips](#important-configuration-tips)
- [Specific Conflicts Reference (Included for Manual Installers)](#specific-conflicts-reference-included-for-manual-installers)

---

## The Key Principle

When combining collections, here's what you need to know:

- **Single profile:** Install one collection as normal, then select "Current profile" at the bottom of the first pop-up when installing the next.
- **JennaJuffuffles collections are designed to work together** within that same profile.
- **Collections from other creators are not designed to stack** with these packs.
- **Adding extra mods is generally fine**, but some combinations may produce unexpected results.

{% hint style="danger" %}
**Aesthetic Valley Fairycore and Aesthetic Valley Witchcore are now mutually exclusive.**

Do **not** install both in the same profile.
{% endhint %}

### Extras Collections

**Aesthetic Valley Fairycore Extra Textures**
- Recommended if using Fairycore
- Does not require Fairycore

**Aesthetic Valley Witchcore Extra Textures**
- Recommended if using Witchcore
- Does not require Witchcore

**Farm maps:**
- Only enable **one** farm map at a time. Multiple farm maps will cause crashes and save corruption.

---

## When Conflicts Happen

If you follow the guidance above, you'll encounter very few conflicts. Collections are pre-configured to handle most conflicts automatically.

If you add additional mods or see conflict notifications, see [Troubleshooting & FAQ](../Troubleshooting/index.md) for detailed guidance on:
- [Vortex Troubleshooting](../Troubleshooting/vortex-troubleshooting.md) - Understanding notifications and managing load order rules

---

## Important Configuration Tips
{% hint style="warning" %}
If your mine entrance is missing, right-click Stardew Valley VERY Configured - Stardew Valley VERY Expanded in the Mods panel and select Reinstall. This is a tell-tale sign configuration did not apply as expected!
{% endhint %}

**In Manage Rules:**
- Configuration and content patch mods should load **after** the mods they modify in Vortex's Manage Rules. This ensures your configuration changes actually apply. **Never use Suggested rules**!

**If you're using the Collection Configuration Manager FOMOD:**
- Disable all Stardew Valley VERY Configured mods for your collections.
- The FOMOD automatically handles greenhouse configuration and helps avoid conflicts. See [Using the Collection Configuration Manager FOMOD](../Customization/index.md#using-the-collection-configuration-manager-fomod) for details.

**If you're not using the FOMOD:**
- Many farm maps include a greenhouse you can disable in configuration. If you're using a farm map with a built-in greenhouse, disable standalone greenhouse mods.

For more advanced customization, including load order management, see:
- [Manage Rules (Load Order)](../Troubleshooting/vortex-troubleshooting.md#3-manage-rules) - Detailed load order guidance

---

## Specific Conflicts Reference (Included for Manual Installers)

These mods are known to conflict when combined. You must disable one mod from each conflicting pair.

**Farm Map Conflicts:**

{% hint style="warning" %}
Never enable multiple farm maps simultaneously. Disable all farm maps except the one you want to use.
{% endhint %}

Only one farm map can be active at a time:
- Lnh's MiNi Farm [CP] ❌ Grandpa's Farm ❌ Immersive Farm 2k Remastered ❌ Frontier Farm

**Building Conflicts:**

These mods replace the same buildings. Only one set can be active:
- Tanga Forest Buildings [CP] ❌ Medieval Buildings [CP]
- Sunroom Greenhouse [CP] ❌ Aimon's Fancy Greenhouse [CP]

{% hint style="danger" %}
Greenhouses are a special case. Only one greenhouse can be active and having both active will result in neither one being loaded. Many farm maps include a greenhouse you can disable in configuration. If you're using a farm map with a built-in greenhouse, either disable standalone greenhouse mods or disable the farm's greenhouse! Doing this mid-playthrough may require some clean-up.
{% endhint %}

**Tool/Equipment Conflicts:**

These mods replace the same tools or equipment. Only one can be active:
- Skell's Flowery Tools [CP] ❌ Grandpa's Tools
- Squishi's Rideable Deer [CP] ❌ Elle's Cuter Horses

**Interface Conflicts:**

These mods modify the game's interface and cannot work together:
- Overgrown Flowery Interface [CP] ❌ DaisyNiko's Earthy Recolour [CP]
- Starblue Valley Unofficial ❌ DaisyNiko's Earthy Recolour [CP]
- (Compat) EventLookup for Overgrown Flowerly UI ❌ (Compat) DaisyNiko's Earthy Interface
- (Compat) Overgrown Flowery ❌ (Compat) DaisyNiko's Earthy Interface
- (Compat) Overgrown Flowery ❌ The Witchs Handmirror - Green
- (Compat) Overgrown Flowery ❌ (Compat) Fashion Sense UI for DaisyNiko's Earthy Interface - FashionSense UI
- (Compat) Overgrown Flowery ❌ (Compat) Font Settings for DaisyNiko's Earthy Interface

---

## See Also

- [How to Customize Collections](../Customization/index.md) - For customizing your combined setup
- [About the Collections](../About/index.md) - Learn about individual collections
- [Troubleshooting & FAQ](../Troubleshooting/index.md) - For issues when combining collections
- [New Player Install Instructions](index.md) - If you're just getting started
