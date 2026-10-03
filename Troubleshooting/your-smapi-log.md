# Your SMAPI Log
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

## How to Share Your Log

When asking for help, include your SMAPI log. The log is useful even when you do not see an obvious error.

### Vortex

These steps are for Vortex:

1. Click the **SMAPI Log** button on the Mods panel
2. Click **Copy & Share log** at the bottom of the pop-up
3. The browser opens automatically. Paste into "Paste Log Here" and click **Save & Parse Log**
4. This log link can be viewed or shared

The parsed log is easier for other people to read. If the path to your game files includes your name, consider using Find & Replace to replace it before uploading.

A new log is only generated when the game launches. If you install, remove, or update mods, launch the game again before the log will show those changes.

<details>
<summary>Share the log without Vortex</summary>

If you're not using Vortex, or you need the file itself:

**Finding your log file:**

- **Windows:** Press **Windows + R**, enter `%appdata%\StardewValley\ErrorLogs`, and open `SMAPI-latest.txt` or `SMAPI-crash.txt`
- **Mac/Linux:** Go to `~/.config/StardewValley/ErrorLogs` and open `SMAPI-latest.txt` or `SMAPI-crash.txt`

**Sharing your log:**

1. Open your log file and copy the entire contents of `SMAPI-latest.txt`
2. Go to [https://smapi.io/log/](https://smapi.io/log/)
3. Paste the log into the text box
4. Click **Save & Parse Log**
5. Copy the URL that appears after uploading
6. Share that URL when asking for help (Discord, forums, and so on)

</details>

## What the Log Shows

SMAPI uses colors for log levels. The colors show how serious a message is.

**Mods loaded** lists every mod that successfully loaded. If a mod is not in that list, it did not load.

### White: Operation

- Normal operation messages
- General information about mod loading and operation
- Usually safe to ignore unless you are troubleshooting

### Yellow: Warning

- Potential problems you should be aware of
- Usually non-critical, but worth reading
- May indicate minor incompatibilities or deprecated features
- Check whether the issues persist

### Red: Error

- Something went wrong
- These need to be addressed
- May prevent mods or the game from working properly
- Always investigate red errors

### Purple: Information

- Mods which have an update available
- Update the collection rather than loose mods. See [Collection / Update Issues](collection-update-issues.md)

## Common Error Messages

### "Empty Vortex folder"

Vortex. This line usually means one of the following:

- A mod was disabled in Vortex
- A configuration file is being applied to a disabled mod
- Leftover files remain from a disabled mod

The longer fix is on [Vortex Notifications and Solutions](vortex-notifications.md).

### "Failed to load"

- The mod couldn't be loaded
- Check for missing dependencies
- Verify mod version compatibility

### "Duplicate mod"

- Two copies of the same mod exist
- Remove one copy

### "Failed parsing new quests."

- **Linux and Mac only** (including Steam Deck on a Linux runtime)

- **Linux and Mac only** (including Steam Deck on a Linux runtime)
- Ridgeside Village quest data failed to parse
- Install [Ridgeside Village Quest Fix For Linux and Mac](https://www.nexusmods.com/stardewvalley/mods/36004)
- See [Mod-Specific Known Issues](mod-specific-known-issues.md#ridgeside-village)

## Related

- [Vortex Notifications and Solutions](vortex-notifications.md)
- [Mod-Specific Known Issues](mod-specific-known-issues.md)
- [Install with Vortex](../Install/vortex.md)
