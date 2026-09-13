<div align="center">

<a href="https://github.com/Akhouri-Anmol-Kumar/ATLOCK">
  <img src="https://readme-typing-svg.demolab.com?font=Righteous&size=55&duration=3000&pause=1500&color=C9B97A&center=true&vCenter=true&width=600&height=90&lines=%F0%9F%94%92+ATLOCK;TOTAL+SECURITY+SUITE" alt="ATLOCK" />
</a>

**The Total Security Suite for Windows.**
One `.exe`. Zero installers. Zero compromises.

<p>
  <img src="https://img.shields.io/github/v/release/Akhouri-Anmol-Kumar/ATLOCK?style=for-the-badge&color=c9b97a&labelColor=0a0a0a&label=version" alt="version">
  <img src="https://img.shields.io/badge/platform-Windows%2010%2B-4a7ab5?style=for-the-badge&labelColor=0a0a0a" alt="platform">
  <img src="https://img.shields.io/github/license/Akhouri-Anmol-Kumar/ATLOCK?style=for-the-badge&color=4a9e6b&labelColor=0a0a0a" alt="license">
  <img src="https://img.shields.io/badge/made%20in-India-4a9e6b?style=for-the-badge&labelColor=0a0a0a" alt="made in India">
</p>

<p>
  <img src="https://img.shields.io/github/stars/Akhouri-Anmol-Kumar/ATLOCK?style=flat-square&color=c9b97a" alt="stars">
  <img src="https://img.shields.io/github/downloads/Akhouri-Anmol-Kumar/ATLOCK/v4.0/total?style=flat-square&color=4a7ab5&label=v4.0%20downloads" alt="v4.0 downloads">
  <img src="https://img.shields.io/github/last-commit/Akhouri-Anmol-Kumar/ATLOCK?style=flat-square&color=4a9e6b" alt="last commit">
  <img src="https://img.shields.io/github/issues/Akhouri-Anmol-Kumar/ATLOCK?style=flat-square&color=c94a4a" alt="issues">
</p>

<br>

<a href="https://github.com/Akhouri-Anmol-Kumar/ATLOCK/releases/download/v4.0/ATLOCK.zip">
  <img src="https://img.shields.io/badge/⬇️_DOWNLOAD_ATLOCK_v4.0-c9b97a?style=for-the-badge&labelColor=0a0a0a&logoColor=white" alt="Download ATLOCK v4.0" height="55">
</a>

<sub>Direct download · no sign-up · no ads</sub>

<br><br>

<p>
  <a href="#-features">Features</a> ·
  <a href="#-installation">Installation</a> ·
  <a href="#-faq">FAQ</a> ·
  <a href="#-roadmap">Roadmap</a>
</p>

</div>

<br>

<p align="center">
  <img width="640" alt="ATLOCK screenshot" src="https://github.com/user-attachments/assets/0c3e061f-b19f-4a43-856c-9618e4c8b83b" />
</p>

---

## 🧭 What is ATLOCK?

> *"We build what others forgot to fix."* — Akhouri Systems

ATLOCK is a **Total Security Suite for Windows** — built by one developer who got tired of half-baked "lock apps" that promise security and deliver a password prompt.

- 📦 Single portable `.exe`
- 🚫 No installation, no setup wizard
- ▶️ Download → Run → Done

<br>

## 📋 Table of Contents

