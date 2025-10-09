# Installation Guide

> 📂 **Docs** / [Start](/start.md) / **Installation Guide**

*Last updated:* 2025-08-10  
*Applies to Stardew Valley:* **1.6.15+**  

> 📖 This guide will be available right on the Nexus Collection page soon!

> ✔️ Always click **Install Optional Mods**  
> 🗑️ Always select **Remove All** when prompted during updates  
> ⬆️ Update the **collection**, never individual mods

---

## Prerequisites

1. Install **Stardew Valley** (Steam, GOG, or Game Pass).
2. Update your game to the [latest version](https://stardewvalleywiki.com/Version_History).
3. Verify game files:  
   - [Steam](https://support.steampowered.com/kb_article.php?ref=2037-QEUH-3335)  
   - [GOG](https://support.gog.com/hc/en-us/articles/360003930017)  
   - [Game Pass](https://support.xbox.com/help/games-apps/troubleshooting/troubleshoot-games-windows-10)  
4. Run the game once to finish initial setup.

---

## Setup Vortex for PC Users

Vortex is the recommended mod manager for svVe.  
**Important:** Enable **Symbolic Links** in Vortex settings if Stardew Valley is not installed on drive C:.

1. [Download and install Vortex Mod Manager](https://www.nexusmods.com/about/vortex/).
2. In Vortex, **Manage Stardew Valley** from the *Games* tab.

---

## PC Installation via Vortex

### 1. Clear Existing Mods
1. In Vortex **Mods** tab, click **Purge Mods**.
2. Click **Open → Game Mods Folder** and delete any leftover files.

### 2. Install the Collection
1. On the [collection page](https://next.nexusmods.com/stardewvalley/collections/tckf0m), click **Add Collection**.
2. Install into a **New Profile**.  
   > Nexus Premium users get auto-downloads. Free users follow manual prompts.
3. Configuration files will be automatically installed via FOMOD during collection installation.
4. Select **Install Optional Mods** when asked.

> **Important:** Always use Optional Mods unless you're using *Stardew Valley Very Expanded + Aesthetic Valley*. In that case, use optional mods from **only one** collection to avoid conflicts. See: [Combining Collections](/combining.md)

### 3. Pre-Launch Setup
1. Install & configure [SMAPI](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Windows#Configure_your_game_client).
2. In Vortex Dashboard, confirm SMAPI is set as the primary tool.
3. Click **Deploy**.
4. Launch the game from Vortex via SMAPI.

---

## Steam Deck Installation

1. Install Stardew Valley via Steam in **Desktop Mode**. Verify integrity.
2. Transfer your modded game files from PC to Deck via USB or network.
3. Install SMAPI for your game version: [Guide](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Steam_Deck).
4. Add SMAPI as a Non-Steam Game in Steam and configure it for the correct compatibility mode.
5. Launch via SMAPI and confirm mods load.

---

## Mac Installation

1. Download mods manually from the Collection's *Mods* tab.  
2. Configuration files are now distributed as FOMOD installers for each collection. All configuration folders can be found in the "files" folder of each collection's FOMOD. Merge the configuration folders into your mods folder (Option + drag to merge).  
5. Verify mod placement and launch the game.

### MacOS SMAPI Security Issues

**Important:** Certain MacOS versions flag SMAPI as malware and forcibly move it to the trash, preventing installation.

*The following solutions are based on community findings and may change as Apple updates MacOS security behaviors.*

#### Problem 1: Unable to Run SMAPI Installer
**Solution:** When you receive a security message, go to Settings → Security (or Privacy & Security) and hit "Open Anyways" where it lists the blocked file.

#### Problem 2: MacOS reports "Malware Blocked and Moved to Trash"
**Solution:** Enable MacOS security permissions:

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

## Mod Configuration

- Configuration files are automatically installed via FOMOD during collection installation.
- Vortex auto-deploys the recommended settings.
- If installing manually, merge configuration files from the "files" folder of the collection's configuration fomod.
- Adjust in-game via **GMCM** (gear icon on the title screen).
- For co-op: all players should match configurations.
- Want to customize further? See our [Personalization & Custom Configurations](/personalization.md) guide.

### Reinstalling Configurations

If you need to reinstall configuration files at any time:
1. In Vortex, right-click on the collection's FOMOD file
2. Select **"Reinstall"** from the context menu
3. This will provide a fresh installation of all configuration files

---

## Updating the Collection

For detailed updating instructions, see our [**Updating Collections**](/updating.md) guide.

**Quick Summary:**
- Collections will show an **Update** button when an update is available
- If using the update button, always select **Remove All** when prompted
- Do **not** update individual mods

---

## Combining with Aesthetic Valley Collections

When combining, always let the **matching recolor or style config load last** in Vortex Rules Manager.

### Witchcore — Disable:
- Seasonal Vanilla UI  
- Lumisteria Short Flowery Grass  
- Immersive Farm 2 Remastered  

### Fairycore — Disable:
- Seasonal Vanilla UI  
- Grandpa's Tools  
- Immersive Farm 2 Remastered  
- Lumisteria Short Flowery Grass  

If using **Immersive Farm 2 Remastered**, disable its Greenhouse option in GMCM.

---

## Quick Links

- [Start Page](/start.md)  
- [Installation Guide](/install.md)  
- [Manual Installation Guide](/manual-install.md)  
- [Updating Collections](/updating.md)  
- [Combining Collections](/combining.md)  
- [Personalization & Custom Configurations](/personalization.md)  
- [Keybinds & Controllers](/keybinds.md)  
- [Troubleshooting](/troubleshooting.md)  
- [FAQ & Known Issues](/faq-and-known-issues.md)  

