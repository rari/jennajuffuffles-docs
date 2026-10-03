# Rules and Conflicts
*Applies to: Stardew Valley 1.6.15+ Last reviewed: 2026-10-02*

**Manage Rules** controls the load order of the mods in a collection: which mods load before others. Load order matters when mods modify the same files.

When several mods change the same file, load order decides which mod's version of that file is used. An incorrect load order can stop a mod from working, make it display incorrectly, or leave mods in conflict. Configuration mods must load after the mods they configure, or their changes will not apply.

Rules tell Vortex:

- Load Mod A before Mod B.
- Load Mod B after Mod A.
- Mod A and Mod B conflict. Choose one.

Configuration mods and content patch mods should load after the mods they modify.

## Setting a rule

You can set a rule without an existing conflict. Turn on the Dependencies column. Drag one mod's dependency icon onto the matching icon on the other mod.

The pop-up offers:

- Must deploy before
- Must deploy after
- Requires (Local only, will not save to collection)
- Conflicts with / Can't be deployed together with

{% embed url="https://youtu.be/iovV-GJYkKA" %}

## Related
- [Mark Mods Required or Optional](mark-mods-required-or-optional.md)
- [Preparing Mods for a Collection](preparing-mods-for-a-collection.md)