- [Windows Defender Warning](#️-windows-defender-warning--this-is-a-false-positive)
- [Features](#-features)
- [Security Hardening](#️-security-hardening)
- [Architecture](#-architecture)
- [Installation](#-installation)
- [What's New in v4.0](#-whats-new-in-v40)
- [FAQ](#-faq)
- [Roadmap](#-roadmap)
- [Disclaimer](#️-disclaimer)
- [License](#-license)
- [About](#️-about)

<br>

## ⚠️ Windows Defender Warning — This Is a False Positive

Windows may flag ATLOCK as an *"unrecognized app"* or *suspicious*. This is a well-known false positive for unsigned, PyInstaller-built Python applications — **it is not malware.**

<details>
<summary><b>🛠️ How to run it anyway</b></summary>
<br>

1. Click **"More info"** on the SmartScreen warning
2. Click **"Run anyway"**
3. ATLOCK opens normally ✅

> Code signing is on the [roadmap](#-roadmap) to remove this warning entirely.

</details>

<br>

## ✨ Features

<table>
<tr>
<td width="50%" valign="top">

### 🔒 System Lockdown
Lock your entire system for a set duration. Once locked — no bypass, no escape.
- `Alt + Tab` blocked
- `Win` key blocked
- Task Manager killed on sight
- One emergency unlock available — use it wisely

</td>
<td width="50%" valign="top">

### 🛡️ File Guard
NTFS ACL-level file locking — the deepest access control Windows allows.
- Protected files can't be opened, moved, copied, or deleted, not even by admins
- Guard up to **10 files** simultaneously
- 3 wrong attempts trigger the intruder response

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔑 Password Vault
Local, **AES-encrypted** (Fernet) storage for anything sensitive — emails, UPI PINs, bank details.
- Master password hashed with **PBKDF2-HMAC-SHA256**, 200,000 iterations
- 3 wrong attempts → warning
- 4th wrong attempt → **10-hour hard lockout** on the entire app
- All attempts masked before logging — never stored in plaintext

</td>
<td width="50%" valign="top">

### 📸 Intruder Ops
Every wrong attempt gets a response.
- 📷 Photo captured on the 1st wrong attempt
- 🎥 10-second video captured on escalation (3rd/4th wrong)
- 🔊 Audible alarm on critical intrusion
- Auto-saved to your Pictures / Videos gallery

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔔 Security Notification Panel
A real-time, in-app notification center.
- Every security event logged: failed unlocks, intruder attempts, file guard triggers
- Auto-deleted after 24 hours
- Live unread badge counter

</td>
<td width="50%" valign="top">

### ⚙️ Settings & Control
Full control from one clean panel.
- Toggle photo / video capture
- Toggle sound & alarm tones
- Jump straight to the intruder media gallery
- Live dependency/status check

</td>
</tr>
</table>

<br>

## ⚔️ Security Hardening

| Mechanism | What it does |
|---|---|
| Low-level `WH_KEYBOARD_LL` hook | Blocks `Alt+Tab`, `Win`, `Esc`, `Alt+F4` system-wide during lockdown |
| Background watchdog thread | Instantly kills Task Manager, Process Hacker, ProcExp |
| Continuous focus enforcement | `grab_set()` + `focus_force()` loop — no window can steal focus |

<br>

## 🏗️ Architecture

```mermaid
flowchart TD
    A[ATLOCK v4 — Lockdown Engine] --> B[File Guard]
    A --> C[Password Vault]
    A --> D[Intruder Ops]
    B --> B1[NTFS ACL Control]
    C --> C1[Fernet Encryption + PBKDF2]
    D --> D1[Camera Capture]
    B1 --> E[Notification Center]
    C1 --> E
    D1 --> E
```

<br>

## 📦 Installation

1. Download `ATLOCK_v4.exe` from the [Releases page](https://github.com/Akhouri-Anmol-Kumar/ATLOCK/releases/latest)
2. Extract it (if zipped)
3. Run `ATLOCK_v4.exe`

**That's it.** No Python required. No installation. No admin setup.

| Requirement | Details |
|---|---|
| OS | Windows 10 or later |
| Runtime | None — fully bundled |
| Camera | Optional, enables Intruder Ops photo/video capture |

<br>

## 🆕 What's New in v4.0

- 🔐 Password Vault re-engineered with real AES encryption (Fernet + PBKDF2, 200k iterations), replacing the old, weaker encoding scheme
- 🧹 Removed external Gmail/Telegram alert integrations for a leaner, fully self-contained app — zero external accounts, tokens, or internet dependency required
- 🎬 Refined Intruder Ops pipeline (photo → escalation → video → alarm)
- 🖥️ Redesigned Settings panel

<br>

## ❓ FAQ

<details>
<summary><b>Is ATLOCK safe to run?</b></summary>
<br>
Yes. It's a locally-run, offline security tool. The Defender warning is a standard false positive for unsigned PyInstaller apps, not a sign of malicious behavior.
</details>

<details>
<summary><b>Does ATLOCK send my data anywhere?</b></summary>
<br>
No. As of v4.0, ATLOCK has zero external integrations — everything (vault, photos, videos, logs) stays on your machine.
</details>

<details>
<summary><b>What happens if I forget my master password?</b></summary>
<br>
There is currently no recovery mechanism by design, this is what makes the vault secure. Store your master password somewhere safe before relying on ATLOCK.
</details>

<details>
<summary><b>Can I unlock a guarded file in an emergency?</b></summary>
<br>
System Lockdown includes one emergency unlock. File Guard does not currently have a bypass, that's the point of ACL-level locking. Be careful about which files you guard.
</details>

<br>

## 🗺️ Roadmap

- [ ] Code signing to eliminate the SmartScreen warning
- [ ] Configurable lockdown/unlock schedules
- [ ] Encrypted cloud backup for the vault (opt-in)
- [ ] Multi-monitor lockdown support

<br>

## ⚠️ Disclaimer

ATLOCK is intended for personal device security on machines you own or are authorized to manage. Features like Task Manager termination, keyboard hooking, and camera-based intruder capture are powerful, use responsibly and in compliance with local laws and workplace policies. The developer is not responsible for data loss resulting from forgotten passwords or misuse of the lockdown/file-guard features.

<br>

## 🤝 Contributing

Issues and feature requests are welcome via the [Issues tab](https://github.com/Akhouri-Anmol-Kumar/ATLOCK/issues). Pull requests are welcome, please open an issue first to discuss significant changes.

<br>

## 📄 License

Licensed under the **MIT License** — see [LICENSE](LICENSE) for details.

<br>

## 🏛️ About

<div align="center">

**ATLOCK** is a product of **Akhouri Systems** — a desktop software company built on one idea:
*if existing software frustrates you, build something better.*

Developed solely by **Akhouri Anmol Kumar** · Indian Software Developer

<sub>An Akhouri Systems Product</sub>

</div>
