# Mod-Specific Known Issues
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

This is not a complete list of every mod. It covers mods with commonly reported issues or questions.

## Alternative Textures

Framework enabling texture variation for placeable objects, buildings, and entities. Purchase tools from Robin: **Paint Bucket** (left-click items to change texture), **Paint Brush** (right-click to copy, left-click to paste), **Spray Can** (randomize textures in a radius), and **Texture Catalogue** (browse available textures). Textures can be seasonal and randomized on placement.

**Common solutions:**

- **How do I change textures?** Visit Robin to purchase a Paint Bucket and other Alternative Textures tools, or receive them through the mail when Creative Neighbors is installed. Left-click a supported item with the Paint Bucket to open texture selection
- **"No alternative textures for this season" message?** This means no textures are available for that item in the current season from the texture packs you have loaded

## Better Crafting

Enhanced crafting menu with categories, favorites, and quality filters. Replaces the vanilla crafting screen with improved organization and bulk crafting support. Use **Shift + Left-click** to craft 5 at a time, or **Ctrl + Shift + Left-click** to craft 25 at a time.

**Common solutions:**

- **Can't craft items despite having ingredients?** Better Crafting has quality filters enabled by default. Click the **Stars button** on the right side of the crafting menu and enable **"Show All Qualities"**
- **Missing recipes (like Chest)?** Better Crafting organizes recipes into categories. Check other categories or look for "Show All" / "Uncategorized" options
- **Bait Maker not working?** This is often blocked by quality filters. Enable "Show All Qualities" as above

## Dynamic Reflections

Adds dynamic reflections to water and other surfaces.

**Common solutions:**

- **Game running slowly?** Disabling Dynamic Reflections may help if you have limited memory
- **Panoramic background in the Highlands appears black?** Dynamic Reflections may cause this. Disable Dynamic Reflections if the Highlands background stays black.

## East Scarp

Major area expansion east of Pelican Town with new locations and NPCs.

**Resources:**

