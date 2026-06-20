# Aegentis Protector / PyAegentis
Python source protector for encrypting and protecting your applications, turning .py files into encrypted runtime packages with pyd output and PyInstaller EXE support.

> **Version:** 0.3.0 · **Platform:** Windows x64 · **Python:** 3.12  
> **License:** Proprietary — not open source. Authorized access only.

---

## Overview

Aegentis Protector (PyAegentis) is a build-time protection utility for Python applications.

The tool:

- Compiles `.py` source into **AEGBC** (custom bytecode container)
- Encrypts payload with sharded AES-GCM (**AEGSH** format)
- Seals runtime modules inside an encrypted vault (no plain `.py` on disk)
- Builds **facade** + **native** `.pyd` pair per protect run
- Embeds master key in native pyd (release mode)
- Optionally packs output with **PyInstaller onefile EXE**
- Supports external hardening (e.g. **Themida** on native pyd)

---

## Requirements

- Python **3.12**
- Windows 10/11 x64
- MSVC Build Tools
- PyInstaller 6+
- Themida (optional, manual — release native pyd)

---
