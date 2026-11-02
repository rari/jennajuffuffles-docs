# Install with Stardrop
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

Stardrop is a supported manager for JennaJuffuffles collections. It is built for Stardew Valley and runs on Windows, Linux, and macOS.

{% hint style="info" %}
Currently, Stardrop does not support stacking collections. This may change in the future!
{% endhint %}

Using a different manager? See [Install with Vortex](vortex.md) or [Install with Amethyst](amethyst.md).

## Install a collection

Use a current [Stardrop release](https://github.com/Floogen/Stardrop/releases). Collection install is included.

1. Install SMAPI from [smapi.io](https://smapi.io/) for your operating system. Connect SMAPI to your store launcher so you can launch from the store, keep achievements, and play co-op. See [Connecting SMAPI to Your Store](vortex.md#connecting-smapi-to-your-store) for Steam, GOG Galaxy, and Xbox App steps, or the [SMAPI client setup](https://stardewvalleywiki.com/Modding:Installing_SMAPI_on_Windows#Configure_your_game_client) on the wiki.
2. Download Stardrop from the [release page](https://github.com/Floogen/Stardrop/releases). Extract it to the location suggested in the [official install guide](https://floogen.gitbook.io/stardrop/getting-started/installing-stardrop) for your operating system.
3. Launch Stardrop and follow the startup wizard.
4. Open **Nexus Mods** > **API Connection**. Create or copy your key from [Nexus Mods API keys](https://www.nexusmods.com/settings/api-keys), or follow Stardrop's [API connection guide](https://floogen.gitbook.io/stardrop/guides/nexus-mods-integration/connecting-to-nexus-mods-api).
5. Download a collection. Stardrop can install it once the API key is connected.

**Update** and **Delete** for each collection are under **Nexus Mods** > **Collection**.

## What a collection install does

- Each collection downloads into its own folder.
- Stardrop creates a protected profile for that collection, with the collection's mods enabled.
- Do not edit that protected profile directly. Clone it when you want your own changes.
- A second collection creates a second protected profile. It does not merge into the first.
- Files Stardrop cannot fetch for you (non-Nexus files, or Nexus files when you are not a Premium member) are gathered into one manual-download list. Free Nexus users finish those downloads from that list.

## Moving an existing Vortex install

Use this when the collection is already installed with Vortex and you want Stardrop to manage those files. Prefer installing the collection in Stardrop when you can. A copied Mods folder is not a Stardrop collection install.

Do not run two mod managers on the same game at the same time. Stop managing Stardew Valley in Vortex before you use Stardrop.

{% hint style="danger" %}
Use hardlink deployment in Vortex before you copy. Softlinks often break when copied, and Stardrop then sees empty mod folders.
{% endhint %}

If you switch between managers, **Register** or **Remove NXM Association** is about halfway down **View** > **Settings** in Stardrop. Restart the computer after you change that setting.

1. Install the collection with [Install with Vortex](vortex.md) first.
2. Copy your Stardew Valley **Mods** folder to a backup.
3. In Vortex, open the **Games** tab, select Stardew Valley, and stop managing the game.
4. Confirm SMAPI is installed for your operating system and connected to your store.
5. Download Stardrop, extract it, and launch it once so it can read the Mods folder.
6. Open Stardrop, confirm SMAPI and the mods are detected, and launch the game from Stardrop.

Collection updates in [Update with Stardrop](../Update/stardrop.md) apply only to a collection Stardrop installed, not to a folder you copied out of Vortex.

## Related

- [Update with Stardrop](../Update/stardrop.md)
- [Install with Vortex](vortex.md)
- [Your SMAPI Log](../Troubleshooting/your-smapi-log.md)
- [Installing to an Existing Save](installing-to-an-existing-save.md)