- [Wiki](https://eastscarp.wiki.gg/) | [Discord](https://discord.com/invite/QFtDA3CJwJ)

**Common solutions:**

- **NPCs not attending festivals?** Some East Scarp NPCs require 4+ hearts before attending festivals
- **SpaceCore crash with Eli & Dylan?** There is a known crash case reported around Eli & Dylan that currently appears to be isolated to Russian localization. This is still under investigation with the mod author

## Fashion Sense

Framework that enables outfit customization for characters, including accessories, hairstyles, hats, shirts, sleeves, pants, and shoes. Purchase a **Hand Mirror** from Pierre's shop (1,500g) and hold it, then left-click to open the appearance menu. The collection configuration also sets a hotkey **G** (unbound by default) to open the dresser interface anywhere.

**Common solutions:**

- **How do I change my outfit?** Buy a Hand Mirror from Pierre (1,500g), hold it, and left-click to open the appearance menu. If the mirror doesn't show in Pierre's stock, use the console command `fs_add_mirror` to add it. In single player you may also choose to get one for free at the start of the game

## Generic Mod Config Menu (GMCM)

Access mod settings and configurations.

**Common solutions:**

- **How do I access mod settings?** Press `Numpad -` or go to the Settings menu and look for "Mod Options" at the bottom (see [Hotkeys](../Reference/hotkeys.md))
- **Can't find GMCM?** It's available from the title screen Settings menu (gear icon) or in-game Settings

## Ridgeside Village

Adds an entirely new village with 45+ NPCs, locations, and a cable car system. Access Ridgeside Village via the staircase at the Bus Stop after the cutscene with Lewis and Lenny, then ride the cable car.

**Resources:**

- [Installation Guide](https://github.com/Rafseazz/Ridgeside-Village-Mod/blob/main/Installation%20Guide.md) | [Wiki](https://ridgeside.fandom.com/wiki/Ridgeside_Village_Wiki) | [Discord](https://discord.gg/4SRbjEQG2D)

**Common solutions:**

**Can't access Ridgeside Village or the cable car?** If the stairs or cable car aren't appearing, check the following:

1. Verify Ridgeside Village shows as installed in [Your SMAPI Log](your-smapi-log.md)
2. Ensure you installed the PC version (not mobile) if installing manually
3. Make sure the mod folder is extracted (not still a .zip or .rar file)
4. Check for missing dependencies. SMAPI will list any required frameworks that are missing
5. Remove any mods that edit the Bus Stop or its warps (including some custom farms) as they can conflict
6. If you have an outdated "Music of Ridgeside Village" add-on, remove it (music is now bundled)

**Game hangs or takes a long time to load?** Ridgeside Village can take several minutes to load schedules on first launch. This is normal. SinZational Speedy Solutions does solve a lot of this.

**NPCs not spawning or events not triggering?**

- If monsters aren't spawning in Ridge Forest or Spirit Realm, check if you have time paused or significantly slowed within It's Stardew Time or Time Master
- For Spirit Realm pedestal issues, use the SMAPI console command: `RSV_reset_pedestals`

**Items turning into other items (JSON shuffle)?** This is a known issue with Json Assets. Trash the bugged items and respawn them with CJB Item Spawner. Ensure all players in multiplayer use identical mod sets and configs.

**Linux and Mac: `Failed parsing new quests.` in your log?** Linux and Mac players may see this error in the SMAPI log when Ridgeside Village quest data fails to parse. Install [Ridgeside Village Quest Fix For Linux and Mac](https://www.nexusmods.com/stardewvalley/mods/36004) to patch it. How to read that line is on [Your SMAPI Log](your-smapi-log.md).

**Farmhand stuck on "Unsealing"?** Farmhand support for this end-stage chain is currently unreliable. If a farmhand gets stuck, run these in SMAPI:

- `debug completequest 72860007` - Completes the quest in the farmhand journal
- `debug ebi 75160259` - Applies the expected follow-up flags for that player

## SinZational Speedy Solutions

Performance optimization mod.

**Common solutions:**

- **Visual bugs after Community Center completion?** "Slow Map Loader" is disabled in the collection's configuration files to prevent these visual bugs
- **ERROR spam about "Failed to store cache entry for ...\Stardew Valley\Mods\Ridgeside Village\[CP] Ridgeside Village\Assets\Maps\EventMaps\RSVOpenPlot.tmx"?** Outside of the minor annoyance of error messages in the console, this has no negative effects (just the lack of the positive effect from the cache). In most cases, you can safely ignore it

## SMAPI

The modding framework that makes all mods work. Required for everything.

**Common solutions:**

- **SMAPI not launching?** See [Install with Vortex](../Install/vortex.md)
- **SMAPI errors?** See [Your SMAPI Log](your-smapi-log.md)

## Stardew Valley Expanded

Adds new NPCs, locations, events, and content to expand the game world.

**Resources:**

- [Installation Guide](https://github.com/FlashShifter/StardewValleyExpanded/wiki/Install-guide) | [Troubleshooting](https://github.com/FlashShifter/StardewValleyExpanded/wiki/Troubleshooting) | [Wiki](https://stardew-valley-expanded.fandom.com/wiki/Stardew_Valley_Expanded_Wiki) | [Discord](https://discord.com/invite/svexpanded)

**Common solutions:**

**Minecart blocking the mine entrance?** If you find a minecart blocking the entrance to the mines, the config file didn't unpack properly during installation.

Vortex:

1. Exit the game
2. Go to **Collections > Mods**
3. Find the configuration pack (Stardew Valley VERY Configured)
4. Remove it (including the archive)
5. Reinstall the configuration pack from Collections > Mods

This should unpack the configuration file and clear the minecart. If Vortex also asked you to set rules, see [Vortex Notifications and Solutions](vortex-notifications.md).

**Can't find the Rusty Key (Sewer Key)?** Due to Stardew Valley Expanded changes, the way you obtain the Rusty Key has changed from vanilla. Gunther no longer provides the Rusty Key at the museum.

To obtain the Rusty Key in Stardew Valley Expanded, complete three requirements:

**1. Meet Krobus in Winter**

- Walk from your farm to the bus stop between 6 AM and 4 PM during Winter
- This triggers an animation where a Shadow Guy (who looks like Krobus) gets startled and runs away
- Follow the footprints to the playground to the left of the Community Center
- Shake the shrubs there to make the Shadow Guy appear
- The Shadow Guy will apologize for stealing, give you a Magnifying Glass, and flee

**2. Reach the bottom of the mines**

- Descend through all 120 levels of the mines
- Use your pickaxe to mine ores and bring bombs to help clear large areas quickly
- Upgrade your weapons and tools as enemies become tougher deeper in the mines
- Reaching the final level completes this requirement

**3. Earn Marlon's trust**

- After meeting Krobus and reaching the bottom of the mines, earn Marlon's trust
- **Year 1 requirements:** Must have 5 hearts with Marlon, and it must be raining, to trigger his key event
- **Year 2 and beyond:** The requirement reverts to 2 hearts, and the weather does not matter
- Raise friendship by talking to Marlon and giving him gifts he likes
- Once you meet the conditions and complete his heart event in the Adventurer's Guild, he rewards you with the Rusty Key, which grants access to the Sewers

**Apples 2 heart event does not trigger immediately?** Sleep and return the next day, even if the Vineyard interior has already changed. This is due to how older mods use next-day flags.

**World Navigator shows the SVE "Train Station" too early?** This can appear before the unlock quest is actually available. Use it as preview only. Progression still follows quest and flag requirements.

## Sword & Sorcery

Fantasy expansion with custom skill trees and unique maps.

**Common solutions:**

**How do I access the Adventure Bar?** Press **Ctrl + U** (configurable) to toggle the Adventure Bar sidebar overlay. Press **U** to configure the Adventure Bar.

**How do I use abilities?** Sword & Sorcery adds two ability bars:

- **Ability Bar 1:** Press **Ctrl + 1** through **Ctrl + 8** to use abilities in slots 1-8
- **Ability Bar 2:** Press **Shift + 1** through **Shift + 8** to use abilities in slots 1-8

**Can I change the keybinds?** Yes. All keybinds can be customized via GMCM (press `Numpad -` or go to Settings > Mod Options). Look for "Sword & Sorcery (SMAPI Component)" in the keybindings section. Default keys are also on [Hotkeys](../Reference/hotkeys.md).

**Quest or event trigger not firing yet?** Sword & Sorcery uses many delayed and conditional triggers. If a step doesn't fire immediately, sleep a few days and check again before assuming it's broken.

## Related

- [Your SMAPI Log](your-smapi-log.md)
- [Hotkeys](../Reference/hotkeys.md) 
- [Adding and Disabling Mods](../Customize/adding-and-disabling-mods.md)
