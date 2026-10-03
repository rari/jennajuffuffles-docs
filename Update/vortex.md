# Update with Vortex
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

{% hint style="danger" %}
Update the collection, not individual mods. Collections are tested together. Updating individual mods outside a collection revision can cause unexpected behavior.
{% endhint %}

These steps are Vortex-only. [Update with Stardrop](stardrop.md) and [Update with Amethyst](amethyst.md) work differently.

## Before You Update

Taking a few minutes to prepare will make the update process smooth and worry-free:

* **Back up your saves** - Your saves are precious! See the [Stardew Valley Wiki Saves page](https://stardewvalleywiki.com/Saves) for how to back them up. This takes just a moment and gives you peace of mind.
* **Note your custom settings** - If you've customized any mod configurations, you might want to note them down or back them up. See [Adjusting Configurations](../Customize/adjusting-configurations.md) for the Vortex steps.
* **Check collection changelog** - Review what's changed in the update to know what to expect

***

## Updating Collection (Profile With No Extra Mods Installed)

1. On the Collections tab in Vortex, remove the collection (but do not check any checkboxes, mods and archives should remain.)
2. Visit the collection's Nexus page and click Add To Vortex
3. If installing more than one collection, install the first to a new profile (default behavior) and then the rest to the same. You can select this at the bottom of the first pop-up.
4. After collection is installed, disable the collection and then re-enable the collection, selecting the 'recommended mods' to ensure they are re-enabled properly (since updating often disables them)

{% embed url="https://youtu.be/AfxLEZAj_NI" %}

## Updating Collection (Profile With Extra Mods Installed)

1. Disable the collection, then check the 'recommended mods' option in the pop-up and click ok. This should disable all mods that are part of the collection from your profile.
2. On the Collections tab in Vortex, remove the collection (but do not check any checkboxes, mods and archives should remain.)
3. Visit the collection's Nexus page and click Add To Vortex
4. At the bottom of the pop-up, select current profile, then click ok on pop-up.
5. When prompted, select to replace, not create variations.
6. After collection is installed, disable the collection and then re-enable the collection, selecting the 'recommended mods' to ensure they are re-enabled properly (since updating often disables them)

{% hint style="info" %}
If this process is not successful, please follow the instructions for "Profile with No Extra Mods Installed" and then re-enable your additional mods.
{% endhint %}

## Alternative Update Method (Not Recommended)

1. In Vortex, go to the **Collections** tab
2. Find your collection in the list
3. Click the **Update** button (or look for an update notification)
4. Follow the prompts to update the collection
5. When prompted during updates, choose **Replace existing file** for consistency
6. **Important:** When Vortex asks to remove mods, allow it to remove them. Failure to remove can result in duplicates that will prevent either mod from loading
7. Click **Deploy** after the update completes

When using this method...

* You may see pop-ups for each mod asking how to handle updates - this is normal for large collection updates
* Choose **Replace existing file** for each mod to ensure consistency
* If asked to remove a mod, do so. This typically means the old file needed to be removed to install the new version.


***

## Common Update Issues

### Mods Not Loading After Update

* Verify the collection was properly updated in Vortex
* Check that all recommended mods are enabled
* Try disabling and re-enabling the collection (with recommended mods selected)
* See [Vortex Notifications and Solutions](../Troubleshooting/vortex-notifications.md) for detailed steps

### Custom Configurations Lost

* Custom configs may be overwritten during updates
* See [Adjusting Configurations](../Customize/adjusting-configurations.md) for the Vortex steps to protect your custom settings

### Game Won't Start After Update

* Verify game files through your store launcher
* Check [Your SMAPI Log](../Troubleshooting/your-smapi-log.md) for errors
* See [Launch Problems](../Troubleshooting/launch-problems.md) if the game will not start

***

## After Updating

* **Test your game** - Load a save and verify everything works correctly
* **Check SMAPI log** - Look for any new errors or warnings
* **Review changelog** - See what's new or changed in the update

If you run into any issues after updating, see [Collection / Update Issues](../Troubleshooting/collection-update-issues.md). You can also reach out on the [Discord Server](https://discord.gg/MPcgJUXeeY).

## Related

- [Vortex Notifications and Solutions](../Troubleshooting/vortex-notifications.md)
- [Collection / Update Issues](../Troubleshooting/collection-update-issues.md)
- [Adjusting Configurations](../Customize/adjusting-configurations.md)
- [Install with Vortex](../Install/vortex.md)
