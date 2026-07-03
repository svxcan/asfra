<div align="center">

<img src="src/assets/asfra.png" width="72" alt="Asfra"/>

# Asfra

**Advanced Minecraft Automation Tool**

![version](https://img.shields.io/badge/version-2.0.0-6855ab?style=flat-square)
![platform](https://img.shields.io/badge/platform-Windows%2010%2F11-4a4a6a?style=flat-square)
![license](https://img.shields.io/badge/license-Proprietary-3a3a5a?style=flat-square)

[Download](#download) • [Features](#features) • [Screenshots](#screenshots) • [Security](#security)

</div>

---

<div align="center">
<img src="src/assets/clicker_pagenew.png" width="700" alt="Asfra - Clicker Page"/>
</div>

---

## Overview

Asfra is a high-performance desktop automation tool built for Minecraft PvP. The core logic runs entirely in native **C++**, wrapped in a clean **PyQt5** interface — delivering precise click timing and movement macros with near-zero CPU overhead.

- Native C++ implementation for optimal performance and timing accuracy
- Independent Left / Right click profiles with per-profile settings
- Focus detection — automatically pauses when Minecraft loses focus
- HUD overlay — live module status on top of the game
- Single portable EXE — no installation, no dependencies

---

## Features

### 🖱️ Clicker

| Feature | Status |
|---|---|
| Left & Right Clicker — independent profiles | ✅ |
| Configurable CPS range (min / max) | ✅ |
| CPS Randomizer — natural timing variance | ✅ |
| Mouse Shake — micro-movement per click | ✅ |
| Toggle Mode / Push Mode | ✅ |
| Custom hotkey binding (A–Z, F1–F12, Mouse2/4/5) | ✅ |
| Block-Hit automation | 🔜 Coming soon |
| Jitter Click | 🔜 Coming soon |
| Butterfly Click pattern | 🔜 Coming soon |

### 🏃 Movement

| Feature | Status |
|---|---|
| Auto Sprint | ✅ |
| No Slow | ✅ |
| Safe Walk | 🔜 Coming soon |
| Inventory Walk | 🔜 Coming soon |
| Strafe | 🔜 Coming soon |
| Scaffold | 🔜 Coming soon |

### 🔧 Misc

| Feature | Status |
|---|---|
| ESP (Player Wallhack) — DLL inject | ✅ |
| Anti AFK — auto-jump every 13s | ✅ |
| Reach | 🔜 Coming soon |
| Velocity | 🔜 Coming soon |
| Fly | 🔜 Coming soon |
| Fast Place | 🔜 Coming soon |

### ⚙️ Settings

| Feature | Status |
|---|---|
| Only in Focus | ✅ |
| HUD Overlay | ✅ |
| Stream Proof | 🔜 Coming soon |
| Discord RPC | 🔜 Coming soon |

---

## Screenshots

<div align="center">

<img src="src/assets/clicker_pagenew.png" width="680" alt="Clicker Page"/>

*Clicker — independent Left / Right profiles with CPS range, randomizer and hotkey binding*

<br/><br/>

<img src="src/assets/movement_pagenew.png" width="680" alt="Movement Page"/>

*Movement — Auto Sprint, No Slow and movement macros*

<br/><br/>

<img src="src/assets/settings_pagenew.png" width="680" alt="Settings Page"/>

*Settings — client options, HUD toggle and version info*

</div>

---

## Download

Download the latest release from the [**Releases**](../../releases) page.

Run `Asfra.exe` — no installer, no dependencies, no setup.

### System Requirements

| | |
|---|---|
| OS | Windows 10 / 11 (64-bit) |
| Disk space | ~45 MB |
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
- ✅ Reads/writes nothing outside the application

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
<sub>Made by <b>svx</b></sub>
</div>
