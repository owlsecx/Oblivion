# 🦉 Oblivion

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OForensics-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **Oblivion** — Ransomware Shield & Security Guard

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview


Oblivion is a secure data-wiping and anti-forensics tool that irreversibly destroys files, free space and metadata on authorized systems. It overwrites data with multiple passes, removes filesystem traces and verifies erasure. It is intended strictly for authorized data-sanitization and decommissioning tasks.

---

## ✨ Features


- Multi-pass secure overwriting of files and directories
- Free-space wiping to remove recoverable deleted data
- Metadata and filesystem-trace removal
- Configurable overwrite patterns and pass count
- Erasure verification and a structured wipe log
- Offline operation with a --self-test mode

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage


```bash
./Oblivion
./Oblivion --self-test
./Oblivion --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
