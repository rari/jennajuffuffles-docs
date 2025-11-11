# FAQ & Known Issues

> 📂 Docs / Getting Started / FAQ & Known Issues

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* **1.6.15+**

---

> **Not finding the answers you need here?** Check out our [Troubleshooting Guide](../Guides/troubleshooting.md) for comprehensive troubleshooting resources and guides.

---

## Getting Started FAQs

### Do I need the optional mods?
> Yes! While some mods are marked as "optional" to make it easier when combining collections, you should install them when using a single collection. These optional mods include:
> - Essential interface improvements 
> - Map enhancements that improve the visual experience
> - Additional content that enhances gameplay
> - Expansions that have been carefully curated for quality
> - Compatibility files for combining collections (only needed when stacking multiple collections)
> 
> The optional designation exists mainly to help with collection stacking (combining multiple collections). When using just one collection, these mods are designed to be part of the intended experience.

### Should I update individual mods myself?
> No. Always wait for the collection to be updated instead of updating individual mods yourself. The collection curator tests all mod versions together to ensure compatibility. Updating mods individually can cause version conflicts, breaking changes, missing compatibility patches, and unstable gameplay. When a collection update is released, it includes tested versions of all mods that work together.

### Can I combine your collections?
> Yes! Any Aesthetic Valley collection (Fairycore, Witchcore, or future Aesthetic Valley collections) is designed to work alongside Stardew Valley VERY Expanded (svVe). You can install them into the same Vortex profile.
> 
> For detailed instructions on how to combine collections, including which optional mods to install and how to manage conflicts, see our [Combining Collections](../Collections/combining-collections.md) guide.

### Can I play svVe if I haven't played Stardew Valley before?
> It's absolutely fine to start with svVe even if you're new to Stardew Valley! The collection is designed to enhance the game while preserving the vanilla feel. However, keep in mind that svVe is quite large with many new areas, NPCs, and content.
> 
> **Recommendation:** Playing vanilla Stardew Valley first will help you appreciate the additions svVe brings, but it's not required. If you're eager to dive in with the collection, go for it - just be prepared for a lot more content to explore!

### Co-op
> All players in a multiplayer game must have matching mods and configurations for everything to work correctly. This means:
> - All players need the same collection(s) installed
> - All players need the same mod versions
> - All players need matching configurations (especially for mods that affect gameplay)
> 
> Consider using a multiplayer manager or keeping careful documentation of your mod setup so everyone can stay in sync. Version mismatches can cause desyncs, crashes, or missing content.

### Where can I download these collections?
> These collections are only available and updated through **Nexus Mods**. This is the official source and ensures you always get the latest tested versions. All collections must be installed through Nexus so each mod download is properly attributed to its creator.
> 
> Using **Nexus Premium** helps support Nexus Mods and the mod creators on the platform. Nexus Premium also enables one-click installation through the support mod managers, making collection setup much easier and faster. However, you can still use Vortex or Nexus Mods App for free to download and install - it just requires a bit more clicking.

### Can I get all the mods in a zip file?
> No. Collections are not modpacks. Providing a downloadable zip file with all mods would be redistributing mods without creators' permission, which is mod piracy. Collections must be installed through Nexus so each mod download is properly attributed to its creator. This respects creators' rights and ensures they receive proper credit and support for their work.

### Why is my game loading slowly?
> Large collections can take several minutes to load, especially on the first launch or when starting a new save. This is normal due to the amount of content being loaded.
> 
> **⚠️ Important:** During loading, please don't alt-tab, click away, or interact with the game window. Doing so can cause crashes or freezes. Just let it load - you'll see progress in the SMAPI console window. The game will be ready when the console stops showing loading messages.

