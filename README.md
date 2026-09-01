<div align="center">

# 🔒 ATLOCK

### *An Akhouri Systems Product*

**Total Security Suite for Windows — one `.exe`, zero compromises.**

![Version](https://img.shields.io/badge/version-4.0-c9b97a?style=for-the-badge&labelColor=0a0a0a)
![Platform](https://img.shields.io/badge/platform-Windows%2010%2B-4a7ab5?style=for-the-badge&labelColor=0a0a0a)
![License](https://img.shields.io/badge/license-MIT-4a9e6b?style=for-the-badge&labelColor=0a0a0a)
![Made in India](https://img.shields.io/badge/made%20in-India-4a9e6b?style=for-the-badge&labelColor=0a0a0a)

<br>

<img width="600" height="633" alt="Image" src="https://github.com/user-attachments/assets/0c3e061f-b19f-4a43-856c-9618e4c8b83b" />

### ⚡ Zero-Effort Launch

**Don't want to dig through repo files or hunt for the Releases tab?**
Click the button below — grab the latest ready-to-run build in one click.

[![Download Latest Release](https://img.shields.io/github/v/release/Akhouri-Anmol-Kumar/ATLOCK?style=for-the-badge&color=c9b97a&labelColor=0a0a0a&label=⬇️%20DOWNLOAD%20ATLOCK)](https://github.com/Akhouri-Anmol-Kumar/ATLOCK/releases/latest)

</div>

---

## 🧭 What is ATLOCK?

> *"We build what others forgot to fix."* — **Akhouri Systems**

ATLOCK is a **Total Security Suite for Windows**, built by one developer who got tired of half-baked lock apps that promise security and deliver a password prompt.

- 📦 Single `.exe`
- 🚫 No installation
- 🧙 No setup wizard
- ▶️ Just run it

---

## ⚠️ Windows Defender Warning — This Is a False Positive

Windows may flag ATLOCK as *"unrecognized app"* or *suspicious*. This is a **known false positive** common with unsigned, PyInstaller-built Python applications — not a sign of malware.

<details>
<summary><b>🛠️ How to run it anyway (click to expand)</b></summary>
<br>

1. Click **"More info"** on the SmartScreen warning
2. Click **"Run anyway"**
3. ATLOCK opens normally ✅

</details>

---

## ✨ Features — v4.0

<table>
<tr>
<td width="50%" valign="top">

### 🔒 System Lockdown
Lock your entire system for a set duration. Once locked — no bypass, no escape.
- `Alt + Tab` blocked
- `Win` key blocked
- Task Manager killed on sight
- One **emergency halve** available — use it wisely

</td>
<td width="50%" valign="top">

### 🛡 File Guard
NTFS ACL-level file locking — the deepest access control Windows allows.
- Protected files can't be opened, moved, copied, or deleted — **not even by admins**
- Guard up to **10 files** simultaneously
- 3 wrong attempts trigger intruder response

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔑 Password Vault
Local, **AES-encrypted** (Fernet) storage for anything sensitive — emails, UPI PINs, bank details.
- Master password hashed with **PBKDF2-HMAC-SHA256**, 200,000 iterations
- 3 wrong attempts = warning
- 4th wrong attempt = **10-hour hard lockout** on the entire app
- All attempts masked before logging — never stored in plaintext

</td>
<td width="50%" valign="top">

### 📸 Intruder Ops
Every wrong attempt gets a response.
- 📷 Photo captured on the **1st** wrong attempt
- 🎥 **10-second video** captured on escalation (3rd/4th wrong)
- 🔊 Audible alarm on critical intrusion
- Auto-saved to your Pictures / Videos gallery

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔔 Security Notification Panel
A real-time, in-app notification center.
- Every security event logged — failed unlocks, intruder attempts, file guard triggers
- Auto-deleted after **24 hours**
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

---

## ⚔️ Security Hardening
Low-level WH_KEYBOARD_LL hook
→ blocks Alt+Tab, Win key, Escape, Alt+F4 system-wide
🐕 Background watchdog thread
→ kills Task Manager, Process Hacker, ProcExp instantly
🎯 Continuous focus enforcement
→ grab_set() + focus_force() loop, no window can steal focus

---
                 ATLOCK v4

       Lockdown Engine
             │
 ┌───────────┼────────────┐
 │           │            │

File Guard  Vault   Intruder Ops

 │           │            │

ACL      Encryption   Camera

 │           │            │

 └───────────┼────────────┘

      Notification Center

## 📦 Installation

Download the .exe from the Releases page (or click the button above)
Extract (if zipped)
Run ATLOCK_v4.exe


**That's it.** No Python required. No installation. No admin setup.

| Requirement | Details |
|---|---|
| OS | Windows 10 or later |
| Runtime | None — fully bundled |
| Camera | Optional, enables Intruder Ops photo/video capture |

---

## 🆕 What's New in v4.0

- 🔐 Password Vault re-engineered with **real AES encryption** (Fernet + PBKDF2, 200k iterations) — replacing the old, weaker encoding scheme
- 🧹 Removed external Gmail/Telegram alert integrations for a **leaner, fully self-contained** app — zero external accounts, tokens, or internet dependency required to run ATLOCK
- 🎬 Refined Intruder Ops pipeline (photo → escalation → video → alarm)
- 🖥️ Redesigned Settings panel

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 🏛️ About

<div align="center">

**ATLOCK** is a product of **Akhouri Systems** — a desktop software company built on one idea:
*if existing software frustrates you, build something better.*

Developed solely by **Akhouri Anmol Kumar**
*Indian Software Developer*

---

**An Akhouri Systems Product** · Developed by **Akhouri Anmol Kumar** · Indian Software Developer

</div>
