# Vortex — FAQ & Common Issues

> 📂 Docs / Installation / Vortex / FAQ

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* **1.6.15+**

---

## FAQ

### Can I use Vortex with another mod manager?
Do not run two mod managers on the same game simultaneously — you may corrupt installs.

### Where should I install Stardew Valley and Vortex?
For best results, it's recommended to install both Stardew Valley and Vortex on `C:\`. This helps avoid potential issues with symbolic links and deployment.

---

## Common Issues

### Unresolved file conflicts (Manage Rules)
Ensure compatibility/config/translation mods load after the mods they affect. Open Mods → Manage Rules, set the relationship, then Deploy. Avoid "Use Suggested" if it creates loops.

### Updates can overwrite/delete custom configs
Use the Sync Mod Configurations button (recommended) or create a custom config mod that loads after targets. See Personalization: [Personalization & Custom Configurations](../../Guides/personalization.md)

### Mod staging may fail silently
After Deploy, verify in the SMAPI log that the mod actually loaded (don’t rely only on the Mods tab). If missing, Redeploy, or delete the mod and its archive, then reinstall from the Collection tab.

### Mods with incorrect folder structure
Some manual additions have improper layouts and won’t deploy correctly. Fix structure per the official wiki, then Deploy.

### Red errors from an empty Vortex folder
Often due to leftover folders from disabled mods, or installing configuration without associated mods. Non-harmful; enable the recommended files or customize configs.

### SMAPI not launching via Vortex
Dashboard → set SMAPI as Primary Tool; re-add if missing. Confirm the path and re-Deploy.

### Best practices for combining collections
Install to the same profile. Let the chosen recolor/theme config load last in Rules Manager. See Combining Collections: [Combining Collections](../../Collections/combining-collections.md)

