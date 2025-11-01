# FAQ & Known Issues

> 📂 Docs / Getting Started / FAQ & Known Issues

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* **1.6.15+**

This page addresses the most common questions and issues players encounter with Stardew Valley VERY Expanded (svVe) and companion collections.

---

## Getting Started FAQs

**Do I need the optional mods?**
> Yes. While some mods are marked as "optional" to simplify collection stacking, you should install them when using a single collection. These include essential interface improvements, map enhancements, and additional content. Expansions are included as optional due to player feedback; they're curated for a high-quality experience.

**Should I update individual mods myself?**
> No. Always wait for collection updates to ensure compatibility and prevent conflicts.

**Can I combine your collections?**
> Yes. The Aesthetic Valley collections are designed to work alongside svVe. See Combining Collections: [Combining Collections](Collections/combining-collections.md)

**First-time players**
> It's fine to start with svVe, though it's large. Vanilla first is recommended but not required.

**Co-op**
> All players should have matching mods and configurations for the best experience. Consider using a multiplayer manager to keep versions aligned.

**Where to download**
> Use Nexus Mods (official source). Premium enables one-click; avoid unauthorized mirrors.

---

## Gameplay FAQs

**Community Center cutscene won't trigger**
> Requirements (vanilla): Enter Pelican Town from the Bus Stop; Spring 5+; 8:00–13:00; sunny (not festival); host must trigger in multiplayer.

**Rusty/Sewer Key changes in SVE**
> Due to SVE changes, Gunther no longer provides the Rusty Key. Reach 5 hearts with Marlon; he will mail the key in a cutscene (see SVE wiki for details).

**Minecart blocks the mine entrance**
> GMCM: SVE → Original Mine Entrance. Often indicates configuration merge issues.

**Missing recipes in crafting menu**
> Better Crafting groups recipes. Check other categories or "Show All/Uncategorized".

**Can't exit house / corrupted farm map**
> Occurs if your farm map mod is disabled or fails to load. Re-enable it and Deploy. Maps can't be switched mid-save without special tools like [Easy Farm Switcher](https://www.nexusmods.com/stardewvalley/mods/16873).

---

## Setup & Customization FAQs

**Can I add more mods?**
> Yes. These collections are solid bases for customization. Test additions individually and review compatibility notes. Create a private collection for your added mods to simplify updates.

**Can I disable a required mod?**
> You can, but you'll need to manage it manually (disable the collection entry). Add the Collections column in Vortex to help manage load order and visibility.

**MacOS Installation**

**Mod Managers**
> Nexus Mods App has planned support for MacOS, but currently no mod manager with collection support exists. Mac users may use our [Manual Installation](Installation/Manual/installation.md) guide or our [Stardrop](Installation/Stardrop/installation.md) guides and transfer from a Windows machine.

**MacOS SMAPI Security Issues**

**Important:** Certain MacOS versions flag SMAPI as malware and forcibly move it to the trash, preventing installation.

*The following solutions are based on community findings, derivded from the Stardew community Discord, and may change as Apple updates MacOS security behaviors.*

**Problem 1: Unable to Run SMAPI Installer**
> When you receive a security message, go to Settings → Security (or Privacy & Security) and hit "Open Anyways" where it lists the blocked file.

**Problem 2: MacOS reports "Malware Blocked and Moved to Trash"**
> Enable MacOS security permissions:

1. Go to System Settings > Privacy and Security
2. Make sure Developer Tools is visible. If you don't see it, open Terminal through Spotlight and enter:
   ```
   spctl developer-mode enable-terminal
   ```
3. Click Developer Tools
4. Add Terminal to the list and enable it
5. If you have other terminal programs (iTerm2, Hyper, Kitty, Alacritty), add them to Developer Tools as well
6. Restart your computer
7. Force close Steam if using it
8. Download and reinstall SMAPI

**Note:** This solution may change over time as Apple updates MacOS security behaviors. If this doesn't work:
- Restart your computer again
- Force close Steam, then try installing SMAPI
- Check the [SMAPI Mac installation wiki](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Mac) for updated solutions

*For the most current solutions and community discussions, visit the the [SMAPI GitHub repository](https://github.com/Pathoschild/SMAPI).*

---

## Known Technical Issues

**Performance & launching**
> Large collections can take 3–5 minutes (or longer) to start a new save or load. Avoid input during loading to prevent crashes.

**Multiplayer / split-screen desync**
> Relaunch the game or restart the session.

**SMAPI not launching**
> Re-add SMAPI as the primary tool in Vortex Dashboard. See Installation.

**Failed to Store Cache Entry (SinZational Speedy Solutions)**
> Informational only; safe to ignore. Not a crash or conflict.

**Unresolved file conflicts (Manage Rules)**
> Ensure configuration/compat/translation files load after the mods they affect. Deploy. Avoid "Use Suggested" if it creates loops.

**Can't craft items despite having ingredients**
> Better Crafting may filter qualities. Enable "Show All Qualities" (Stars button).  
> Example: Bait Maker blocked by quality filters.

---

## NPC & World Bugs

**Duplicated NPCs**
> Rare base-game issue. To remove:
> 1) Load your save  
> 2) In SMAPI console: `debug removenpc [InternalNPCName]`  
> 3) Save and exit  
> Use `patch export "Data/NPCDispositions"` to find internal names. Example: `debug removenpc SenS`

**East Scarp NPCs not attending festivals**
> Expected behavior unless you have 4 hearts with them.

---

## Vortex Behaviors & Workarounds

**Updates can overwrite/delete custom configs**
> Use the Sync Mod Configurations button or create a custom config mod. See Personalization: [Personalization & Custom Configurations](Guides/personalization.md)

**Mod staging may fail silently**
> Verify loaded mods in your SMAPI log, not just the Vortex Mods tab. If a mod is missing, redeploy, or delete and reinstall from the Collection tab.

**Incorrect mod folder structures**
> Fix structure per the official wiki guide, then redeploy.

**Red errors from an "empty Vortex folder"**
> Typically leftovers or config-only installs. Enable recommended files or customize configs as needed.

**Generic Mod Manager version compatibility**
> Use the version recommended in the collection; newer versions may soft-lock certain menus.

---

## Getting Help
- Community Discord: https://discord.com/invite/de2NrHXuty  
- Vortex support: https://discord.com/invite/nexusmods, https://wiki.nexusmods.com/index.php/Category:Vortex

