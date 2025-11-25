---
description: Guide to combining Stardew Valley VERY Expanded with Aesthetic Valley collections. Learn about conflict resolution, optional mods strategy, and known incompatibilities.
keywords: combining collections, collection conflicts, optional mods, Aesthetic Valley, svVe, conflict resolution, mod incompatibilities, Vortex rules
tags: [combining collections, conflicts, optional mods, compatibility]
---

# Combining Collections

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* 1.6.15+

> Warning: If your mine entrance is missing, enable "Original Mine Entrance" in GMCM under Stardew Valley Expanded.

You can combine Stardew Valley VERY Expanded (svVe) with any Aesthetic Valley collection (Fairycore, Witchcore) for a custom look and feel. Always install them into the same Vortex profile and follow the conflict resolution steps below.

---

## Table of Contents

- [General Rules](#general-rules)
- [Known Mod Incompatibilities](#known-mod-incompatibilities)
- [Aesthetic Valley + svVe](#aesthetic-valley--svve)

---

## General Rules

1. In Vortex > Rules Manager, all configuration and content patch mods should load after the mods they modify.
2. If two configuration files conflict, the one for your chosen recolor/theme should load last.
3. Skip or disable compat that is not relevant to you!
4. Only have the farm mod you are using enabled.

### Optional Mods Strategy

When combining svVe with any Aesthetic Valley collection:
- **svVe optional mods:** Can always be installed when combining with Aesthetic Valley collections.
- **Aesthetic Valley optional mods:** Only install optional mods from **one** Aesthetic Valley collection to avoid conflicts.
- **Farm optional mods:** Only install optional mods from **one** farm to avoid conflicts.

- Optional mods can be added later from any collection's Mods tab by setting the filter to "Recommended".
- If you customize optional mods individually, review configurations afterwards to avoid unexpected behavior.

### Configuration Management
Use the Collection Configuration Manager FOMOD to customize which configuration files are deployed and remove premade configurations you don’t need:
- Disable included configuration mods in your collection first
- Run the FOMOD installer and select desired configurations (works in Vortex, NMA, MO2)

See: [Personalization & Custom Configurations](../Guides/personalization.md)

> Conflict warnings in Vortex indicate one mod of a conflicting pair should be disabled. They may appear multiple times due to a display quirk.

---

## Known Mod Incompatibilities
Disable one mod from each conflicting pair when combining collections.

### Interface Conflicts
- (Compat) EventLookup for Overgrown Flowerly UI ❌ (Compat) DaisyNiko's Earthy Interface
- (Compat) Overgrown Flowery ❌ (Compat) DaisyNiko's Earthy Interface
- (Compat) Overgrown Flowery ❌ The Witchs Handmirror - Green
- (Compat) Overgrown Flowery ❌ (Compat) Fashion Sense UI for DaisyNiko's Earthy Interface - FashionSense UI
- (Compat) Overgrown Flowery ❌ (Compat) Font Settings for DaisyNiko's Earthy Interface

### Visual/Recolor Conflicts
- Overgrown Flowery Interface [CP] ❌ DaisyNiko's Earthy Recolour [CP]
- Starblue Valley Unofficial ❌ DaisyNiko's Earthy Recolour [CP]

### Farm Map Conflicts
- Lnh's MiNi Farm [CP] ❌ Grandpa's Farm ❌ Immersive Farm 2k Remastered (Only one farm map option should ever be active, including Frontier Farm)

### Building Conflicts
- Tanga Forest Buildings [CP] ❌ Medieval Buildings [CP]
- Sunroom Greenhouse [CP] ❌ Aimon's Fancy Greenhouse [CP]

### Tool/Equipment Conflicts
- Skell's Flowery Tools [CP] ❌ Grandpa's Tools
- Squishi's Rideable Deer [CP] ❌ Elle's Cuter Horses

> Choose the option that fits your desired aesthetic.

Greenhouses: only one greenhouse can be active. Many farm maps include a greenhouse you can disable in configuration.

---

## Aesthetic Valley + svVe

Disable any unused farms in Vortex (no more than one active):
- Immersive Farm 2 Remastered, LnH's MiNi Farm, Grandpa's Farm, Frontier Farm

Configure in GMCM:
- If using Frontier Farm, Immersive Farm 2 Remastered, or Grandpa's Farm, disable the Greenhouse option (the Configuration Manager handles this automatically).

Recommended:
- Review "Compat" files for additional compatibility options.

---

## See Also

- [Personalization & Custom Configurations](../Guides/personalization.md) - For customizing your combined setup
- [Stardew Valley VERY Expanded Overview](Stardew%20Valley%20VERY%20Expanded/overview.md) - Learn about svVe
- [Aesthetic Valley Collections](aesthetic-valley.md) - Learn about Aesthetic Valley
- [Troubleshooting & FAQ](../Guides/troubleshooting.md) - For issues when combining collections

