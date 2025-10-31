# Troubleshooting — Vortex

> 📂 Docs / Installation / Vortex / Troubleshooting

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* **1.6.15+**

This page focuses on troubleshooting Vortex-related setup issues for the collections.

---

## Quick Fix: Try Restarting First!

Before diving into complex troubleshooting steps, restart your computer and try again. Many issues with Vortex, SMAPI, or the game itself can be resolved with a simple restart.

---

## Part 1 — Game Installation Check (Game itself is healthy)

1. Use your store launcher to verify integrity of game files:
   - Steam: Library → Stardew Valley → Properties → Installed Files → Verify  
   - GOG: More → Manage Installation → Verify / Repair  
   - Xbox / Game Pass: Right-click game → Manage → Files → Verify and Repair

---

## Part 2 — Vortex Profile Check (Only collection mods selected)

1. On the Nexus Mods collection page, click Add Collection.
2. When prompted, install into a New Profile.
3. In Vortex, switch to that profile and confirm only the collection's mods are enabled.
4. Ensure Optional Mods are ticked for full functionality.

---

## Part 3 — Game Mods Folder Check (Only mods Vortex knows about)

1. In Vortex → Mods tab, click Purge to remove all active mods from the game folder.
2. Click Open → Game Mods Folder and manually delete any files/folders left behind.
3. Back in Vortex, click Deploy to put the clean set of mods back.

---

## Vortex-Specific Tips

- Set SMAPI as the Primary Tool in Dashboard; re-add if missing.  
- Manage Rules: ensure configuration/compat/translation mods load after the mods they affect; avoid Use Suggested if it creates loops.  
- After Deploy, confirm mods actually loaded in the SMAPI log (not just the Mods tab).  
- If a mod is missing: Redeploy, or delete the mod and its archive, then reinstall from the Collection tab.

---

## Need More Help?
- Community Discord: https://discord.com/invite/de2NrHXuty  
- Official Vortex Discord: https://discord.com/invite/nexusmods (Support hours: 9 AM – 5 PM GMT, Mon–Thu)

More help:  
- Vortex Wiki: https://wiki.nexusmods.com/index.php/Category:Vortex  
- Stardew Setup Guide: https://wiki.nexusmods.com/index.php/Modding_Stardew_Valley_with_Vortex

The official Stardew Valley Discord does not support Vortex.

---

## How to Create a SMAPI Log

Windows:
1. Press Windows+R  
2. Enter: `%appdata%\StardewValley\ErrorLogs`  
3. Open SMAPI-latest.txt (or SMAPI-crash.txt if it crashed)

Mac/Linux: visit https://smapi.io/log

Upload to https://smapi.io/log and share the link in Discord.

