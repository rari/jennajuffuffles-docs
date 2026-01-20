---
title: Using Stardrop Mod Manager
description: Transfer Stardew Valley collections from Vortex to Stardrop mod manager. Learn how to migrate collections and use Stardrop as an alternative mod manager.
keywords: [Stardrop, Stardrop mod manager, transferring to Stardrop, Stardrop migration, mod manager, Stardew Valley mod manager, collection migration]
tags: [installation, stardrop, mod-manager, migration]
---

# Sideload to Stardrop

*Last updated:* 2026-01-15  
*Applies to Stardew Valley:* 1.6.15+

Stardrop is an excellent mod manager designed specifically for Stardew Valley and is great for managing individual mods. However, because it doesn't support Nexus Collections directly, it's not recommended for collection users. If you want to use Stardrop with a collection, you'll need to install the collection through Vortex first, then fully migrate to Stardrop. This guide covers the migration process and Stardrop-specific setup requirements.

---

## Installation Instructions

For detailed installation instructions for your platform, please refer to the official Stardrop documentation:

- **Linux:** [Linux Installation Instructions](https://floogen.gitbook.io/stardrop/getting-started/installing-stardrop/linux)
- **macOS:** [macOS Installation Instructions](https://floogen.gitbook.io/stardrop/getting-started/installing-stardrop/macos)
- **Windows:** [Windows Installation Instructions](https://floogen.gitbook.io/stardrop/getting-started/installing-stardrop/windows)

Official Stardrop Documentation: [Installing Stardrop](https://floogen.gitbook.io/stardrop/getting-started/installing-stardrop)

> **Note:** [SMAPI (Stardew Modding API)](https://smapi.io/) must be installed separately. Stardrop does not install SMAPI for you.

---

## Transferring to Stardrop

Follow these steps to move your existing Vortex-managed setup to Stardrop.

{% hint style="danger" %}
Do not run two mod managers on the same game at the same time. You may corrupt installs. Make sure to stop managing Stardew Valley in Vortex before using Stardrop.
{% endhint %}

**Before you begin:** You must first install the collection using Vortex. Follow the [New Player Install Instructions](index.md) to download and install all mods before proceeding with these steps.

{% hint style="danger" %}
You must use Hardlink deployment in Vortex. Softlinks cannot be copied in the same way, which will cause issues when transferring to Stardrop.
{% endhint %}

### 1) Backup Your Mods
- Open your Stardew Valley/Mods folder
- Copy the entire folder to a safe backup (e.g., `C:\Backup\Mods`)

### 2) Stop Vortex Managing Stardew Valley
- Open Vortex
- Games tab > Stardew Valley > Stop Managing/Unmanage Game

### 3) Install SMAPI (if needed)
- Stardrop does not install SMAPI for you
- Download from https://smapi.io/ and install for your OS

### 4) Get Stardrop
- Download Stardrop (mod manager for SMAPI)
- Extract it somewhere convenient (e.g., Desktop)
- Launch once to ensure it reads your Mods folder

### 5) Launch via Stardrop
- Open Stardrop
- Verify SMAPI and mods are detected
- Launch the game from Stardrop

---

## See Also

- [New Player Install Instructions](index.md) - Install collections first using Vortex
- [Troubleshooting & FAQ](../Troubleshooting/index.md) - For non-Stardrop-specific issues
- [Manual Installation](manual.md) - Alternative installation method
