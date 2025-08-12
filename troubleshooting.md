# Troubleshooting

> 📂 **Docs** / [Start](/start.md) / **Troubleshooting**

*Last updated:* 2025-08-12  
*Applies to Stardew Valley:* **1.6.15+**

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
- Reach out to our community on **[Discord](https://discord.gg/de2NrHXuty)** for live assistance.
- Create and share a SMAPI log so others can help diagnose your issue.

## 📄 How to Create a SMAPI Log

1. Press the **Windows** and **R** keys at the same time.
2. In the 'Run' box that appears, enter:
```
%appdata%\StardewValley\ErrorLogs
```
3. The log file will be:
   - `SMAPI-crash.txt` if it exists  
   - Otherwise: `SMAPI-latest.txt`

Upload the log to [smapi.io/log](https://smapi.io/log) and share the link.

---

<!-- ## 📚 Quick Links

- 🌾 [Start Page](/start.md)  
- 🚀 [Installation Guide](/install.md)  
- 🧩 [Manual Installation Guide](/manual-install.md)  
- 🔀 [Combining Collections](/combining.md)  
- 🎮 [Keybinds & Controllers](/keybinds.md)  
- 🛠️ [Troubleshooting](/troubleshooting.md)  
- ❓ [Known Issues & FAQ](/known-issues-and-faq.md)

-->
