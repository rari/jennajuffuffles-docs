# Stardrop

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* 1.6.15+

---

Stardrop is an excellent mod manager designed specifically for Stardew Valley and is great for managing individual mods. However, because it doesn't support Nexus Collections directly, it's not recommended for collection users. 

If you want to use Stardrop with a collection, you'll need to install the collection through Vortex first, then migrate to Stardrop. See [Transferring to Stardrop](#transferring-to-stardrop) for migration instructions. Ensure SMAPI is installed and configure mods via GMCM.

---

## Installation Instructions

For detailed installation instructions for your platform, please refer to the official Stardrop documentation:

- **Linux:** [Linux Installation Instructions](https://floogen.gitbook.io/stardrop/getting-started/installing-stardrop/linux)
- **macOS:** [macOS Installation Instructions](https://floogen.gitbook.io/stardrop/getting-started/installing-stardrop/macos)
- **Windows:** [Windows Installation Instructions](https://floogen.gitbook.io/stardrop/getting-started/installing-stardrop/windows)

Official Stardrop Documentation: [Installing Stardrop](https://floogen.gitbook.io/stardrop/getting-started/installing-stardrop)

> **Note:** [SMAPI (Stardew Modding API)](https://smapi.io/) must be installed separately. Stardrop does not install SMAPI for you.
---

## FAQ

### Can I use Stardrop with another mod manager?
> Do not run two mod managers on the same game at the same time. You may corrupt installs. 

---

## Transferring to Stardrop

Follow these steps to move your existing Vortex-managed setup to Stardrop.

**Before you begin:** You must first install the collection using Vortex. Follow the [Vortex Installation Guide](Vortex/installation.md) to download and install all mods before proceeding with these steps. **Hardlink must be used.**

### 1) Get Stardrop
- Download Stardrop (mod manager for SMAPI)
- Extract it somewhere convenient (e.g., Desktop)
- Launch once to ensure it reads your Mods folder

### 2) Backup Your Mods
- Open your Stardew Valley/Mods folder
- Copy the entire folder to a safe backup (e.g., `C:\Backup\Mods`)

### 3) Stop Vortex Managing Stardew Valley
- Open Vortex
- Games tab > Stardew Valley > Stop Managing/Unmanage Game

### 4) Restore Your Mods
- Return to your original Mods directory
- Copy your backup back into Mods
- Do not include `VortexDeployment.json`

### 5) Install SMAPI (if needed)
- Stardrop does not install SMAPI for you
- Download from https://smapi.io/ and install for your OS

### 6) Launch via Stardrop
- Open Stardrop
- Verify SMAPI and mods are detected
- Launch the game from Stardrop

---

## See Also

- [Mod Managers Overview](index.md) - To compare with other mod managers
- [Vortex Installation](Vortex/installation.md) - If you need to install collections first
- [Troubleshooting & FAQ](../../Guides/troubleshooting.md) - For non-Stardrop-specific issues
- [Manual Installation](manual.md) - Alternative installation method
- [NMA Guide](nma.md) - Beta collection installation option (not recommended) 

