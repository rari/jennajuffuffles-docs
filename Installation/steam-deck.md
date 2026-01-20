---
title: Installing Collections on Steam Deck
description: Install Stardew Valley mod collections on Steam Deck. Learn how to transfer collections from Windows, set up SMAPI with Proton, and mod on Linux.
keywords: [Steam Deck, Steam Deck installation, Linux modding, Steam Deck mods, transferring to Steam Deck, Proton, Steam Deck SMAPI, Linux mods]
tags: [installation, steam-deck, linux, proton]
---

# Sideload to Steam Deck

*Last updated:* 2026-01-15  
*Applies to Stardew Valley:* 1.6.15+

This guide covers installing collections on Steam Deck. Since Vortex is Windows-only, you'll need to install the collection on a PC first, then transfer it to your Steam Deck. This process involves installing the collection on Windows, transferring files, and configuring SMAPI on the Steam Deck.

---

## Prerequisites

- A Windows PC with Vortex installed
- A USB drive or network connection to transfer files
- Stardew Valley installed on both PC and Steam Deck

{% hint style="danger" %}
You must use Hardlink deployment in Vortex. Softlinks cannot be copied in the same way, which will cause issues when transferring files to your Steam Deck.
{% endhint %}

---

## Installation Steps

### On PC: Install the Collection

1. Follow the [New Player Install Instructions](index.md) to install the collection using Vortex on your PC
2. Boot the game once on PC to verify mods deploy correctly
3. This ensures all mods are properly installed before transfer

### On PC: Prepare for Transfer

1. Browse local files: Right-click Stardew Valley in Steam > Manage > Browse local files
2. Copy the **Mods** folder to a USB drive or prepare for network transfer
3. Also copy any configuration files you've customized (usually in the Mods folder or game directory)

### On Steam Deck: Install Stardew Valley

1. Switch to **Desktop Mode** on your Steam Deck
2. Install Stardew Valley via Steam in Desktop Mode
3. Launch the game once to complete initial setup

### On Steam Deck: Install SMAPI

1. Install SMAPI for your game version: [SMAPI Installation Guide for Steam Deck](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Steam_Deck)
2. Follow the platform-specific instructions for Linux/Steam Deck
3. **Important:** Install the Linux/Proton version of SMAPI on Steam Deck - don't copy the Windows version from your PC

### On Steam Deck: Transfer Mods

1. Connect your USB drive or use network transfer
2. On Steam Deck, browse to your Stardew Valley game folder: Right-click Stardew Valley in Steam > Manage > Browse Local Files
3. Copy your **Mods** folder from PC into the Steam Deck game directory
4. Also copy any configuration files you transferred
5. Ensure the Mods folder is in the same location as the Stardew Valley executable

### On Steam Deck: Launch and Verify

1. Boot using `smapi.exe` (or the SMAPI launcher)
2. Confirm mods load correctly in the SMAPI console
3. Check for any errors in the SMAPI log

---

## Troubleshooting

### Mods not loading
- Verify SMAPI is properly installed for Steam Deck
- Check that all mod files transferred correctly
- Review the SMAPI log for specific errors

### Game won't start
- Ensure SMAPI is configured correctly for Steam Deck
- Verify game files are not corrupted
- Check SMAPI installation guide for Steam Deck-specific issues

### Performance issues
- Some mods may impact performance on Steam Deck
- Consider disabling resource-intensive mods if needed
- Check Steam Deck power settings

---

## See Also

- [New Player Install Instructions](index.md) - Install collections on PC first
- [Troubleshooting & FAQ](../Troubleshooting/index.md) - For additional help
- [SMAPI Steam Deck Guide](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Steam_Deck) - Official SMAPI installation
