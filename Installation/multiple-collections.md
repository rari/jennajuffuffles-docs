---
title: Installing Multiple Collections Together
description: Combine multiple Stardew Valley mod collections safely. Learn how to install Aesthetic Valley with svVe, resolve conflicts, and manage optional mods strategy.
keywords: [combining collections, multiple collections, collection conflicts, optional mods, Aesthetic Valley, svVe, conflict resolution, mod incompatibilities, Vortex rules]
tags: [combining-collections, conflicts, optional-mods, compatibility]
---

# Installing Multiple Collections

*Last updated:* 2026-01-15  
*Applies to Stardew Valley:* 1.6.15+

{% hint style="warning" %}
If your mine entrance is missing, enable "Original Mine Entrance" in GMCM under Stardew Valley Expanded.
{% endhint %}

You can combine Stardew Valley VERY Expanded (svVe) with any Aesthetic Valley collection (Fairycore, Witchcore) for a custom look and feel. Always install them into the same Vortex profile.

---

## Table of Contents

- [The Key Principle](#the-key-principle)
- [When Conflicts Happen](#when-conflicts-happen)
- [Configuration Tips](#configuration-tips)
- [Specific Conflicts Reference](#specific-conflicts-reference)

---

## The Key Principle

When combining collections, here's what you need to know:

**Aesthetic Valley optional mods:**
- **For easiest installation:** Pick one theme (Fairycore or Witchcore) for your optional mods.
- **You can absolutely mix and match:** If you install optional mods from both themes, Vortex will show conflicts so you know what to choose between. You'll just need to resolve more conflicts.
- **svVe optional mods:** These can always be installed alongside Aesthetic Valley collections—they don't conflict.

**Farm maps:**
- Only enable **one** farm map at a time. Multiple farm maps will cause crashes and save corruption.

**Don't worry about getting everything perfect the first time!** You can add optional mods later from any collection's Mods tab (set the filter to "Recommended") to experiment with different combinations after your initial installation.

---

## When Conflicts Happen

If you follow the recommendation to install optional mods from one Aesthetic Valley collection, you'll encounter very few conflicts. Collections are pre-configured to handle most conflicts automatically.

If you choose to mix and match optional mods from multiple collections, or if you see conflict notifications, see [Troubleshooting & FAQ](../Troubleshooting/index.md) for detailed guidance on:
- [Vortex Troubleshooting](../Troubleshooting/vortex-troubleshooting.md) - Understanding notifications and managing load order rules
---

## Configuration Tips
**In Manage Rules:**
- Configuration and content patch mods should load **after** the mods they modify in Vortex's Manage Rules. This ensures your configuration changes actually apply.

**If you're using the Collection Configuration Manager FOMOD:**
- The FOMOD automatically handles greenhouse configuration and helps avoid conflicts. See [Using the Collection Configuration Manager FOMOD](../Customization/index.md#using-the-collection-configuration-manager-fomod) for details.

**If you're not using the FOMOD:**
- Many farm maps include a greenhouse you can disable in configuration. If you're using a farm map with a built-in greenhouse, disable standalone greenhouse mods.

For more advanced customization, including load order management, see:
- [Manage Rules (Load Order)](../Troubleshooting/manage-rules.md) - Detailed load order guidance

---

## Specific Conflicts Reference (Included for Manual Installers)

These mods are known to conflict when combined. You must disable one mod from each conflicting pair.

**Interface Conflicts:**

These mods modify the game's interface and cannot work together:
- (Compat) EventLookup for Overgrown Flowerly UI ❌ (Compat) DaisyNiko's Earthy Interface
- (Compat) Overgrown Flowery ❌ (Compat) DaisyNiko's Earthy Interface
- (Compat) Overgrown Flowery ❌ The Witchs Handmirror - Green
- (Compat) Overgrown Flowery ❌ (Compat) Fashion Sense UI for DaisyNiko's Earthy Interface - FashionSense UI
- (Compat) Overgrown Flowery ❌ (Compat) Font Settings for DaisyNiko's Earthy Interface

**Visual/Recolor Conflicts:**

These mods change the game's color scheme and visual style. Only one can be active:
- Overgrown Flowery Interface [CP] ❌ DaisyNiko's Earthy Recolour [CP]
- Starblue Valley Unofficial ❌ DaisyNiko's Earthy Recolour [CP]

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
Greenhouses are a special case. Only one greenhouse can be active. Many farm maps include a greenhouse you can disable in configuration. If you're using a farm map with a built-in greenhouse, disable standalone greenhouse mods.
{% endhint %}

**Tool/Equipment Conflicts:**

These mods replace the same tools or equipment. Only one can be active:
- Skell's Flowery Tools [CP] ❌ Grandpa's Tools
- Squishi's Rideable Deer [CP] ❌ Elle's Cuter Horses

---

## See Also

- [How to Customize Collections](../Customization/index.md) - For customizing your combined setup
- [About the Collections](../About/index.md) - Learn about individual collections
- [Troubleshooting & FAQ](../Troubleshooting/index.md) - For issues when combining collections
- [New Player Install Instructions](index.md) - If you're just getting started
