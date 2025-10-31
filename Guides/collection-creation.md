# How to Create A Collection

> 📂 Docs / Guides / How to Create A Collection

*Last updated:* 2025-10-31  
*Applies to Stardew Valley:* **1.6.15+**

A unified technical guide combining the general collection creation workflow and the mechanics of Replicate, Exact, and Binary Patch.

---

# Creating and Managing Collections in Vortex

## 1. What a Collection Is

A *collection* in **Vortex** is a curated list of mods and optional assets that can be installed and managed as a single package.
Collections reference mods hosted on Nexus Mods (or other allowed sources) rather than embedding the actual mod files.
They are designed to make modded setups reproducible, consistent, and shareable across users and systems.

---

## 2. Best Practices for Curators

Before creating your collection, keep these principles in mind:

* Begin with a **clean, stable base profile** to minimize conflicts.
* Verify **mod compatibility and load order** before export.
* Follow Nexus' terms for public distribution — collections reference mods, they do not own them.
* When using mods from external sources, prioritize mods with stable, long-term availability — avoid linking to mods that may be removed or become unavailable.
* Curators are responsible for supporting users of their collection, not individual mod authors.

---

## 3. Creating a Collection

### Option A — Convert an Existing Profile

1. Launch **Vortex** and load the game profile you want to package.
2. Resolve conflicts and confirm stability.
3. Open the **Collections** menu.
4. In the **Workshop** tab, select **Create a Collection → From Profile**.
5. Vortex will generate a collection based on your profile. Rename and edit as needed.
6. Open the **Edit** interface to fine-tune mod inclusion, metadata, and structure.

### Option B — Start from Scratch

1. Navigate to **Collections → Workshop**.
2. Click **Create a Collection → Empty**.
3. Name your new collection.
4. Add mods manually, set metadata, and configure load order and dependencies.

---

## 4. Required Metadata and Considerations

When finalizing a collection:

