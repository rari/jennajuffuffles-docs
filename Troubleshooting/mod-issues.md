---
title: Mod-Specific Troubleshooting Guide
keywords:
  - mod troubleshooting
  - mod-specific issues
  - mod problems
  - mod solutions
  - mod hotkeys
  - mod FAQ
  - common questions
  - mod fixes
tags:
  - troubleshooting
  - mods
  - known-issues
  - faq
  - mod-specific
description: >-
  Fix problems with specific mods in Stardew Valley collections. Find solutions
  for mod issues, hotkeys, functionality problems, and answers to common
  questions.
---

# Mod-Specific Known Issues

_Last updated:_ 2026-01-19\
&#xNAN;_&#x41;pplies to Stardew Valley:_ 1.6.15+

This guide answers known issues and common questions specific to individual mods in the collections. If you're experiencing problems with a particular mod, having trouble using a mod's features, or need to know how a mod works, check here. This is not a complete list of every mod—it focuses on mods with commonly reported issues or questions.

***

## Table of Contents

* [Core Framework](mod-issues.md#core-framework)
  * [SMAPI](mod-issues.md#smapi)
* [Major Expansions](mod-issues.md#major-expansions)
  * [Stardew Valley Expanded](mod-issues.md#stardew-valley-expanded)
  * [Ridgeside Village](mod-issues.md#ridgeside-village)
  * [East Scarp](mod-issues.md#east-scarp)
  * [Sword & Sorcery](mod-issues.md#sword--sorcery)
* [Quality of Life](mod-issues.md#quality-of-life)
  * [Automate](mod-issues.md#automate)
  * [Better Crafting](mod-issues.md#better-crafting)
  * [Chests Anywhere](mod-issues.md#chests-anywhere)
  * [Event Lookup](mod-issues.md#event-lookup)
  * [Lookup Anything](mod-issues.md#lookup-anything)
  * [NPC Map Locations](mod-issues.md#npc-map-locations)
  * [UI Info Suite 2](mod-issues.md#ui-info-suite-2)
  * [Schedule Viewer](mod-issues.md#schedule-viewer)
  * [To-Dew](mod-issues.md#to-dew)
  * [Convenient Inventory](mod-issues.md#convenient-inventory)
  * [Generic Mod Config Menu (GMCM)](mod-issues.md#generic-mod-config-menu-gmcm)
  * [SinZational Speedy Solutions](mod-issues.md#sinzational-speedy-solutions)
* [Visual & Customization](mod-issues.md#visual--customization)
  * [Dynamic Reflections](mod-issues.md#dynamic-reflections)
  * [Fashion Sense](mod-issues.md#fashion-sense)
  * [Alternative Textures](mod-issues.md#alternative-textures)
  * [Happy Home Designer](mod-issues.md#happy-home-designer)
  * [Precise Furniture](mod-issues.md#precise-furniture)

***

## Core Framework

### SMAPI

The modding framework that makes all mods work. Required for everything.

**Common Solutions:**

* **SMAPI not launching?** See [New Player Install Instructions](../Installation/index.md#connecting-smapi-to-your-store)
* **SMAPI errors?** See [Your SMAPI Log](your-smapi-log.md)

***

## Major Expansions

### Stardew Valley Expanded

Adds new NPCs, locations, events, and content to expand the game world.

**Resources:**

* [Installation Guide](https://github.com/FlashShifter/StardewValleyExpanded/wiki/Install-guide) | [Troubleshooting](https://github.com/FlashShifter/StardewValleyExpanded/wiki/Troubleshooting) | [Wiki](https://stardew-valley-expanded.fandom.com/wiki/Stardew_Valley_Expanded_Wiki) | [Discord](https://discord.com/invite/svexpanded)

**Common Solutions:**

**Community Center cutscene won't trigger?** The Community Center cutscene has specific requirements that must be met:

* Enter Pelican Town from the Bus Stop (not from another direction)
* Must be Spring 5 or later in Year 1
* Time must be between 8:00 AM and 1:00 PM
* Day must be sunny (no rain or storms)
* Cannot be a festival day
* In multiplayer, only the host can trigger this cutscene

The mods in the collection do not change this event. These are vanilla requirements. If all conditions are met and it still won't trigger, check your SMAPI log for any errors that might be blocking the event.

**Minecart blocking mine entrance?** If you find a minecart blocking the entrance to the mines, it indicates that the config file didn't unpack properly during installation. To fix this:

1. Exit the game
2. In Vortex, go to **Collections > Mods (tab)**
3. Find the configuration pack (Stardew Valley VERY Configured)
4. Remove it (including archive)
5. Reinstall the configuration pack from Collections > Mods tab

This should properly unpack the configuration file and resolve the minecart issue.

**Can't find Rusty/Sewer Key?** Due to Stardew Valley Expanded changes, the way you obtain the Rusty Key (Sewer Key) has changed from vanilla. Gunther no longer provides the Rusty Key at the museum.

To obtain the Rusty Key in SVE, you must complete three requirements:

**1. Meet Krobus in Winter**

* Walk from your farm to the bus stop between 6 AM and 4 PM during Winter
* This triggers an animation where a Shadow Guy (who looks like Krobus) gets startled and runs away
* Follow the footprints to the playground to the left of the Community Center
* Shake the shrubs there to make the Shadow Guy appear
* The Shadow Guy will apologize for stealing, give you a Magnifying Glass, and flee

**2. Reach the Bottom of the Mines**

* Descend through all 120 levels of the mines
* Use your pickaxe to mine ores and bring Bombs to help clear large areas quickly
* Upgrade your weapons and tools as enemies become tougher deeper in the mines
* Reaching the final level completes this requirement

**3. Earn Marlon's Trust**

* After meeting Krobus and reaching the bottom of the mines, you'll need to earn Marlon's trust
* **Year 1 requirements:** Must have 5 hearts with Marlon and it must be raining to trigger his key event
* **Year 2 and beyond:** The requirement reverts to 2 hearts, and the weather does not matter
* Raise friendship by talking to Marlon and giving him gifts he likes
* Once you meet the conditions and complete his heart event in the Adventurer's Guild, he will reward you with the Rusty Key, granting you access to the Sewers

### Ridgeside Village

Adds an entirely new village with 45+ NPCs, locations, and a cable car system. Access Ridgeside Village via the staircase at the Bus Stop after the cutscene with Lewis and Lenny, then ride the cable car.

**Resources:**

* [Installation Guide](https://github.com/Rafseazz/Ridgeside-Village-Mod/blob/main/Installation%20Guide.md) | [Wiki](https://ridgeside.fandom.com/wiki/Ridgeside_Village_Wiki) | [Discord](https://discord.gg/4SRbjEQG2D)

**Common Solutions:**

**Can't access Ridgeside Village or cable car?** If the stairs or cable car aren't appearing, check the following:

1. Verify Ridgeside Village shows as installed in your SMAPI log
2. Ensure you installed the PC version (not mobile) if installing manually
3. Make sure the mod folder is extracted (not still a .zip/.rar file)
4. Check for missing dependencies - SMAPI will list any required frameworks that are missing
5. Remove any mods that edit the Bus Stop or its warps (including some custom farms) as they can conflict
6. If you have an outdated "Music of Ridgeside Village" add-on, remove it (music is now bundled)

**Game hangs or takes a long time to load?** Ridgeside Village can take several minutes to load schedules on first launchThis is normal. SinZational Speedy Solutions does solve a lot of this.

**NPCs not spawning or events not triggering?**

* If monsters aren't spawning in Ridge Forest or Spirit Realm, check if you have time paused or significantly slowed within It's Stardew Time/Time Master.
* For Spirit Realm pedestal issues, use SMAPI console command: `RSV_reset_pedestals`

**Items turning into other items (JSON shuffle)?** This is a known issue with Json Assets. Trash the bugged items and respawn them with CJB Item Spawner. Ensure all players in multiplayer use identical mod sets and configs.

**Linux Quest Parsing Errors?** Linux users may see errors about quest parsing in the SMAPI log. This issue will be fixed in the next update. In the meantime, you can install [Ridgeside Village Quest Fix For Linux and Mac](https://www.nexusmods.com/stardewvalley/mods/36004) to patch this issue.

### East Scarp

Major area expansion east of Pelican Town with new locations and NPCs.

**Resources:**

* [Wiki](https://eastscarp.wiki.gg/) | [Discord](https://discord.com/invite/QFtDA3CJwJ)

**Common Solutions:**

* **NPCs not attending festivals?** Some East Scarp NPCs require 4+ hearts before attending festivals

### Sword & Sorcery

Fantasy expansion with custom skill trees and unique maps.

**Common Solutions:**

**How do I access the Adventure Bar?** Press **Ctrl + U** (configurable) to toggle the Adventure Bar sidebar overlay. Press **U** to configure the Adventure Bar.

**How do I use abilities?** Sword & Sorcery adds two ability bars:

* **Ability Bar 1:** Press **Ctrl + 1** through **Ctrl + 8** to use abilities in slots 1-8
* **Ability Bar 2:** Press **Shift + 1** through **Shift + 8** to use abilities in slots 1-8

**Can I change the keybinds?** Yes, all keybinds can be customized via GMCM (press `Numpad -` or go to Settings > Mod Options). Look for "Sword & Sorcery (SMAPI Component)" in the keybindings section.

***

## Quality of Life

### Automate

Automatically processes items in machines and chests by connecting them to chests. Press **U** (configurable) to show an automation overlay that visualizes connected machines, chests, and connectors.

### Better Crafting

Enhanced crafting menu with categories, favorites, and quality filters. Replaces the vanilla crafting screen with improved organization and bulk crafting support. Use **Shift + Left-click** to craft 5 at a time, or **Ctrl + Shift + Left-click** to craft 25 at a time.

**Common Solutions:**

* **Can't craft items despite having ingredients?** Better Crafting has quality filters enabled by default. Click the **Stars button** on the right side of the crafting menu and enable **"Show All Qualities"**
* **Missing recipes (like Chest)?** Better Crafting organizes recipes into categories. Check other categories or look for "Show All" / "Uncategorized" options
* **Bait Maker not working?** This is often blocked by quality filters - enable "Show All Qualities" as above

### Chests Anywhere

Access your chests, dressers, fridge, shipping bin, and Junimo huts from anywhere. You can edit chest names and categories by clicking the edit icon when a chest is open. The shipping bin can be opened like a chest to retrieve items before they're shipped. The collection adjusts chests to work within the area you are in, and disables the chest hotkey.

### Event Lookup

View today's events and schedules. Press **N** (configurable) to open a list of all heart events you can trigger today, with details on when and how to trigger them. Also adds console commands for event lookup.

### Lookup Anything

Press **F1** to see live information about whatever's under your cursor. Learn villager favorite gifts, when crops will be ready, fence durability, why animals are unhappy, and more. Works on world objects, inventory, calendar, menus, and shops. Press **Left Shift + F1** to search. On laptops/macOS you may need **FN + F1**.

### NPC Map Locations

Shows NPCs and farmers on a modified map page. Open the game map with **M** (vanilla key), then press **Tab** while the map is open to access the mod menu. Includes an optional minimap HUD and various filtering options.

### UI Info Suite 2

Displays helpful information about things around you, including calendar, quest board, daily luck, experience gains, crop info, sprinkler ranges, and more. Press **B** to open the Calendar anywhere, or **H** to open the Help Wanted/Quest Billboard anywhere. Also adds buttons in the inventory menu to access these features.

**Common Solutions:**

* **Want to adjust UI Info Suite 2 features?** On the title screen, open GMCM (⚙️ button, lower left), find UI Info Suite 2, and enable its menu. In-game, open the menu (ESC) and use the 🔨 tab to customize the interface.
* **Can't access calendar or quest board?** Use the default keybinds (**B** for Calendar, **H** for Quest Board). If these don't work, check your keybinds in GMCM (Settings menu or `Numpad -`) or edit the mod's data file for your save

### Schedule Viewer

Shows NPC schedules for the current day. Press **V** (configurable) to open/close the schedule viewer. The main menu lists previous/current/next entries per NPC and shows an "!" if the NPC has an active quest. Clicking an NPC opens a details menu with their full schedule, current location, and whether they can receive a gift.

### To-Dew

An in-game to-do list. Press **L** (configurable) to open the list. The list can also be shown as a top-left overlay (can be disabled in config). Click items to mark them done. Type in the textbox and press Enter to add items. Press **Esc** to close the list.

### Convenient Inventory

Adds convenience features to your inventory. Hold **Left Alt** (PC) or **Left Shoulder** (controller) and select items to favorite them (favorited items are protected from quick stack, trashing, dropping, and shipping). Click the "Quick Stack to Nearby Chests" button in the inventory UI to deposit matching items into nearby chests. Right-click a stack while holding **Left Ctrl + Left Shift** (PC) or **Left Trigger** (controller) to take all but one from the stack.

### Generic Mod Config Menu (GMCM)

Access mod settings and configurations.

**Common Solutions:**

* **How do I access mod settings?** Press `Numpad -` or go to Settings menu and look for "Mod Options" at the bottom (see [About the Collections](../About/index.md) for keybinds)
* **Can't find GMCM?** It's accessible from the title screen Settings menu (⚙️ icon) or in-game Settings

### SinZational Speedy Solutions

Performance optimization mod.

**Common Solutions:**

* **Visual bugs after Community Center completion?** "Slow Map Loader" is disabled in the collection's configuration files to prevent this visual bugs.

***

## Visual & Customization

### Dynamic Reflections

Adds dynamic reflections to water and other surfaces.

**Common Solutions:**

* **Game running slowly?** Disabling Dynamic Reflections may help if you have limited memory

### Fashion Sense

Framework that enables outfit customization for characters, including accessories, hairstyles, hats, shirts, sleeves, pants, and shoes. Purchase a **Hand Mirror** from Pierre's shop (1,500g) and hold it, then left-click to open the appearance menu. The collection configuration also sets a hotkey **G** (unbound by default) to open the dresser interface anywhere!

**Common Solutions:**

* **How do I change my outfit?** Buy a Hand Mirror from Pierre (1,500g), hold it and left-click to open the appearance menu. If the mirror doesn't show in Pierre's stock, use console command `fs_add_mirror` to add it. In single player games you may also select to get one for free at the start of the game.

### Alternative Textures

Framework enabling texture variation for placeable objects, buildings, and entities. Purchase tools from Robin: **Paint Bucket** (left-click items to change texture), **Paint Brush** (right-click to copy, left-click to paste), **Spray Can** (randomize textures in a radius), and **Texture Catalogue** (browse available textures). Textures can be seasonal and randomized on placement.

**Common Solutions:**

* **How do I change textures?** Visit Robin to purchase a Paint Bucket and other AT tools. Left-click a supported item with the Paint Bucket to open texture selection
* **"No alternative textures for this season" message?** This means no textures are available for that item in the current season

### Happy Home Designer

Overhauls the furniture and wallpaper catalogues with a feature-rich UI. Right-click a placed catalogue to open the menu and place furniture directly from it. You can combine catalogues by holding one and right-clicking another in your inventory. Supports favorites/bookmarks and integrates with Alternative Textures. Configure hotkeys via GMCM (defaults are unbound).

### Precise Furniture

Move furniture pixel-by-pixel for perfect placement. Press **Arrow Keys** while hovering over placed furniture to move it. Hold **Left Alt** while pressing arrow keys for faster movement. Hold **Left Alt** and right-click furniture to lock it (prevents picking up or moving). Only works with furniture, not objects.

***

## See Also

* [About the Collections](../About/index.md) - Collection features and keybinds
* [Troubleshooting & FAQ](index.md) - For general troubleshooting
* [How to Customize Collections](../Customization/index.md) - Adding your own mods
* [New Player Install Instructions](../Installation/index.md) - Installation guide
