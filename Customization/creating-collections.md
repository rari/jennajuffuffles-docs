---
title: Creating Your Own Mod Collections
description: Create your own Stardew Valley mod collections with Vortex. Learn about version policies, load order, binary patches, bundling, and publishing collections to Nexus.
keywords: [creating collections, collection creation, Vortex collections, mod collections, version policies, Exact Only, Replicate, Binary Patch, bundling, load order, private collections, public collections]
tags: [collection-creation, vortex, collections, modding]
---

# How to Make a Collection

*Last updated:* 2026-01-19  
*Applies to Stardew Valley:* 1.6.15+

This guide will help you create your own mod collections for Stardew Valley! Whether you want to build a collection from scratch, share your custom setup with friends, or create a companion collection to use alongside Stardew Valley Expanded or the Aesthetic Valley collections, this guide covers everything you need to know.

{% hint style="danger" %}
This guide is for creating your own original collections, not for copying or repackaging existing collections. Collections include curated configurations and sometimes custom patches that belong to the original curator or others.
{% endhint %}

---

## Table of Contents

- [Creating a Collection](#creating-a-collection)
- [Sharing Your Collection](#sharing-your-collection)
- [Mods Must Have a Source](#mods-must-have-a-source)
- [Versions (Why They Matter)](#versions-why-they-matter)
- [Install as New vs Replicate](#install-as-new-vs-replicate)
- [Mod Structure (Unpack As-Is)](#mod-structure-unpack-as-is)
- [Binary Patch](#binary-patch)
- [Bundling](#bundling)
- [Rules = Load Order](#rules--load-order)
- [Required vs Optional](#required-vs-optional)
- [Private vs Public Collections](#private-vs-public-collections)

---

## Creating a Collection

There are two main methods for creating a collection:

**Method 1: Create from Profile (Recommended)**

This method captures all your additional mods automatically:

1. In Vortex, go to the **Mods** tab
2. Filter for active collection name(s) on your current profile
3. Disable the collection (click to include recommended mods when prompted)
4. Go to **Collections > Create a Collection > From Profile**
5. This creates a DRAFT of your collection
6. (Optional) Upload to Nexus' server from the Workshop section

**Method 2: Create Empty Collection**

For creating a collection from scratch:

1. Create an empty collection in Vortex
2. Right-click "Add to Collection" on each mod in the Mods page
3. (Optional) Upload to Nexus' server from the Workshop section

---

## Sharing Your Collection

When creating a collection, you can choose how it's shared:

- **Private link:** Share with friends without making it public
- **Unlisted:** Collection won't appear in search results but can be accessed via link
- **Listed:** Public collection (only if you want it discoverable by the community)

---

## Mods Must Have a Source

When building your collection, you may notice that some mods display an error ⚠️ in Vortex. Mods that have been added to Vortex, particularly those installed manually or from uncompressed folders, may not have sufficient source information in Vortex to upload as part of a collection.

Collections need to know where to download each mod from. Without proper source information, Vortex can't include the mod in your collection, and others won't be able to install it. This is a critical requirement for sharing collections.

**To ensure mods can be included in your collection:**

- **Download mods** using the mod manager button (if available) when browsing Nexus Mods
- **Add ZIP files directly** after downloading with the manual download button on Nexus Mods
- **Supply accurate source information** for user-generated resources or mods downloaded from sources outside Nexus
- **Avoid adding uncompressed or repackaged folders** - while this practice is totally fine for solo play, these lack the hash data necessary for Vortex to link that mod back to its original source for download by others

If a mod shows an error ⚠️, you'll need to remove it from your profile, download it properly through Vortex or as a ZIP from Nexus Mods, and reinstall it before including it in your collection.

---

## Versions (Why They Matter)

Each mod in your collection has a version policy that governs how Vortex resolves the download:

**Exact Only (default)**
- **Behavior:** Enforces the curator's specific file version by its Nexus Mods ID. Locks to specific version. Required if file layout or checksums are referenced (e.g., with *Replicate*).
- **Typical Use Case:** Ensures all users get byte-identical files. Most stable but may become outdated. Required for Replicate installs. This is the policy used for all of Jenna Juffuffles' collections.

**Prefer Exact**
- **Behavior:** Uses the same version as the curator if it's still available; otherwise, the newest version.
- **Typical Use Case:** Safe default; maintains compatibility while allowing updates. Balanced approach; recommended default.

**Latest**
- **Behavior:** Always uses the newest available version on Nexus Mods, ignoring curator's version metadata.
- **Typical Use Case:** Useful for ongoing, rolling collections or when mods are frequently updated. Good for actively maintained collections, but may introduce breaking changes.


{% hint style="info" %}
If a file used by the curator is removed from Nexus Mods, *Exact Only* installs will fail until the curator updates the collection or provides an alternate source.
{% endhint %}

---

## Install as New vs Replicate

These installation methods control how mods are installed and whether users can customize installation options.

**Fresh Install (Install as New):**
- Performs a clean install
- Presents FOMOD installer UI if available
- User chooses installer options

Use this when you want users to customize their installation or when mods have important installation choices.

**Replicate:**
- Reproduces exact folder structure by hash
- Requires Exact Only version policy
- Use for reorganized mod layouts

Replicate ensures users get the exact folder structure you created, which is essential if you've reorganized mod files or merged assets. This is critical for collections that use custom folder structures.

**Same Install Options:**
- Reuses curator's saved installer choices
- Skips prompts
- Works only with curated FOMOD settings

{% hint style="info" %}
Use this when you want users to get your exact configuration without prompts. This ensures consistency across all installations.
{% endhint %}

---

## Mod Structure (Unpack As-Is)

If a mod archive contains nested folders or an unusual structure, you can install it with **Unpack As-Is** (right-click the mod > *Install As-Is*).

This bypasses Vortex's automatic directory detection and extracts the archive exactly as stored. 

Some mods are packaged inconsistently or have custom folder structures. Unpack As-Is preserves the exact structure, which is essential when using Replicate or when the folder structure matters for the mod to work correctly.

Curators often use this to:

* Correct mods with inconsistent packaging (extra folder levels, embedded archives).
* Merge manually prepared assets into the staging area for later replication.
* Use Exact and Replicate policies to preserve the complete structure.

---

## Binary Patch

**Binary Patch** allows the curator to distribute lightweight, byte-level modifications (for example, fixing a texture or INI). However, binary patches alter file content and thus change checksums. Since *Replicate* and *Exact Only* depend on stable hashes, they become invalid once a patch is applied.

Binary patches let you fix small issues in mod files without redistributing entire mods. However, they change file checksums, which breaks hash-based installation methods. You must choose between patching files or preserving exact folder structures—you can't do both.

Use only one of the following per file:
- **Adjust file contents (minor fix)** - Use **Binary Patch + Exact Only**
- **Preserve curator's file layout** - Use **Replicate + Exact Only**
- **Keep version flexibility** - Use **Prefer Exact** or **Latest**

---

## Bundling

**Bundling** allows curators to include optional auxiliary support files directly in a collection. However, bundling has strict limitations and should not be used as a substitute for properly uploading mods to Nexus Mods.

Collections are designed to reference mods via Nexus entries, not bundle them. This ensures mod authors get proper credit, downloads, and donation points. Bundling is only for auxiliary files that wouldn't have their own mod page.

### When to Use Bundling

**Use bundling only for:**
- Tool-generated support files (e.g., LOD data, optimization files)
- Auxiliary files that are impractical to host per-mod
- Generated components or patches that wouldn't have their own mod page

### When NOT to Use Bundling

{% hint style="warning" %}
Collection cannot include full mod files as bundled content. Collections must reference mods via their Nexus entries so mod authors receive proper credit, downloads, and donation points. See [Nexus Mods Collection Guidelines](https://help.nexusmods.com/article/115-guidelines-for-collections) for complete policy details.
{% endhint %}

**Do NOT use bundling for:**
- Full mods or mod files created by others (requires explicit permission and should be referenced via Nexus)
- Distributing mods without proper Nexus entries
- Avoiding the need to upload mods to Nexus Mods 

---

## Rules = Load Order

**Manage Rules** controls the **load order** of your mods—which mods load before others. This is crucial for mods that modify the same files.

Load order determines which mod's version of a file is used when multiple mods modify the same file. Incorrect load order can cause mods to not work, display incorrectly, or conflict with each other. Configuration mods must load after the mods they configure, or their changes won't apply.

Rules tell Vortex:
- "Load Mod A before Mod B"
- "Load Mod B after Mod A"
- "Mod A and Mod B conflict - choose one"

Configuration and content patch mods should load after the mods they modify.

---

## Required vs Optional

Understanding the difference between required and optional mods helps you design collections that are flexible while maintaining core functionality.

**Required Mods:**
- Essential for the collection to work
- Cannot be skipped during installation
- Core framework and dependencies

Required mods are the foundation of your collection. Without them, the collection won't function. These are typically framework mods (like SMAPI, Content Patcher) and mods that other mods depend on.

**Optional Mods:**
- Enhance the experience but not strictly necessary
- Can be skipped during installation
- Visual enhancements, alternative configurations
- **May represent conflicts** where players need to choose between mutually exclusive options (e.g., different farm maps, alternative visual styles, or conflicting gameplay mods)

Optional mods give players choices. They can customize their experience by selecting which optional mods to install. When optional mods represent conflicts, players must choose one option, which prevents incompatible combinations.

---

## Private vs Public Collections

Understanding the difference between private and public collections helps you choose the right approach for sharing your collection.

**Private Collections:**
- Unlisted on Nexus Mods (won't appear in search results)
- Shareable via private link
- Good for personal use, friends-only, or organizing your custom mods
- Help you preserve your additions through collection updates
- Make it easy to reinstall your favorite mods
- Allow you to keep track of what you've added

**Public Collections:**
- Listed on Nexus Mods
- Discoverable in search
- Good for sharing with the community
- Requires following Nexus Mods guidelines

{% hint style="danger" %}
Listed or unlisted, a collection's link remains active indefinitely once published. Nexus Mods currently does not support deleting or archiving collections.
{% endhint %}

---

## See Also

- [New Player Install Instructions](../Installation/index.md) - For installing collections
- [Troubleshooting & FAQ](../Troubleshooting/index.md) - For collection management issues
- [How to Customize Collections](index.md) - For custom configurations
- [Nexus Mods Guidelines for Collections](https://help.nexusmods.com/article/115-guidelines-for-collections)
