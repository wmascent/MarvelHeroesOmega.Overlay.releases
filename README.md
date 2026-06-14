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

## First launch

1. Set your **game folder** (the Marvel Heroes install that contains `UnrealEngine3\`).
2. Set your **Bifrost config folder** (where `Bifrost.LaunchConfig.json` and `Bifrost.ServerList.json` live).
3. Choose your **server** from the list.
4. Click **Play**.

The launcher starts the game and turns on the overlay. After you are in-world, look for the **OVERLAY** tab on the **left edge** of the game window.

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
| Inject / access denied | Run **MhLauncher** as **Administrator**. |
| Loot toggles do nothing | Make sure the **`LootFilter`** folder is next to `MhLauncher.exe` (comes in the zip). |

---

## About this repo

This repository holds **release downloads only** (zip + checksum). It is not the source code project — just the place to grab builds and where the launcher looks for updates.
