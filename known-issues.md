# Known Issues

*Last updated:* 2025-08-03*Applies to Stardew Valley:* **1.6.15***SVVE Revision:* **86+**

This page covers **collection‑specific issues** and **common modding problems** for **Stardew Valley VERY Expanded** (SVVE) and its companion collections.

> 📘 Installation or Vortex problems? See [Troubleshooting](/troubleshooting) or [Quick Fixes](/quick-fixes).> ❓ Gameplay or compatibility questions? See the [FAQ](/faq).

---

## 🔁 General Issues

### Very slow load time

Large collections can take **3–5 minutes** (or longer on low‑spec PCs) to start a new save or to load from the title screen.

> 🖐️ **Hands‑up method:** keep your hands off the mouse/keyboard until the screen fades in and music starts. Input during asset loading can crash the game.

### Multiplayer / split‑screen desync

Split‑screen sessions may occasionally lag or lose sync. Relaunching the game or restarting the session usually resolves it.

### SMAPI not launching

- Re‑add **SMAPI** as the primary tool in Vortex Dashboard.
- Follow the [Install Guide](/install) → PC → SMAPI section.

### Stuck on 74 / 75 introductions

Enable the **Debug Mode** mod temporarily and run:

```bash
debug wtc lumajunimo
debug wh
```

Disable Debug Mode after fixing.

---

## 🔧 Missing Configurations

If the collection’s configuration files do **not** apply you may see blocked paths, missing overlays, or color mismatches.

1. In **Vortex** **> Rules Manager** check that configurations load ***after*** the mods they impact.
2. Click **Deploy**.
3. If that does not resolve the configurations, you may need to download and apply them manually from [Nexus](https://www.nexusmods.com/stardewvalley/mods/20870). 

#### Minecart blocks the Mine entrance

- Click on the ⚙️ on the main menu. Toggle `GMCM → Stardew Valley Expanded → Original Mine Entrance`.

---

## 🛠️ Visual & UI Conflicts

### Can't exit house, farm map appears "corrupted"

This happens when your **farm map mod becomes disabled or fails to load**. It may look like your house is surrounded by random tiles or even completely missing.

Maps **cannot be switched mid-playthrough** unless you're using a helper mod like [Easy Farm Switcher](https://www.nexusmods.com/stardewvalley/mods/16873).

**Fix:**

- Exit the game.
- Re-enable your farm map mod in Vortex and click **Deploy**.

---

## 🧪 NPC Bugs

### Duplicated NPCs

This rare but known bug causes some NPCs to appear twice (or more) in the world, often after interacting with them.

**Fix:**

1. Load your save.
2. In the SMAPI console, type:

```bash
debug removenpc [InternalNPCName]
```

3. Save and exit the game.

> 💡 **Note:** The internal NPC name is not always the same as the in-game name.

To find it:

1. Load your save.
2. In the SMAPI console, type:

```bash
patch export "Data/NPCDispositions"
```

3. SMAPI will tell you where the file was saved. Open it to look up the internal name.

---

## 🧼 After Updating

If things break after a collection update:

1. In **Collections** tab, click **Remove** the collection Poster.
2. Do not delete mods when asked.
3. On the SVVE page, click **Add Collection**
4. In Vortex install to a **New Profile**.
5. Click **Deploy**.

See [Install → Clean](/install/clean) for a full wipe.

---

## 💬 Need more help?

Upload your log to **[smapi.io/log](https://smapi.io/log)** and ask in our Discord support channel:

👉 **Join us** → [**https://discord.gg/de2NrHXuty**](https://discord.gg/de2NrHXuty)
