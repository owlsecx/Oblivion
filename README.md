# 🛡️ Oblivion

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-OForensics%20%2F%20Real-time%20Defense-cyan?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-watchdog%20%2B%20psutil-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v2.0-cyan?style=flat-square"/>
</p>

> **Oblivion** is a real-time ransomware shield and behavioral detection system. It monitors the filesystem for suspicious burst activity, high-entropy file creation, suspicious extensions, and automatically terminates known ransomware processes.

---

## 📌 Overview

Oblivion acts as a proactive defense layer against ransomware. It watches a chosen directory (or the entire user home) and triggers containment actions when multiple indicators match (burst of file changes + high entropy files + suspicious extensions).

**Detection is based on 2-of-3 flags** for high accuracy and low false positives.

---

## 🖥️ Modules

| # | Module                  | Description |
|---|-------------------------|-------------|
| **[1]** | **Live Guard**              | Start real-time ransomware monitoring |
| **[2]** | **Deep Scan**               | One-time folder scan for threats |
| **[3]** | **Process Manager**         | List and kill suspicious processes |
| **[4]** | **Entropy Check**           | Check file/folder entropy levels |
| **[5]** | **Threat Log**              | View and export alert history |
| **[6]** | **Settings**                | Configure watch path, thresholds, auto-kill |

---

## 📊 Key Features

- **Real-time Filesystem Monitoring** using watchdog
- **Behavioral Detection** — burst of file events + unique files
- **Entropy Analysis** — detects encrypted/packed files (H ≥ 7.20)
- **Suspicious Extension Detection** — .locked, .enc, .crypt, .wncry, etc.
- **Automatic Process Termination** — kills processes with ransomware keywords
- **Threat Scoring** (0-100) with clear levels (SAFE → CRITICAL)
- **Alert Logging** — persistent JSON log with timestamps
- **Configurable Thresholds** — burst window, entropy cutoff, high-entropy trigger

---

## ⚙️ Requirements

- **Linux** (recommended)
- **watchdog**: `pip install watchdog`
- **psutil**: `pip install psutil` (for process killing)

---

## 🚀 Usage

```bash
sudo ./Oblivion

📁 Output

Live Terminal Feed — real-time colored alerts with timestamps
Threat Log — persistent JSON log with all events
Export — full JSON report of alert history
Statistics — events per window, unique files, high-entropy count


📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.

DEFENSIVE USE ON AUTHORISED SYSTEMS ONLY
