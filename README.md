<div align="center">

<img src="src/assets/asfra.png" width="72" alt="Asfra"/>

# Asfra

**Advanced Minecraft Automation Tool**

![version](https://img.shields.io/badge/version-3.5.0-6855ab?style=flat-square)
![platform](https://img.shields.io/badge/platform-Windows%207%2F8.1%2F10%2F11-4a4a6a?style=flat-square)
![license](https://img.shields.io/badge/license-Proprietary-3a3a5a?style=flat-square)

[Download](#download) • [Features](#features) • [Screenshots](#screenshots) • [Security](#security)

</div>

---

<div align="center">
<img src="docs/screenshots/clicker_stormy.png" width="700" alt="Asfra - Clicker panel"/>
</div>

---

## Overview

Asfra is a high-performance desktop automation tool built for Minecraft PvP. The core logic runs entirely in native **C++**, wrapped in a clean **PyQt5** interface — delivering precise click timing and movement macros with near-zero CPU overhead.

- Native C++ implementation for optimal performance and timing accuracy
- Independent Left / Right click profiles with per-profile settings
- Focus detection — automatically pauses when Minecraft loses focus
- **Inventory Check** — cursor-center detection, auto-pauses on GUI/ESC/inventory
- **Break Blocks** — WASD-gated clicking, only fires while the player is moving
- HUD overlay — live RGB module status on top of the game
- Profile system — save and load named configurations instantly
- Raw Input based button tracking — zero latency added to mouse movement
- Multi-language UI — English and Turkish supported
- Theme preference saved across sessions
- Discord & Website shortcuts in the side menu
- Single portable EXE — no installation, no dependencies

---

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

- **Rod Macro** — olta slotuna geçip sağ tık basıyor, ayarlanan ms bekleyip kılıç slotuna dönüyor
- **Smooth page transitions** — sayfa geçişlerinde fade animasyonu eklendi
- **Keybind fix** — Sol/Sağ clicker'da NONE ataması artık çakışma sayılmıyor; ikisi de bağımsız NONE olabiliyor
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
| Toggle Mode / Push Mode | ✅ |
| Custom hotkey binding (A–Z, F1–F12, Mouse2/4/5) | ✅ |
| Inventory Check — auto-pause on GUI/ESC/inventory (per side) | ✅ |
| Break Blocks — WASD-gated, only clicks while moving (per side) | ✅ |
| Rod Macro — switch to rod, right-click, wait, switch back | ✅ |
| Gapple Macro — switch to gapple, hold right-click to eat, switch back | ✅ |
| Blockhit — short sword block after a hit, with an adjustable chance (left click) | ✅ |
| Only Weapons — clicks only while your weapon's hotbar slot is selected (follows 1-9 keys and the wheel, re-synced from the on-screen hotbar) | ✅ |

### 🏃 Movement

| Feature | Status |
|---|---|
| Auto Sprint | ✅ |
| No Slow | ✅ |
| Safe Walk | 🔜 Coming soon |
| Strafe | 🔜 Coming soon |

### 🔧 Misc

| Feature | Status |
|---|---|
| ESP (Player Wallhack) — DLL inject | ✅ |
| Anti AFK — auto-jump every 13s | ✅ |

### ⚙️ Settings

| Feature | Status |
|---|---|
| Only in Focus | ✅ |
| HUD Overlay (RGB or theme-flow colours, scalable) | ✅ |
| HUD layout editor — drag the module list and CPS counter, pick the rows | ✅ |
| Show CPS on HUD | ✅ |
| Discord RPC | ✅ |
| Language — English / Turkish | ✅ |
| Themes — Stormy, Eclipse, Lush, Ink, Fireworks (and a hidden one) | ✅ |
| Close to system tray (quit from the tray icon) | ✅ |
| Stream Proof | 🔜 Coming soon |

### 💾 Profiles

| Feature | Status |
|---|---|
| Save / Load configurations | ✅ |
| Multiple named profiles | ✅ |
| Per-profile clicker, movement, misc, settings & theme | ✅ |
| Share a profile as a one-line code, import a friend's code | ✅ |

---

## Screenshots

<div align="center">

<img src="docs/screenshots/clicker_stormy.png" width="680" alt="Clicker panel"/>

*Clicker — independent Left / Right profiles with their own CPS, options and hotkey, plus Rod and Gapple macros*

<br/><br/>

<img src="docs/screenshots/modules_stormy.png" width="680" alt="Modules — Movement and Misc"/>

*Modules — Auto Sprint, No Slow, Safe Walk · ESP & Chams, Anti AFK, PvP Bat*

<br/><br/>

<img src="docs/screenshots/profiles_stormy.png" width="680" alt="Manage profiles"/>

*Profiles — save and load named configurations instantly*

<br/><br/>

<img src="docs/screenshots/settings_stormy.png" width="680" alt="Settings panel"/>

*Settings — client options, HUD, language, theme and version info*
</div>

---

## Download

Download the latest release from the [**Releases**](../../releases) page or visit **[asfra.xyz](https://asfra.xyz)**.

Run `Asfra.exe` — no installer, no dependencies, no setup.

### System Requirements

| | |
|---|---|
| OS | Windows 7 / 8.1 / 10 / 11 (64-bit) |
| Disk space | ~20 MB |
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
- ❌ No network connections
- ❌ No registry modifications
- ❌ No process injection outside of opt-in ESP feature
- ❌ Does not auto-start with Windows
- ✅ Reads/writes nothing outside `%APPDATA%\AsfraClient`

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
