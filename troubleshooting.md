# Troubleshooting

> 📂 **Docs** / [Start](/start.md) / **Troubleshooting**

*Last updated:* 2025-08-14  
*Applies to Stardew Valley:* **1.6.15+**

> 📖 This guide will be available right on the Nexus Collection page soon!

---

## 🚀 Quick Fix: Try Restarting First!

Before diving into complex troubleshooting steps, **restart your computer** and try again. Many issues with Vortex, SMAPI, or the game itself can be resolved with a simple restart. This is often the fastest solution and can save you a lot of time!

---

## **Part 1 — Vortex Profile Check** *(Only collection mods selected)*

1. On the [Nexus Mods collection page](https://next.nexusmods.com/stardewvalley/collections/tckf0m), click **Add Collection**.
2. When prompted, install into a **New Profile**.
3. In Vortex, switch to that profile and confirm **only the collection's mods are enabled** (no leftovers or personal add-ons).
4. Ensure **Optional Mods** are ticked for full functionality.

---

## **Part 2 — Game Mods Folder Check** *(Only mods Vortex knows about)*

5. In Vortex → **Mods** tab, click **Purge** to remove all active mods from the game folder.
6. Click **Open → Game Mods Folder** and manually delete any files/folders left behind.
7. Back in Vortex, click **Deploy** to put the clean set of mods back.

---

## **Part 3 — Game Installation Check** *(Game itself is healthy)*

8. Use your store launcher to **verify integrity** of game files (fast reinstall):

   * **Steam:** Library → Stardew Valley → Properties → Installed Files → Verify  
   * **GOG:** More → Manage Installation → Verify / Repair  
   * **Xbox / Game Pass:** Right-click game → Manage → Files → Verify and Repair

---

## 💬 Need More Help?

If you run into issues that aren't solved here, you can:
- Reach out to our community on **[Discord](https://discord.com/invite/de2NrHXuty)** for live assistance.
- Create and share a SMAPI log so others can help diagnose your issue.

## 💬 Further Support

💬 For Vortex support:
- **Official Vortex Discord**: [Join Here](https://discord.com/invite/nexusmods)
- **Support Hours**: 9 AM – 5 PM GMT, Monday–Thursday

📚 More help available:
- **Vortex Wiki**: [Read Here](https://wiki.nexusmods.com/index.php/Category:Vortex)
- **Stardew Setup Guide**: [Read Here](https://wiki.nexusmods.com/index.php/Modding_Stardew_Valley_with_Vortex)

🚫 The **official Stardew Valley Discord** does *not* support Vortex. Please respect their policy.

---

## 📚 Additional Resources for Expansion Mods

If you're experiencing issues with specific expansion mods, these resources may help:

### Stardew Valley Expanded
- [Installation Guide](https://github.com/FlashShifter/StardewValleyExpanded/wiki/Install-guide)
- [Troubleshooting](https://github.com/FlashShifter/StardewValleyExpanded/wiki/Troubleshooting)
- [Wiki](https://stardew-valley-expanded.fandom.com/wiki/Stardew_Valley_Expanded_Wiki)
- [Discord](https://discord.com/invite/svexpanded)

### Ridgeside Village & Lunna
- [Installation Guide](https://github.com/Rafseazz/Ridgeside-Village-Mod/blob/main/Installation%20Guide.md)
- [Wiki](https://ridgeside.fandom.com/wiki/Ridgeside_Village_Wiki)
- [Discord](https://discord.gg/4SRbjEQG2D)

### East Scarp & Lurking in the Dark, Sword & Sorcery, etc
- [Wiki](https://eastscarp.fandom.com/wiki/East_Scarp_Wiki)
- [Discord](https://discord.com/invite/QFtDA3CJwJ)

⚠️ **Important:** Please avoid troubleshooting in these Discords unless you can show (via log) a repeatable error from their mod without the rest of the collection active.

---

## 📄 How to Create a SMAPI Log

**Don't worry, this is easier than it sounds!** A SMAPI log is just a text file that shows what mods loaded and any errors that occurred.

### Windows Users:
1. Press the **Windows** and **R** keys at the same time.
2. In the 'Run' box that appears, enter:
   ```
   %appdata%\StardewValley\ErrorLogs
   ```
3. Look for one of these files:
   - `SMAPI-crash.txt` (if the game crashed)
   - `SMAPI-latest.txt` (normal log from your last game session)

### Mac/Linux Users:
Visit [smapi.io/log](https://smapi.io/log) for platform-specific instructions.

### What to do with your log:
1. Upload it to [smapi.io/log](https://smapi.io/log) 
2. Share the link in our [Discord](https://discord.gg/de2NrHXuty) for help!

**💡 Tip:** The log will show exactly which mods loaded successfully and highlight any problems in red.

---

## 📚 Quick Links

- 🌾 [Start Page](/start.md)  
- 🚀 [Installation Guide](/install.md)  
- 🧩 [Manual Installation Guide](/manual-install.md)  
- 🔀 [Combining Collections](/combining.md)  
- 🎮 [Keybinds & Controllers](/keybinds.md)  
- 🛠️ [Troubleshooting](/troubleshooting.md)  
- ❓ [FAQ & Known Issues](/faq-and-known-issues.md)