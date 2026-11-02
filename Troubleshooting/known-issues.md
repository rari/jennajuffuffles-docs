# Known Issues
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

## Gameplay Issues

### Farm Map Not Loading

**Symptom:** Can't exit house, corrupted farm map, missing textures

**Solution:**

- Ensure your farm map mod is enabled
- Only one farm map should be active

### Crafting Issues

**Symptom:** Can't craft items despite having ingredients

**Solution:**

- Check Better Crafting quality filters in GMCM
- Verify ingredient quality matches requirements
- Check if items are favorited (may prevent crafting)

### Ginger Island Locations - Redux

**Symptom:** Buying the Dusts from the trader, including Growing Dust, does not add them to the crafting window.

**Solution:**

Until the mod is updated, add the recipes from the SMAPI console:

```bash
debug craftingrecipe GiEXredux_GrowPlaceholder
debug craftingrecipe GiEXredux_PurifyPlaceholder
debug craftingrecipe GiEXredux_GoldPlaceholder
debug craftingrecipe GiEXredux_VoidPlaceholder
debug craftingrecipe GiEXredux_RevivalPlaceholder
```

### NPCs May Split

This is caused by a vanilla game bug that causes some modded NPCs to split. This is a known issue in the game (not specifically related to the collection) that seems to most frequently happen when talking to NPCs while they are in movement.

**Solution:**

1. Load your save.
2. Run in the SMAPI console:

```bash
debug removenpc [InternalNPCName]
```

3. Sleep.

The `removenpc` command removes all instances of that NPC from the game immediately. One instance of them will spawn normally the next day.

**Example:** For Sen specifically, use:

```bash
debug removenpc SenS
```

### Community Center Cutscene Won't Trigger

The Community Center cutscene has specific requirements that must be met:

- Enter Pelican Town from the Bus Stop (not from another direction)
- Must be Spring 5 or later in Year 1
- Time must be between 8:00 AM and 1:00 PM
- Day must be sunny (no rain or storms)
- Cannot be a festival day
- In multiplayer, only the host can trigger this cutscene

The mods in the collection do not change this event. These are vanilla requirements. If all conditions are met and it still won't trigger, check [Your SMAPI Log](your-smapi-log.md) for errors that might be blocking the event.

### NPCs Won't Leave Their Houses

This is normal on the first day modded NPCs are added to the game. Their schedules load the next day.

## Performance Issues

### Slow Loading

**Symptom:** Game takes a long time to load

**Solution:**

- This is normal for large collections
- Don't alt-tab during loading
- First launch may take several minutes

## Multiplayer Issues

### Cannot Create Multiplayer Game

**Symptom:** Unable to create a multiplayer game session

**Solution:**

- Ensure the game shop client (Steam, Xbox Games, and so on) is available before launch
- There may be an error in the player log at start-up if this step is missed

### Crashing, No Cabins, or Cannot Find Farm

**Symptom:** Game crashes, insufficient cabins, or farm cannot be found in multiplayer

**Solution:**

- Mods mismatch (different mods, different versions, different configurations)
- Both players need the same collections, mods, versions, and configurations
- If one player updated and the other did not, see [Collection / Update Issues](collection-update-issues.md)
- Use [Multiplayer Mod Sync](https://www.nexusmods.com/stardewvalley/mods/6609) to verify all players have matching mod loadouts at launch

### Desync Issues

**Symptom:** Players seeing different things, actions not registering

**Solution:**

- All players must have matching mods and versions
- Restart the game and session
- Verify configurations match across all players

### Controller Input Captured by SMAPI Console on Start-up

**Symptom:** If the game starts with a controller already connected, input can be captured by both Stardew Valley and the SMAPI console window at the same time. This can lead to accidental SMAPI console closure and a crash shortly after start-up.

**Solution:**

- Click once into the game window with your mouse after launch so focus is on Stardew Valley
- Or connect or power on the controller after the game has already started
- If a crash already happened, relaunch and apply one of the focus steps above before continuing

### Quests May Require Host to Advance

**Symptom:** Some quests (notably Ridgeside Village; see [Mod-Specific Known Issues](mod-specific-known-issues.md#ridgeside-village)) may not progress unless the host advances them.

**Solution:**

- Have the host trigger or advance the quest steps
- If progress still stalls, check [Your SMAPI Log](your-smapi-log.md) for related errors and restart the session
- Make a record of the event or quest that was stuck and report it on [Discord](https://discord.gg/MPcgJUXeeY)

## Vortex

These steps are for Vortex.

### Sync Mod Configurations Backs Up "smapi-internal"

**Symptom:** The Sync Mod Configurations feature incorrectly backs up the `smapi-internal` folder

**Solution:**

1. Right-click the **Stardew Valley Configurations** mod entry created by Vortex
2. Select **Open in File Manager** to open the mod folder
3. Locate the `smapi-internal` folder within the configuration mod
4. Cut the `smapi-internal` folder from the configuration mod location
5. Navigate to your main Stardew Valley folder (where the game is installed)
6. Paste the `smapi-internal` folder back into its proper location

{% hint style="info" %}
Please report this to Vortex staff if it happens. This issue needs more visibility to be properly addressed. Using Sync Mod Configurations is not recommended at this time.
{% endhint %}

## Related

- [Your SMAPI Log](your-smapi-log.md)
- [Install with Vortex](../Install/vortex.md)
- [Mod-Specific Known Issues](mod-specific-known-issues.md)
