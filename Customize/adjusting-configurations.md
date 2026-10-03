# Adjusting Configurations
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

The steps on this page are for Vortex.

In-game settings use Generic Mod Config Menu. In Vortex, collection configuration files are edited from each collection's VERY Configured mod.

Adding or disabling a mod? See [Adding and Disabling Mods](adding-and-disabling-mods.md).

## In-Game Configuration (GMCM)

Many mods support **Generic Mod Config Menu (GMCM)**, which provides an in-game menu for adjusting mod settings:

- Open Generic Mod Config Menu from the main page (⚙️), the button at the bottom of Settings (Mod Options), or the assigned [Hotkey](../Reference/hotkeys.md).
- Adjust settings directly in-game without editing files.
- Changes are saved automatically.
- Some mods may require restarting the game for changes to take effect.

## VERY Configured

{% hint style="warning" %}
**Sync Mod Configurations** is not recommended with collections. If it is already enabled, turn it off in **Game Settings**.
{% endhint %}

In Vortex, right-click the VERY Configured mod for a collection and open it in File Manager to edit its configuration files. After you edit a file in File Manager, right-click **Reinstall** of the VERY Configured mod will include that change. 

To copy settings you already changed in Generic Mod Config Menu, go to **Open > Game Mods Folder** (the third option) and find `config.json` in that mod's folder. 

If you have made changes to VERY Configured, be aware that they will not be retained should the configuration file change in the next revision. 

You can also add your own config file that loads after VERY Configured, but it can be complicated. See [Creating Mods and Loose Files](creating-mods-and-loose-files.md#loose-files).

## What Configs Actually Change

Configuration files control:

- How mods behave (automation ranges, display options, and similar)
- Keyboard shortcuts and controller mappings
- UI scaling, color schemes, display options
- Difficulty settings, quality-of-life features

Most configs can be changed safely without breaking saves. Some changes can affect save compatibility.

## Related

- [Adding and Disabling Mods](adding-and-disabling-mods.md)
- [Creating Mods and Loose Files](creating-mods-and-loose-files.md)
- [Update with Vortex](../Update/vortex.md)
- [Keybinds](../Troubleshooting/known-issues.md)
- [Known Issues](../Troubleshooting/known-issues.md#sync-mod-configurations-backs-up-smapi-internal)
