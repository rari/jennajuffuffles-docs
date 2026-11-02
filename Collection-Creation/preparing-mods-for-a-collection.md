# Preparing Mods for a Collection
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

## Mods Must Have a Source

Some mods show an error in Vortex while you build a collection. Mods added to Vortex manually or from uncompressed folders may not have enough source information for Vortex to upload them as part of a collection.

A collection needs to know where to download each mod. To keep a mod eligible for the collection do any of these things:

- Download mods with the mod manager button, when that button is available, while browsing Nexus Mods.
- Add ZIP files directly after downloading with the manual download button on Nexus Mods.
- Supply accurate source information for user-generated resources from sources outside Nexus.
- Avoid adding uncompressed or repackaged folders from Nexus. That is fine for solo play but they lack the hash data Vortex needs to tie the mod back to its original source so others can download it.

If a mod shows an error, remove it from your profile, download it through Vortex or as a ZIP from Nexus Mods, and reinstall it before you include it in the collection.

## Versions

Each mod has a version policy. The policy controls how Vortex resolves the download.

| Policy | Behavior | Typical use |
| --- | --- | --- |
| Exact Only (default) | Enforces the curator's specific file version by its Nexus Mods ID. Locks to that version. Required if file layout or checksums are referenced, for example with Replicate. | Ensures all users get byte-identical files. Most stable, and may become outdated. Required for Replicate installs. This is the policy used for all of JennaJuffuffles' collections. |
| Prefer Exact | Uses the same version as the curator if it is still available; otherwise, the newest version. | Safe default. Maintains compatibility while allowing updates. Balanced approach; recommended default. |
| Latest | Always uses the newest available version on Nexus Mods, ignoring the curator's version metadata. | Useful for ongoing, rolling collections, or when mods are frequently updated. Good for actively maintained collections, but may introduce breaking changes. |

{% hint style="info" %}
If a file used by the curator is removed from Nexus Mods, Exact Only installs fail until the curator updates the collection or provides an alternate source.
{% endhint %}

Replicate requires Exact Only. [Publishing and Revisions](publishing-and-revisions.md) explains Install as New, Replicate, and Same Install Options.

## Mod Structure (Unpack As-Is)

If a mod archive contains nested folders or an unusual structure, install it with **Unpack As-Is** (right-click the mod, then **Install As-Is**).

Unpack As-Is bypasses Vortex's automatic directory detection and extracts the archive exactly as stored. Some mods are packaged inconsistently or use a custom folder structure. Unpack As-Is preserves that structure. That matters for Replicate, and whenever the folder structure is required for the mod to work.

Curators often use Unpack As-Is to:

- Correct mods with inconsistent packaging, such as extra folder levels or embedded archives.
- Merge manually prepared assets into the staging area for later replication.
- Use Exact Only and Replicate to preserve the complete structure.

## Binary Patch

Binary Patch lets a curator distribute lightweight, byte-level modifications, for example a texture fix or an INI fix. A binary patch alters file content and changes checksums. Replicate and Exact Only depend on stable hashes, so they become invalid once a patch is applied.

A patch can fix a small issue without redistributing the whole mod. Because the checksum changes, hash-based installation no longer matches. Choose one approach per file. Patching the file and preserving the exact folder structure cannot be combined on that file.

Use only one of the following per file:

- **Adjust file contents (minor fix).** Use **Binary Patch + Exact Only**.
- **Preserve the curator's file layout.** Use **Replicate + Exact Only**.
- **Keep version flexibility.** Use **Prefer Exact** or **Latest**.

## Bundling

Bundling lets curators include optional auxiliary support files directly in a collection. It has strict limits. It is not a substitute for uploading mods to Nexus Mods.

Collections are designed to reference mods through Nexus entries, not to bundle those mods. Referencing the Nexus entry is how mod authors receive credit, downloads, and donation points. Bundling is only for auxiliary files that would not have their own mod page.

### When to use bundling

Use bundling only for:

- Tool-generated support files, such as LOD data or optimization files.
- Auxiliary files that are impractical to host per mod.
- Generated components or patches that would not have their own mod page.

### When not to use bundling

{% hint style="warning" %}
A collection cannot include full mod files as bundled content. Collections must reference mods through their Nexus entries so mod authors receive credit, downloads, and donation points. See [Nexus Mods Guidelines for Collections](https://help.nexusmods.com/article/115-guidelines-for-collections) for the policy.
{% endhint %}

Do not use bundling for:

- Full mods or mod files created by others. That requires explicit permission, and those files should be referenced through Nexus.
- Distributing mods that do not have proper Nexus entries.
- Avoiding an upload of those mods to Nexus Mods.

## Related
- [Creating a Collection](creating-a-collection.md)
- [Publishing and Revisions](publishing-and-revisions.md)
- [Rules and Conflicts](rules-and-conflicts.md)
