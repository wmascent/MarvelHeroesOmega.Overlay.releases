# Marvel Heroes Omega Overlay

Download page for the **Marvel Heroes Omega Overlay** — a small Windows companion for the live game. It adds an in-game **OVERLAY** tab (loot filter and DPS meter) and a launcher that starts the game and applies the overlay for you.

**Latest release:** [Releases](https://github.com/wmascent/MarvelHeroesOmega.Overlay.releases/releases) — pick the newest **v** tag and download **`MarvelHeroesOmega-Overlay-v…-win-x64.zip`**.

---

## What you need

- **Windows 10 or 11** (64-bit)
- **[.NET 8 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/8.0/runtime)** — choose *Run desktop apps*
- **Marvel Heroes Omega** installed
- Your usual **Bifrost** server config (same files you use with the normal launcher)

---

## Install

1. Open **[Releases](https://github.com/wmascent/MarvelHeroesOmega.Overlay.releases/releases)** and download the latest **`MarvelHeroesOmega-Overlay-v…-win-x64.zip`**.
2. **Right-click the zip ? Properties ? Unblock**, then OK. (Windows often blocks downloaded files; this avoids launch/inject issues.)
3. **Extract** the zip anywhere you like (for example `C:\MhOverlay\`).
4. Open the extracted folder and run **`MhLauncher.exe`**.

---

## First launch (Play)

1. Set your **game folder** (the Marvel Heroes install that contains `UnrealEngine3\`).
2. Set your **Bifrost config folder** (where `Bifrost.LaunchConfig.json` and `Bifrost.ServerList.json` live).
3. Choose your **server** from the list.
4. Click **Play**.

The launcher starts the game and turns on the overlay. After you are in-world, look for the **OVERLAY** tab on the **left edge** of the game window.

---

## Play vs Inject

**MhLauncher** has two buttons at the bottom right:

| Button | When to use |
|--------|-------------|
| **Play** | Normal path. Starts Marvel Heroes with your chosen server and turns on the overlay. |
| **Inject** | The game is **already running** and you did **not** start it from this launcher (Steam, another Bifrost shortcut, etc.). Adds the overlay to the game that is open now. |

### When to click Inject

Use **Inject** if you:

- Launched Marvel Heroes from **Steam** (or any launcher other than **MhLauncher**).
- Already had the game open and only then opened **MhLauncher**.
- Clicked **Play** but the log said the game was already running — use **Inject** instead of closing and re-launching.

### How to use Inject

1. Start Marvel Heroes your usual way.
2. Wait until you are at the **main menu** or **in-game** (not on the loading screen).
3. Open **MhLauncher** and confirm your game folder and Bifrost settings are set.
4. Click **Inject**.
5. Read the **Log** panel at the bottom. On success, alt-tab to the game — the **OVERLAY** tab should appear on the left edge.

**Good to know:**

- After a successful **Play**, the overlay is already on — you do **not** need **Inject**.
- **Inject** does **not** start the game; the client must already be running.
- If the log says the hook is **already loaded**, restart the game, then use **Play** or **Inject** again (common after updating the overlay).
- If inject fails with access denied, run **MhLauncher** as **Administrator**.
- Hover the **Inject** button in the launcher for a quick reminder.

---

## In-game

- **OVERLAY tab** — click to open the panel.
- **Loot filter** — hide drops you do not want (categories, rarities, crafting elements, and more).
- **DPS meter** — see damage during fights (boss mode, top contributors, power breakdown on hover).

The tab hides when the game is not in the foreground and comes back when you return to the game.

---

## Updates

**MhLauncher** checks for updates when it starts and when you click **Check for updates**. If a newer version is available, choose **Update now** (close the game first).

You can also download a fresh zip from **[Releases](https://github.com/wmascent/MarvelHeroesOmega.Overlay.releases/releases)** and extract over your existing folder.

---

## Quick fixes

| Problem | Try this |
|--------|-----------|
| Launcher will not start | Install **.NET 8 Desktop Runtime**. |
| No OVERLAY tab after Play | Alt-tab to the game and click in the world; if still missing, restart and launch again. |
| No OVERLAY tab after Inject | Launch the game first, reach the menu or in-game, then click **Inject**; try **MhLauncher** as **Administrator**. |
| "No Marvel Heroes process is running" | Start the game (Steam / Bifrost / etc.), then click **Inject**. |
| "Hook is already loaded" | Restart the game, then **Play** or **Inject** again. |
| "Game is already running" when clicking Play | Close the game and click **Play**, or leave it open and click **Inject**. |
| Inject / access denied | Run **MhLauncher** as **Administrator**. |
| Loot toggles do nothing | Make sure the **`LootFilter`** folder is next to `MhLauncher.exe` (comes in the zip). |

---

## About this repo

This repository holds **release downloads only** (zip + checksum). It is not the source code project — just the place to grab builds and where the launcher looks for updates.
