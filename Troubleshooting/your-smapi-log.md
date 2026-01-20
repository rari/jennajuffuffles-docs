---
title: Using SMAPI Log Files for Troubleshooting
description: Learn how to read and share SMAPI log files to diagnose Stardew Valley mod problems. Understand log levels, error messages, and how to use smapi.io for log analysis.
keywords: [SMAPI log, error log, log levels, troubleshooting, sharing logs, smapi.io, log colors, trace, debug, error messages]
tags: [troubleshooting, smapi, logs, errors, debugging]
---

# Your SMAPI Log

*Last updated:* 2026-01-19  
*Applies to Stardew Valley:* 1.6.15+

The SMAPI log shows what mods loaded and any errors that occurred. Understanding how to read it is essential for troubleshooting. This guide will help you interpret log levels, identify errors, and share your log when seeking help.

---

## What the Log Shows

SMAPI uses different colors to indicate log levels. The colors help you quickly identify the severity of messages:

### White/Gray Text
- **Info, Debug, or Trace** - Normal operation messages
- General information about mod loading and operation
- Usually safe to ignore unless troubleshooting

### Yellow Text
- **Warnings** - Potential problems that you should be aware of
- Usually non-critical but worth reading
- May indicate minor incompatibilities or deprecated features
- Check if issues persist

### Red Text
- **Errors** - Something went wrong
- These need to be addressed
- May prevent mods or the game from working properly
- Always investigate red errors

### Purple Text
- Indicates mods which have an update available

---

## Key Sections

### Mods Loaded
Lists all mods that successfully loaded. If a mod isn't listed, it didn't load.

### Errors
Red text showing what went wrong. These are the most important to address.

### Warnings
Yellow text showing potential issues. Review these if you're experiencing problems.

---

## Common Log Messages

### "Empty Vortex folder"
- Usually means a mod was disabled in Vortex
- A configuration file being applied to a disabled mod
- Or leftover files from a disabled mod
- See [Troubleshooting & FAQ](index.md) for solutions

### "Failed to load"
- Mod couldn't be loaded
- Check for missing dependencies
- Verify mod version compatibility

### "Duplicate mod"
- Two copies of the same mod exist
- Remove one copy
- See [Troubleshooting & FAQ](index.md) for details

---

## How to Share Your Log

When asking for help, always include your SMAPI log. The log contains valuable information even if you don't see obvious errors.

### Vortex

1. Click the **SMAPI Log** button on the Mods panel
2. Click **Copy & Share log** at the bottom of the pop-up
3. Browser opens automatically, paste into the "Paste Log Here" and click **Save & Parse Log**
4. This log link can be easily viewed or shared

The parsed log makes it easier for others to read and identify issues. If the path to your game files includes your name, consider using Find & Replace to replace it before uploading.

**Important:** A new log is only generated when the game launches. If you make changes to mods (install, remove, or update), you must launch the game again to see those changes reflected in the log.

<details>
<summary>Access and Share Log without Vortex</summary>

If you're not using Vortex or need to access the log file directly:

**Finding your log file:**

- **Windows:** Press **Windows + R**, enter `%appdata%\StardewValley\ErrorLogs`, open `SMAPI-latest.txt` or `SMAPI-crash.txt`
- **Mac/Linux:** Navigate to `~/.config/StardewValley/ErrorLogs`, open `SMAPI-latest.txt` or `SMAPI-crash.txt`

**Sharing your log:**

1. **Open your log file** and copy the entire contents of `SMAPI-latest.txt`
2. **Go to** [https://smapi.io/log/](https://smapi.io/log/)
3. **Paste the log** into the text box on the page
4. **Click "Save & Parse Log"**
5. **Copy the URL** that appears after uploading
6. **Share the URL** when asking for help (Discord, forums, etc.)

</details>

---

## See Also

- [Troubleshooting & FAQ](index.md) - For common issues
- [New Player Install Instructions](../Installation/index.md) - If mods aren't loading
