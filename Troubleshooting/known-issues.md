---
title: Known Issues and Solutions
description: Find fixes for known problems with Stardew Valley mod collections. Includes platform-specific issues, Linux problems, Quest Framework issues, and their solutions.
keywords: [known issues, bugs, fixes, solutions, platform issues, Linux problems, Quest Framework, common problems, bug fixes]
tags: [troubleshooting, known-issues, bugs, fixes, platform-specific]
---

# Known Issues

*Last updated:* 2026-01-15  
*Applies to Stardew Valley:* 1.6.15+

This page documents known issues with collections and their solutions. These are problems that have been identified and resolved by the community or collection maintainers. If you're experiencing an issue, check this list first—you may find a documented solution.

---

## Gameplay Issues
### Farm Map Not Loading
**Symptom:** Can't exit house, corrupted farm map, missing textures

**Solution:**
- Ensure your farm map mod is enabled
- Only one farm map should be active
- Verify in Vortex that the farm map mod is enabled and deployed

### Crafting Issues
**Symptom:** Can't craft items despite having ingredients

**Solution:**
- Check Better Crafting quality filters in GMCM
- Verify ingredient quality matches requirements
- Check if items are favorited (may prevent crafting)

---

## Performance Issues

### Slow Loading
**Symptom:** Game takes a long time to load

**Solution:**
- This is normal for large collections
- Don't alt-tab during loading
- First launch may take several minutes

---

## Multiplayer Issues

### Cannot Create Multiplayer Game
**Symptom:** Unable to create a multiplayer game session

**Solution:**
- Ensure game shop client (Steam, Xbox Games, etc) is available before launch
- There may be an error in the player log at start-up if this step is missed

### Crashing, No Cabins, or Cannot Find Farm
**Symptom:** Game crashes, insufficient cabins, or farm cannot be found in multiplayer

**Solution:**
- Mods mismatch (different mods, different versions, different configurations)
- Recommend using the quick fix process to ensure similar installations for both players
- Use [Multiplayer Mod Sync](https://www.nexusmods.com/stardewvalley/mods/6609) to verify all players have matching mod loadouts at launch

### Desync Issues
**Symptom:** Players seeing different things, actions not registering

**Solution:**
- All players must have matching mods and versions
- Restart the game and session
- Verify configurations match across all players

---

## Vortex Issues

### Sync Mod Configurations Backs Up smapi-internal
**Symptom:** The Sync Mod Configurations feature incorrectly backs up the `smapi-internal` folder

**Solution:**
1. Right-click on **Stardew Valley Configurations** mod entry created by Vortex
2. Select **Open in File Manager** to access the mod folder
3. Locate the `smapi-internal` folder within the configuration mod
4. Cut the `smapi-internal` folder from the configuration mod location
5. Navigate to your main Stardew Valley folder (where the game is installed)
6. Paste the `smapi-internal` folder back into its proper location

{% hint style="info" %}
Please report to Vortex staff if this happens - this issue needs more visibility to be properly addressed.
{% endhint %}

---

## See Also

- [Troubleshooting & FAQ](index.md) - For general troubleshooting
- [Your SMAPI Log](your-smapi-log.md) - To diagnose issues
- [Discord Community](https://discord.gg/MPcgJUXeeY) - Join for additional help
