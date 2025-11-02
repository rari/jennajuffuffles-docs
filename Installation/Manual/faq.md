# Manual Installation FAQ & Limitations

> 📂 Docs / Installation / Manual / FAQ

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* **1.6.15+**

---

## FAQ

### Why choose manual installation?
> Manual installation is available for users who:
> - Cannot use Vortex (e.g., on macOS or Linux without NMA support)
> - Prefer direct control over their mod files
> - Need to work around mod manager limitations
>
> **Note:** We strongly recommend using Vortex or Nexus Mods App when possible, as they handle configuration files, load order, provide bundled patches, and updates automatically.

### What are the main limitations?
> - **No automatic updates** — You must manually download and update each mod
> - **No automatic configuration** — You must manually apply config files from the configuration package
> - **Load order management** — You must manually manage mod load order (mod folder names affect loading or false requirements in manifest)
> - **Patch management** — You must manually apply required patches when collections update
> - **Error detection** — Harder to identify missing or incorrectly installed mods
> - **Collection updates** — Requires re-downloading and reinstalling mods when the collection updates

### How do I update mods manually?
> 1. Check the collection's last update date on Nexus
> 2. Compare your installed mod versions with the collection's mod list
> 3. Download updated mods from their individual Nexus pages
> 4. Replace old mod folders with new ones in your Mods directory
> 5. Re-apply configuration files and patches if needed
>
> **Important:** Always check the collection changelog first — don't update individual mods beyond the collection's tested versions.

### How do I manage load order?
> Mods load alphabetically by folder name. If you need a specific load order:
> - Rename mod folders (add prefixes like `001_`, `002_`, etc.)
> - Be careful — this can break if mods update and you reinstall them

### What if a mod isn't working?
> 1. Check the SMAPI console for error messages
> 2. Verify the mod folder structure matches the mod's requirements
> 3. Ensure all dependencies are installed
> 4. Check that configuration files were merged correctly
> 5. Verify you're using the correct mod version (matching the collection's last update date)
> 6. Check the mod's individual Nexus page for known issues

### Configuration files keep getting overwritten — how do I preserve custom settings?
> Create backups of your custom configuration files. When updates occur:
> 1. Back up your custom config files before updating
> 2. Download and apply the new configuration package
> 3. Manually merge your custom settings back into the updated configs
>
> Alternatively, use in-game configuration via GMCM, which persists through mod updates.

### I see update notifications in SMAPI — should I update?
> Not necessarily. Only update mods when the collection itself updates. Individual mod updates may break compatibility with other mods in the collection. Check the collection's last update date before updating anything.

### Can I mix manual installation with a mod manager?
> No. Do not run a mod manager and manually install mods to the same game installation — this will cause conflicts and potential corruption.

---

## Common Issues

### Missing mods in SMAPI console
> - Verify all mods were downloaded and placed correctly
> - Check folder structure — some mods require specific subfolder layouts
> - Ensure mod folders are directly in the Mods directory, not nested incorrectly

### Configuration not applying
> - Verify you extracted and merged config files correctly
> - On Mac, use Option + drag to merge folders properly
> - Check that config files are in the correct mod folders
> - Some configs may need to be placed in subfolders (e.g., `config/`, `assets/`)

### Incorrect folder structure
> Some mods require specific folder layouts. If SMAPI reports structure issues:
> - Check the mod's Nexus page for installation instructions
> - Ensure you extracted the mod correctly (not double-nested folders)
> - Verify all required files are present in the mod folder

### SMAPI update notifications are annoying
> Edit the mod's `manifest.json` file and update the `"Version"` field to match the version shown on Nexus. This suppresses update notifications without actually updating the mod.
