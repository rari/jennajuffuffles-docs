# Install with Amethyst
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

Amethyst is a supported manager for these collections on Linux, including Steam Deck. It is not a Windows app.

Using a different manager? See [Install with Vortex](vortex.md) or [Install with Stardrop](stardrop.md).

## Install Amethyst

These steps follow the [Amethyst README](https://github.com/ChrisDKN/Amethyst-Mod-Manager).

The application may ask to set a password. This is for the OS keyring to store your Nexus API key, as Amethyst does not store it in a plain text file. Set the password to anything you want.

### AppImage

Run the following command in a terminal. It will appear in your applications menu under Games and Utilities.

```bash
curl -sSL https://raw.githubusercontent.com/ChrisDKN/Amethyst-Mod-Manager/main/src/appimage/Amethyst-MM-installer.sh | bash
```

Alternatively, download the AppImage from the [release page](https://github.com/ChrisDKN/Amethyst-Mod-Manager/releases) and install it with Gear Lever.

The application will notify you when a new update goes live. Pressing the update button will rerun the script and update to any new version.

### Alternative: Flatpak

Amethyst can also be installed as a Flatpak. AppImage is the recommended installation method for this guide.

For current Flatpak installation, update, and beta-branch instructions, see the [Amethyst README](https://github.com/ChrisDKN/Amethyst-Mod-Manager).

## Install a collection

Follow [Installing a collection](https://github.com/ChrisDKN/Amethyst-Mod-Manager/wiki/3.4-Installing-a-collection) in the Amethyst wiki for the buttons and windows. 

What Amethyst does with a Nexus collection:

- It downloads the collection and applies the curator's load order, bundled files, and mod diff patches.
- On the collection page you can change the revision before you install. When you install, Amethyst asks whether to make a new profile or append to an existing profile.
- Amethyst includes a wizard that installs SMAPI. You can also install SMAPI from [smapi.io](https://smapi.io/) for Linux before you play.
- Aesthetic Valley Fairycore and Aesthetic Valley Witchcore are mutually exclusive. Append one of them, not both. Enable only one farm map.

After the collection finishes installing, deploy your profile before launching Stardew Valley.

## Related

- [Update with Amethyst](../Update/amethyst.md)
- [Steam Deck](steam-deck.md)
- [Your SMAPI Log](../Troubleshooting/your-smapi-log.md)
- [Installing to an Existing Save](installing-to-an-existing-save.md)