### Mobile support
> The status of mobile support can change rapidly. We recommend trying with the [1.5.6 version collection](https://www.nexusmods.com/games/stardewvalley/collections/9sf9yn), but support is not guaranteed or known. Mobile modding has significant limitations and compatibility issues that may prevent collections from working properly. Stardew Valley on iOS cannot be modded. 

---

## Gameplay FAQs

For svVe-specific gameplay questions including Community Center cutscenes, Rusty/Sewer Key changes, minecart blocking the mine entrance, duplicated NPCs, East Scarp festival attendance, crafting issues, and performance problems, see the [svVe FAQ](../Collections/Stardew%20Valley%20VERY%20Expanded/faq.md).

### Can't exit house / corrupted farm map
> If you find yourself unable to exit your house or see a corrupted farm map (missing textures, black areas, or errors), this usually means your farm map mod is disabled or failed to load properly.
> 
> To fix this:
> 1. Open your mod manager 
> 2. Find your farm map mod 
> 3. Make sure it's **Enabled** 
> 4. Check that no other farm map mods are enabled - only one farm map should be active at a time
> 5. Click **Deploy** to apply the changes
> 6. Restart the game and load your save
> 
> **Important:** Farm maps cannot be switched mid-save without special tools. If you want to change your farm map, you'll need to start a new save file, or use a tool like [Easy Farm Switcher](https://www.nexusmods.com/stardewvalley/mods/16873) which can handle the transition (though this should be done carefully and with backups).

---

## Setup & Customization FAQs

### Can I add more mods?
> Yes! These collections are designed as solid bases that you can build upon. However, there are some important things to keep in mind:
> 
> - **Test additions individually** - Add one mod at a time and test thoroughly before adding another. This helps you identify any conflicts quickly.
> - **Review compatibility notes** - Check mod pages for compatibility warnings, especially with major expansions like SVE, Ridgeside Village, or East Scarp.
> - **Create a private collection** - Once you've found mods that work well, create a private collection containing just your additions. This makes it easy to reinstall them after collection updates. See our [Personalization guide](../Guides/personalization.md) for details.
> - **Check load order** - Some mods may need specific load orders. Use Vortex's "Manage Rules" to adjust if needed.
> 
> Remember that adding mods can introduce conflicts or bugs, and collection updates may not account for your additions. Keep backups of working configurations!

### Can I disable a required mod?
> You can disable a required mod, but it requires manual management since the collection expects it to be enabled.
> 
> **For Vortex users:**
> 1. Go to the **Mods** tab
> 2. Find the mod you want to disable and toggle it off
> 3. The collection will show a warning - this is expected
> 4. Click **Deploy** to apply the change
> 
> **Tip:** Add the **Collections** column in Mod view to help track which mods belong to which collection. This makes it easier to see what you've modified and manage visibility.
> 
> **For Nexus Mods App users:**
> You'll need to create a collection clone to disable required mods, as NMA doesn't allow disabling required mods directly in a collection. Create a clone of the collection and modify it to remove or disable the required mods you don't want.
> 
> **Warning:** Disabling required mods can break functionality, cause crashes, or create gameplay issues. Only disable mods if you understand what they do and are prepared to troubleshoot problems. Some mods are required because others depend on them.

---

## Installation-Specific FAQs
For mod-manager-specific questions and troubleshooting:

- [Vortex FAQ & Troubleshooting](../Installation/Vortex/troubleshooting.md)
- [Nexus Mods App FAQ & Common Issues](../Installation/NMA/faq.md)
- [Stardrop FAQ & Common Issues](../Installation/Stardrop/faq.md)
- [Manual Installation FAQ & Limitations](../Installation/Manual/faq.md)

---

### MacOS Installation

#### Mod Managers
> Nexus Mods App has planned support for MacOS, but currently no mod manager with collection support exists. Mac users may use our [Manual Installation](../Installation/Manual/installation.md) guide or our [Stardrop](../Installation/Stardrop/installation.md) guides and transfer from a Windows machine.

#### MacOS SMAPI Security Issues

> **Important:** Certain MacOS versions flag SMAPI as malware and forcibly move it to the trash, preventing installation.
> 
> *The following solutions are based on community findings, derivded from the Stardew community Discord, and may change as Apple updates MacOS security behaviors.*

#### Problem 1: Unable to Run SMAPI Installer
> When you receive a security message, go to Settings → Security (or Privacy & Security) and hit "Open Anyways" where it lists the blocked file.

#### Problem 2: MacOS reports "Malware Blocked and Moved to Trash"
> Enable MacOS security permissions:
> 
> 1. Go to System Settings > Privacy and Security
> 2. Make sure Developer Tools is visible. If you don't see it, open Terminal through Spotlight and enter:
>    ```
>    spctl developer-mode enable-terminal
>    ```
> 3. Click Developer Tools
> 4. Add Terminal to the list and enable it
> 5. If you have other terminal programs (iTerm2, Hyper, Kitty, Alacritty), add them to Developer Tools as well
> 6. Restart your computer
> 7. Force close Steam if using it
> 8. Download and reinstall SMAPI
> 
> **Note:** This solution may change over time as Apple updates MacOS security behaviors. If this doesn't work:
> - Restart your computer again
> - Force close Steam, then try installing SMAPI
> - Check the [SMAPI Mac installation wiki](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Mac) for updated solutions
> 
> *For the most current solutions and community discussions, visit the the [SMAPI GitHub repository](https://github.com/Pathoschild/SMAPI).*

---

For Vortex-specific troubleshooting, see the [Vortex Troubleshooting](../Installation/Vortex/troubleshooting.md) guide.

---

## Known Technical Issues

### Multiplayer / split-screen desync
> If you experience desynchronization in multiplayer (players seeing different things, actions not registering, or players getting stuck), this is usually a temporary network or mod state issue.
> 
> **Note:** Split-screen co-op may exhibit unusual behavior while modded. Feedback via [Discord](https://discord.gg/MPcgJUXeeY) is always appreciated to help improve mod compatibility with split-screen multiplayer.
> 
> Quick fixes to try:
> 1. **Relaunch the game** - All players should quit and restart the game completely
> 2. **Restart the session** - The host should save, close the game, and start a new multiplayer session
> 3. **Check mod sync** - Ensure all players have the exact same mods enabled and the same versions
> 4. **Verify configurations match** - Important mod configurations should be identical across all players
> 
> Persistent desync issues may indicate mod conflicts or version mismatches. Check the SMAPI logs from all players for errors.

### Failed to Store Cache Entry (SinZational Speedy Solutions)
> This error message appears in your SMAPI log related to SinZational Speedy Solutions, but **it's completely safe to ignore**. It's an informational message, not an actual error.
> 
> - It does **not** indicate a crash or conflict
> - It does **not** affect gameplay
> - Your game will run normally despite this message
> - No action is needed
> 
> This is communicating that the mod failed to cache the map, but functionally this means the map still will load normally. You can safely continue playing!

### Is JennaJuffuffles affiliated with Nexus Mods?
> No. JennaJuffuffles is an independent collection curator and is not affiliated with or employed by Nexus Mods. As such, JennaJuffuffles is not responsible for:
> - Changes to the Nexus Mods website or platform
> - How Nexus Premium works, its pricing, or its features
> - Issues with Nexus Mods services, servers, or account access
> - Mod manager updates or changes (Vortex, Nexus Mods App, etc.)
> - Decisions made by Nexus Mods or its staff
> 
> For questions or issues related to Nexus Mods services, account access, Premium subscriptions, or platform features, please contact [Nexus Mods Support](https://help.nexusmods.com/).



---

## Getting Help

- [Community Discord](https://discord.gg/MPcgJUXeeY)
- [Vortex Support Discord](https://discord.com/invite/nexusmods)
- [Vortex Wiki](https://wiki.nexusmods.com/index.php/Category:Vortex)

