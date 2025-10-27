# Combining Collections

> 📂 **Docs** / [Start](/start.md) / **Combining Collections**


*Last updated:* 2025-09-10  
*Applies to Stardew Valley:* **1.6.15+**

> 📖 This guide will be available right on the Nexus Collection page soon!

**Warning:** If your mine entrance is missing, enable **Original Mine Entrance** in GMCM under *Stardew Valley Expanded*.

You can combine **Stardew Valley VERY Expanded (svVe)** with one or both **Aesthetic Valley** collections for a custom look and feel.  
Always install them **into the same Vortex profile** and follow the conflict resolution steps below.

---

## General Rules

1. In **Vortex → Rules Manager**, all **configuration and content patch mods** should load **after** other mods they modify.  
2. If two configuration files conflict, **the one for your chosen recolor/theme should load last**.
3. **Installation Order:** When combining collections, install the "dominant" Aesthetic Valley collection last, or reinstall its included configuration file at the end to ensure it takes priority.

### Optional Mods Strategy

For easiest combining, **only download one set of 'optional mods'**. This method is **recommended when combining 2 or 3 collections created by JennaJuffuffles**.

> **Note:** 'Optional mods' can easily be added later by accessing any collection's poster in the collection view → mods tab → set required dropdown to "Recommended".

**Custom Selections:** While you can pick and choose optional mods individually, review your configuration files afterwards as this may introduce unexpected behavior.

**Configuration Management:** For easier configuration management when combining collections, use the [Collection Configuration Manager FOMOD](https://www.nexusmods.com/stardewvalley/mods/20870?tab=files) available on Nexus. This tool provides a wizard interface that allows you to:

- Completely customize which configuration files are deployed
- Remove premade configurations you'd prefer to manage yourself

**To use the Configuration Manager:**
- Disable the included configuration mods from your collection before using this tool
- Run the FOMOD installer to select your desired configurations (Works in Vortex, NMA, and MO2)

> **Need help with custom configurations?** See our [Personalization & Custom Configurations](/personalization.md) guide for detailed instructions on protecting your settings.

**Conflict Warnings:** If optional mods that the collection creator has flagged as conflicting are enabled, Vortex will show a warning notification. Due to a Vortex display error, this warning may appear up to 6 times per conflict, which is confusing to see! This is different from a rules conflict and simply indicates that one mod of the pair should be disabled.

### Known Mod Incompatibilities

When combining collections, you may encounter these specific incompatibilities. **Disable one mod from each conflicting pair:**

**Interface Conflicts:**
- `(Compat) EventLookup for Overgrown Flowerly UI` ❌ `(Compat) DaisyNiko's Earthy Interface` 
- `(Compat) Overgrown Flowery` ❌ `(Compat) DaisyNiko's Earthy Interface`
- `(Compat) Overgrown Flowery` ❌ `The Witchs Handmirror - Green`
- `(Compat) Overgrown Flowery` ❌ `(Compat) Fashion Sense UI for DaisyNiko's Earthy Interface - FashionSense UI`
- `(Compat) Overgrown Flowery` ❌ `(Compat) Fashion Sense UI for DaisyNiko's Earthy Interface - FashionSense UI`
- `(Compat) Overgrown Flowery` ❌ `(Compat) Font Settings for DaisyNiko's Earthy Interface`

**Visual/Recolor Conflicts:**
- `Overgrown Flowery Interface [CP]` ❌ `DaisyNiko's Earthy Recolour [CP]`
- `Starblue Valley Unofficial` ❌ `DaisyNiko's Earthy Recolour [CP]`

**Farm Map Conflicts:**
- `Lnh's MiNi Farm [CP]` ❌ `Grandpa's Farm` ❌ `Immersive Farm 2k Remastered` 

**Building Conflicts:**
- `Tanga Forest Buildings [CP]` ❌ `Medieval Buildings [CP]`
- `Sunroom Greenhouse [CP]` ❌ `Aimon's Fancy Greenhouse [CP]`

**Tool/Equipment Conflicts:**
- `Skell's Flowery Tools [CP]` ❌ `Grandpa's Tools`
- `Squishi's Rideable Deer [CP]` ❌ `Elle's Cuter Horses`

*Choose the mod that best fits your desired aesthetic when resolving conflicts.*

**Greenhouses:** When using Aesthetic Valley collections, remember that only one greenhouse can be used. This includes if using farms from Stardew Valley Exapnded, each of which has a greenhouse built in. This can be disabled in the configuration if desired. So keep this in mind if you decide to mix-and-match your collection options!

---

## Aesthetic Valley paired with Stardew Valley VERY Expanded

**Disable** all but one in Vortex:
- Immersive Farm 2 Remastered, LnH's MiNi Farm, Grandpa's Farm

**Configure** in GMCM:
- If using Frontier Farm, Immersive Farm 2 Remastered, or Grandpa's Farm, disable the Greenhouse option (the Configuration Manager will handle this automatically.)

**Recommended**:
- Review recommended files for compatability options (labeled with "Compat").

---

## Quick Links

- [Start Page](/start.md)  
- [Installation Guide](/install.md)  
- [Manual Installation Guide](/manual-install.md)  
- [Updating Collections](/updating.md)  
- [Combining Collections](/combining.md)  
- [Personalization & Custom Configurations](/personalization.md)  
- [Keybinds & Controllers](/keybinds.md)  
- [Troubleshooting](/troubleshooting.md)  
- [FAQ & Known Issues](/faq-and-known-issues.md)  