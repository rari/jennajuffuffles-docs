# Steam Deck
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

## Amethyst on Steam Deck

Use this when Amethyst installs and manages the collection on the Deck.

1. Switch to **Desktop Mode**.
2. Install Stardew Valley from Steam if it is not already installed. Launch it once, then quit.
3. Set the game to the **Linux** build (no Proton): **Stardew Valley** > **Properties** > **Compatibility**, and disable "Force the use of a specific Steam Play compatibility tool." Amethyst is a Linux manager. Proton is not the usual path here.
4. Install Amethyst. Open a terminal in Desktop Mode and run the AppImage command from [Install with Amethyst](amethyst.md). Amethyst appears under Games and Utilities. You can add it to Steam if you want to open it from Gaming Mode.
5. Use Amethyst's SMAPI wizard, or install Linux SMAPI from [smapi.io](https://smapi.io/) / the [SMAPI Steam Deck guide](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Steam_Deck) for the Linux runtime.
7. Launch **Stardew Valley from Steam**. Do not double-click `StardewModdingAPI.exe`. Check [Your SMAPI Log](../Troubleshooting/your-smapi-log.md).

---

## Quick answers

**Do I run `StardewModdingAPI.exe` directly?** No. After SMAPI is installed, launch **Stardew Valley from Steam**. SMAPI attaches automatically.

**Linux or Proton?** For Amethyst, use the **Linux** build. 

**Co-op with a PC or Mac?** Mod **content** is cross-platform, but each player needs SMAPI installed locally and the same mod versions and configs. See [About the Collections](../Reference/about-the-collections.md#multiplayer-support).

---

## Troubleshooting

### Nothing happens when I open `StardewModdingAPI.exe`

You should not launch SMAPI manually. Start the game from **Steam**. If SMAPI is installed correctly, it runs when Stardew starts.

### Mods missing or SMAPI shows an empty mod list

- Confirm **Mods** is in the folder for your runtime (see the table above). Linux uses `~/.local/share/StardewValley/Mods`, not only the Steam game directory.
- Confirm **runtime and SMAPI match** (Linux + Linux SMAPI, or Proton + Proton/Windows SMAPI).
- Reinstall SMAPI after changing Proton settings.
- Verify every mod folder copied completely from PC (no broken symbolic links).

### Game won't start

- Re-run the [SMAPI Steam Deck guide](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Steam_Deck) for your runtime
- Verify game files in Steam: **Properties** > **Installed Files** > **Verify**
- Check the SMAPI log for red errors

### Linux-specific log errors

If your SMAPI log shows **`Failed parsing new quests.`**, install [Ridgeside Village Quest Fix For Linux and Mac](https://www.nexusmods.com/stardewvalley/mods/36004). See [Mod-Specific Known Issues](../Troubleshooting/mod-specific-known-issues.md) for more context.

### Performance issues

- Large collections can be heavy on Steam Deck; lower in-game settings if needed
- Disable optional performance-heavy mods if you added any
- Check Steam Deck power settings in Gaming Mode

---

## Related

- [Install with Amethyst](amethyst.md)
- [Install with Vortex](vortex.md)
- [Your SMAPI Log](../Troubleshooting/your-smapi-log.md)
- [Launch Problems](../Troubleshooting/launch-problems.md)
