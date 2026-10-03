<div align="center">

<img src="assets/asfra.png" width="72" alt="Asfra"/>

# Asfra

**Advanced Minecraft Automation Tool**

![version](https://img.shields.io/badge/version-3.7.0-6855ab?style=flat-square)
![platform](https://img.shields.io/badge/platform-Windows%2010%2F11-4a4a6a?style=flat-square)
![license](https://img.shields.io/badge/license-Proprietary-3a3a5a?style=flat-square)

[Download](#download) • [Features](#features) • [Screenshots](#screenshots) • [Security](#security)

</div>

---

<div align="center">
<img src="assets/clicker_stormy.png" width="700" alt="Asfra - Clicker panel"/>
</div>

---

## Overview

Asfra is a high-performance desktop automation tool built for Minecraft PvP. The core logic runs entirely in native **C++**, wrapped in a clean **PyQt5** interface — delivering precise click timing and movement macros with near-zero CPU overhead.

- Native C++ implementation for optimal performance and timing accuracy
- Independent Left / Right clicker with their own CPS, key and options
- Focus detection — automatically pauses when Minecraft loses focus
- **Inventory Check** — cursor-center detection, auto-pauses on GUI/ESC/inventory
- **Rod & Gapple macros**, **Blockhit**, **Only Weapons**
- **Module keys** — every module can be switched on and off with its own key
- **HUD overlay** — module list, CPS counter and on/off alerts on top of the game, in three styles
- **Stats** — live CPS chart and all-time click statistics, backed up so they are never lost
- **CraftRise page** — look up any player's rank, experience and modes; save yourself, follow today's gains and keep a day-by-day log
- **Player card on the HUD** — your rank, TP and the mode you play, right in the game
- **Shortcuts (F1)** — every key in one list, clashes marked
- Profile system — save, load and share named configurations
- Silent updates with release notes inside the app, and an opt-in beta channel
- Raw Input based button tracking — zero latency added to mouse movement
- English and Turkish UI, six themes, keyboard navigation, Windows display scaling
- Single portable EXE — no installation, no dependencies

---

## What's New — v3.7.0

- **CraftRise has its own page** — next to Stats in the top bar, with two tabs: Player and Daily. Stats now shows only your clicks (CPS)
- **My player** — the CraftRise star became a panel: see your saved player, swap or remove them, and put them on the HUD
- **Today** — your saved player's points, TP and wins count from 00:00 (Istanbul time), stay when you reopen Asfra and reset at midnight; gains made while Asfra was closed the same day are added when it opens
- **Daily** — every day since you saved the player (up to 30): points, TP, wins, rank changes and each mode's gains (K/D in The Pit). The previous saved player's days stay below a divider
- **Last 7 days** — a small bar chart in My player, with a link to the Daily tab
- **Player card on the HUD** — rank, TP, progress to the next rank, the mode you play and this session's points, right in the game
- **New HUD editor** — the editor is now the game screen: parts on a shelf, a small toolbar on the selected part and its settings beside it; arrow keys nudge, Enter opens settings
- **SonOyuncu in Only in Focus** — the clicker recognises the SonOyuncu client (and other launchers with their own Java), and browser tabs with "Minecraft" in the title no longer count as the game
- **Updates stay in place** — Asfra updates its own file: the desktop icon keeps its place and no extra files are left behind
- Smoother Stats tabs, no HUD hiccup when a module is switched, and Ctrl+4 opens CraftRise, Ctrl+5 opens Stats

## What's New — v3.6.0

- **CraftRise page** — a second page under Stats: look up any CraftRise player and see their rank, experience and what they gain from then on
- **Rank road** — the nearby ranks on one road coloured like the tiers, filled as far as the experience goes, with a gently pulsing ring on the current rank
- **Points per minute** — a chart of the points each minute of play brought, split by mode (SkyWars, BedWars, The Bridge…), each mode's best minute marked; hover a dot for its points, mode and time
- **Right now** — the mode being played, the points and wins it brought this session, K/D in The Pit, and the other modes that scored
- **Save yourself** — the saved player is followed from the moment Asfra opens, even while you look someone else up; one click brings them back
- **Gentle on the site** — reads every 20 s while the player scores and every 2 min while they don't, and waits longer when CraftRise is slow or down
- **Silent updates** — a new version downloads in the background while you play; a small "ready" chip offers a restart, otherwise it switches the next time Asfra opens
- **Beta channel** — turn on "Get beta versions" in Settings to try new versions early (settings are backed up first); beta builds carry a BETA badge and send reports straight to the team
- **One Asfra at a time** — opening it again (or another copy) brings the running one to the front instead of starting a second
- Shortcuts and What's New are now icon-only buttons in the top bar

## What's New — v3.5.6

- **Smoother What's New panel** — opening, scrolling and expanding releases no longer stutter
- **Release notes fit the panel** — long lines wrap instead of being cut off at the right edge
- **Cleaner disk** — temporary files left behind when Asfra was force-closed are removed on the next start
- **Stats are backed up** — kept in a second file, so they survive even a broken config.json
- Fixed: an error window when closing Asfra, Discord status now clears right away when turned off

## What's New — v3.5.5

- **What's New** — release notes right inside the app, with a dot when there is something you haven't read; the update screen shows what's in the new version
- **Stats** — live CPS chart, this session and all-time clicks, peak and average CPS
- **Shortcuts (F1)** — every key in one list; bind or change keys right there, clashes are marked
- **Module keys** — Auto Sprint, No Slow, Anti AFK, PvP Bat and Performance Mode each get an on/off key
- **Performance Mode** — gives the game Windows' High process priority while it runs
- **HUD** — follows the app language, title on top, three styles (Classic, Card, Minimal), background opacity, sort order, clock / session time / profile lines, and on/off alerts you can place anywhere; the HUD editor was redesigned
- **Safer one-click updates** — works in folders with Turkish letters, checks the download's SHA-256, cleans up after itself and tells you when it's done
- **Easier to use** — keyboard navigation (Tab, Space, Enter), clearer key fields, a warning right under a key that is already taken, hover explanations for every option
- **Windows display scaling** (125 % / 150 %) and a **Report a problem** button with an error log
- **Profiles keep everything** — module keys, PvP Bat, Performance Mode and the HUD look; older profiles load cleanly
- Fixed: ESP now says when the game isn't found, numbers no longer shift the sliders, several crashes

## What's New — v3.5.0

- **New look** — three pages (Clicker, Modules, Settings), a sliding "street lamp" tab indicator, rounded content panel and smooth animations everywhere
- **Redesigned themes** — Stormy, Eclipse, Lush, Ink and Fireworks rebuilt from scratch, plus a hidden theme to discover
- **Single CPS slider** — pick one CPS; clicks vary naturally around it (continuous timing, properly seeded randomness)
- **Per-side options** — Left and Right click each keep their own Inventory Check; Break Blocks, Blockhit and Only Weapons belong to the left click
- **Blockhit** — short sword block after a hit with an adjustable chance
- **Only Weapons** — clicks only while your weapon slot is selected, re-synced from the on-screen hotbar
- **Gapple Macro** — next to the Rod Macro, same timing
- **HUD editor** — drag the module list and CPS counter, pick which rows show; HUD colours flow through the theme when RGB is off
- **Profiles** — carry their theme, animate when loaded, and can be shared as a one-line code
- **Close to tray**, key-conflict warnings, double-click to type slider values
- **One-click updates** — "Update now" downloads, installs and restarts; "Later" keeps you playing
- **Half the size** — the exe went from ~40 MB to ~20 MB
- Fixed: settings not loading at startup, stray pop-up windows, black tooltip boxes, a crash with the HUD enabled at launch, the ESP "already injected" check

## What's New — v3.4.0

- **Rod Macro** — switches to the rod slot, right-clicks, waits the set delay and switches back to the sword
- **Smooth page transitions** — pages fade when you switch between them
- **Keybind fix** — leaving both clicker sides unbound no longer counts as a key conflict
- Added Turkish & English language support
- Theme preference is now saved across sessions
- Added Discord and Website shortcuts to the side menu
- Added Windows 7 & 8.1 support
- Fixed ESP-related issues
- Fixed side menu logo bug
- Fixed application crash issues
- Minor fixes and improvements

---

## Features

### 🖱️ Clicker

| Feature | Status |
|---|---|
| Left & Right Clicker — independent profiles | ✅ |
| One-slider CPS (clicks within ±1 of the chosen value) | ✅ |
| Toggle Mode / Hold Mode | ✅ |
| Custom hotkey binding (A–Z, F1–F12, Mouse 2/4/5 and more) | ✅ |
| Inventory Check — auto-pause on GUI/ESC/inventory (per side) | ✅ |
| Break Blocks — WASD-gated, only clicks while moving (per side) | ✅ |
| Rod Macro — switch to rod, right-click, wait, switch back | ✅ |
| Gapple Macro — switch to gapple, right-click, wait, switch back (same timing as the Rod Macro) | ✅ |
| Blockhit — short sword block after a hit, with an adjustable chance (left click) | ✅ |
| Only Weapons — clicks only while your weapon's hotbar slot is selected (follows 1-9 keys and the wheel, re-synced from the on-screen hotbar) | ✅ |

### 🏃 Movement

| Feature | Status |
|---|---|
| Auto Sprint (with its own on/off key) | ✅ |
| No Slow (with its own on/off key) | ✅ |
| Safe Walk | 🔜 Coming soon |
| Strafe | 🔜 Coming soon |

### 🔧 Misc

| Feature | Status |
|---|---|
| ESP (Player Wallhack) — DLL inject | ✅ |
| Anti AFK — auto-jump every 13s | ✅ |
| PvP Bat — network & power tweaks for lower ping | ✅ |
| Performance Mode — High process priority for the game while it runs | ✅ |
| On/off key for every module above except ESP | ✅ |

### ⚙️ Settings

| Feature | Status |
|---|---|
| Only in Focus | ✅ |
| HUD Overlay (RGB or theme-flow colours, scalable) | ✅ |
| HUD styles — Classic, Card, Minimal; background opacity; sort order | ✅ |
| HUD editor — drag the module list, CPS box and on/off alerts; pick rows; clock / session / profile lines | ✅ |
| Discord RPC | ✅ |
| Language — English / Turkish | ✅ |
| Themes — Stormy, Eclipse, Lush, Ink, Fireworks (and a hidden one) | ✅ |
| Close to system tray (quit from the tray icon) | ✅ |
| Stats page — live CPS chart, session and all-time statistics | ✅ |
| CraftRise page — any player's rank road, points per minute by mode, wins and K/D since the search | ✅ |
| Save a player — followed whenever Asfra is open, alongside other searches | ✅ |
| Shortcuts (F1) — every key in one list, bind keys in place | ✅ |
| What's New — release notes inside the app | ✅ |
| Silent updates — download in the background, switch on restart (SHA-256 verified) | ✅ |
| Beta channel — opt in to early versions, settings backed up, reports sent from the app | ✅ |
| One Asfra at a time — a second launch brings the running one forward | ✅ |
| Report a problem — copies version and recent errors | ✅ |
| Stream Proof | 🔜 Coming soon |

### 💾 Profiles

| Feature | Status |
|---|---|
| Save / Load configurations | ✅ |
| Multiple named profiles | ✅ |
| Per-profile clicker, modules, module keys, HUD look, settings & theme | ✅ |
| Share a profile as a one-line code, import a friend's code | ✅ |

---

## Screenshots

<div align="center">

<img src="assets/clicker_stormy.png" width="680" alt="Clicker panel"/>

*Clicker — independent Left / Right profiles with their own CPS, options and hotkey, plus Rod and Gapple macros*

<br/><br/>

<img src="assets/modules_stormy.png" width="680" alt="Modules — Movement and Misc"/>

*Modules — Auto Sprint, No Slow, Anti AFK, PvP Bat and Performance Mode, each with its own on/off key · ESP & Chams*

<br/><br/>

<img src="assets/profiles_stormy.png" width="680" alt="Manage profiles"/>

*Profiles — save and load named configurations instantly*

<br/><br/>

<img src="assets/settings_stormy.png" width="680" alt="Settings panel"/>

*Settings — client options, HUD, language, theme and version info*

<br/><br/>

<img src="assets/account_stormy.png" width="680" alt="Stats"/>

*Stats — live CPS chart, this session and all-time clicks*

<br/><br/>

<img src="assets/craftrise_stormy.png" width="680" alt="Stats — CraftRise"/>

*Stats › CraftRise — rank road, points per minute by mode and the mode being played (a demo player)*
</div>

---

## Download

Download the latest release from the [**Releases**](../../releases/latest) page or visit **[asfra.xyz](https://asfra.xyz)**.

Run `Asfra.exe` — no installer, no dependencies, no setup.

### System Requirements

| | |
|---|---|
| OS | Windows 10 / 11 (64-bit) |
| Disk space | ~22 MB |
| Dependencies | None |

---

## Security

Asfra may be flagged by Windows Defender or antivirus engines due to autoclicker behavior patterns. **These are false positives.**

<details>
<summary><b>Why does antivirus flag it?</b></summary>

<br/>

| Detection | Reason |
|---|---|
| Mouse / keyboard simulation | Uses `SendInput` Win32 API — standard autoclicker functionality |
| Hotkey detection | Uses `GetAsyncKeyState` for configured hotkeys — does **not** log keystrokes |
| DLL injection (ESP) | Uses `CreateRemoteThread` for ESP module — standard technique |
| Unsigned binary | Code signing certificates cost $200–400/year; absence does not indicate malware |

**Actual behavior:**
- 🌐 Connects to GitHub to check for updates and show release notes, and to craftrise.com.tr only when you look up or save a player, to read that player's public profile (Discord RPC talks to the Discord app on your PC)
- ❌ No registry changes, except PvP Bat while it is on: it sets Windows' network throttling off (and puts it back to the Windows default when turned off), and switches the power plan and TCP tuning, which it also restores. Most of these need Asfra to run as administrator
- ❌ No process injection outside of opt-in ESP feature
- ❌ Does not auto-start with Windows
- ✅ Settings and stats live in `%APPDATA%\AsfraClient`; the log and update files in `%LOCALAPPDATA%\AsfraClient`
- ✅ An update replaces `Asfra.exe` in its own folder, after checking the download's SHA-256

</details>

To bypass SmartScreen: click **"More info" → "Run anyway"**, or add an exclusion in Windows Security settings.

---

## Compatibility

| Environment | Status |
|---|---|
| Craftrise | ✅ Full compatibility |
| Sonoyuncu | ✅ Full compatibility |
| Vanilla / Fabric | ✅ Full compatibility |
| Lunar Client / Badlion | ✅ Full compatibility |
| Hypixel | ⚠️ Use with caution |

---

## License

Proprietary software. All rights reserved.  
Unauthorized distribution, modification, or reverse engineering is prohibited.

---

<div align="center">
<sub>Made by <b>svx</b> &nbsp;·&nbsp; <a href="https://asfra.xyz">asfra.xyz</a></sub>
</div>