* Provide a descriptive title and summary.
* Document its scope and purpose (e.g., "Hardcore Survival Build for Stardew Valley").
* Add all relevant mods and dependencies.
* Define load order rules and conflict resolutions.
* Include configuration instructions (INI tweaks, external tools, etc.).
* Review mod-by-mod installation, version, and source tags are properly attributed.
* Ensure you follow [Nexus Mods guidelines](https://help.nexusmods.com/article/115-guidelines-for-collections).

---

## 5. Collection Visibility

When publishing a collection to Nexus Mods, you control whether it is **listed** or **unlisted**.

* **Listed collections** are publicly visible on Nexus Mods.
  They appear in search results, can be endorsed, followed, and discovered by any user.
  This option is suited for stable, public releases intended for general use.

* **Unlisted collections** are private or semi-private.
  They do not appear in search results or public listings, but anyone with the direct link can install them through Vortex.
  This setting is ideal for:

  * Testing or work-in-progress builds
  * Group or server setups shared only with trusted users
  * Temporary or experimental configurations

> **Important:** Listed or unlisted, a collection's link remains active indefinitely once published.
> Nexus Mods currently does not support deleting or archiving collections.
> If you need to retire a collection, you can unlist it and optionally mark it as deprecated in the title or description, but the URL will continue to function for anyone who already has it.

When deciding which visibility setting to use, consider whether your collection is stable, documented, and ready for a general audience.
Curators often keep early builds **unlisted** during development or testing, then switch to **listed** once the collection is complete and verified for public release.

---

## 6. Installation and Version Control in Collections

When curating a collection, you define not just *which mods* are included but *how each mod is installed* and *which version is pulled*.
Vortex exposes these as two separate but related controls:

* **Version Policy** → determines *which version* of the mod is used.
* **Install Option** → determines *how the mod's archive is installed and deployed* on the user's machine.

---

## 6.1 Version Policy (which mod version to use)

Each mod in your collection has a version policy that governs how Vortex resolves the download:

**Prefer Exact (default)**
- **Behavior:** Uses the same version as the curator if it's still available; otherwise, the newest version.
- **Typical Use Case:** Safe default; maintains compatibility while allowing updates.

**Exact Only**
- **Behavior:** Enforces the curator's specific file version by its Nexus Mods ID. Required if file layout or checksums are referenced (e.g., with *Replicate*).
- **Typical Use Case:** Ensures all users get byte-identical files.

**Latest**
- **Behavior:** Always uses the newest available version on Nexus Mods, ignoring curator's version metadata.
- **Typical Use Case:** Useful for ongoing, rolling collections or when mods are frequently updated.

> **Note:** If a file used by the curator is removed from Nexus Mods, *Exact Only* installs will fail until the curator updates the collection or provides an alternate source.

---

## 6.2 Install Option (how the mod is applied)

Install options tell Vortex how to reproduce your installation behavior for each mod:

**Fresh Install**
- **Behavior:** Performs a clean install as if the user manually installed the mod; presents any mod installer (e.g., FOMOD) UI.
- **Requirements:** None
- **When to Use:** For users who should choose their own installer options.

**Same Install Options**
- **Behavior:** Reuses the curator's saved installer choices (skipping prompts).
- **Requirements:** Works only with curated FOMOD settings.
- **When to Use:** For standardized setups where user input should be avoided.

**Replicate**
- **Behavior:** Exports a manifest of file hashes and folder paths from the curator's deployed mod. When installed, Vortex matches files by checksum and reproduces the exact folder structure and file placement the curator used.
- **Requirements:** Requires **Exact Only** version policy; incompatible with *Latest*.
- **When to Use:** For reorganized or cleaned-up mod layouts that need structural fidelity.

---

## 6.3 Using "Open in File Manager" and "Unpack As-Is"

### Open in File Manager

Curators can right-click any mod in Vortex and choose **Open in File Manager**.
This opens the deployed (staging) folder, letting you:

* Inspect the unpacked file structure.
* Manually move, rename, or delete files.
* Verify texture or script locations before building your collection.

When you later export your collection with **Replicate**, Vortex records these layout changes by hashing each file's content and path.
During installation, Vortex matches those hashes in the user's downloaded mod archive and reproduces your reorganized structure automatically.

### Unpack As-Is

If a mod archive contains nested folders or an unusual structure, you can install it with **Unpack As-Is** (right-click the mod → *Install As-Is*).
This bypasses Vortex's automatic directory detection and extracts the archive exactly as stored.
Curators often use this to:

* Correct mods with inconsistent packaging (extra folder levels, embedded archives).
* Merge manually prepared assets into the staging area for later replication.

When combined with **Open in File Manager**, this approach gives you full control over how a mod's files are laid out before capturing that configuration in a **Replicate** install manifest.

---

## 6.4 Binary Patching (and why not to mix it)

**Binary Patch** allows the curator to distribute lightweight, byte-level modifications (for example, fixing a texture or INI).
However, binary patches alter file content and thus change checksums.
Since *Replicate* and *Exact Only* depend on stable hashes, they become invalid once a patch is applied.

Use only one of the following per file:

- **Adjust file contents (minor fix)** → Use **Binary Patch**
- **Preserve curator's file layout** → Use **Replicate + Exact Only**
- **Keep version flexibility** → Use **Prefer Exact** or **Latest**

---

### Summary

**Version Policies:**
- **Exact Only** (Versioning) - Locks file version via Nexus Mods ID and checksum. Use for controlled environments and reproducibility.
- **Prefer Exact** (Versioning) - Tries curator's version, falls back to latest. Use for balanced flexibility.
- **Latest** (Versioning) - Always newest file. Use for actively maintained collections.

**Install Options:**
- **Replicate** (Deployment) - Recreates curator's folder structure by hash. Use for structural edits and repackaged mods.
- **Same Options** (Deployment) - Reuses curator's installer choices. Use for FOMOD automation.
- **Fresh** (Deployment) - Prompts user during install. Use for customizable setups.

**Tools:**
- **Open in File Manager** - View/edit deployed file structure. Use for manual curation.
- **Unpack As-Is** - Extract archive exactly as stored. Use to fix mispackaged mods.


---

### Further Reading
* https://help.nexusmods.com/article/115-guidelines-for-collections
* https://modding.wiki/en/nexusmods/collections/how-to-install
* https://modding.wiki/en/nexusmods/collections/create

