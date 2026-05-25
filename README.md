# Racketeer

**Self-hosted rack documentation for AV and IT integrators.**

Racketeer is a self-hosted rack management tool that runs as a background service on your local network. Document racks, map every port and cable, track cameras and PAVA systems, manage assets, and generate professional PDF reports — with zero cloud dependency and no data ever leaving your network.

[![Latest Release](https://img.shields.io/github/v/release/Racketeer-io/Racketeer?label=latest&color=4ade80)](https://github.com/Racketeer-io/Racketeer/releases/latest)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20macOS-lightgrey)](#installation)
[![License](https://img.shields.io/badge/license-Commercial-blue)](https://racketeer.io/terms)

---

## Features

- **Visual rack builder** — drag-and-drop device placement with front and back views, 1U–42U, half and quarter-width slots
- **Port & cable mapping** — document every connection, colour-coded by cable type, with status tracking
- **Camera & CCTV documentation** — full NVR camera records including IP, MAC, VLAN, channel, patch location, and cable ID
- **PAVA system documentation** — horn speakers, bi-directional units, fist mics, and yellow phones with full field capture
- **IP conflict detection** — real-time duplicate IP alerts across all devices, cameras, and PAVA units
- **Asset licence tracking** — software, hardware, and subscription licences per site with expiry alerts on the dashboard
- **Audit log** — every change recorded with user, timestamp, and detail — filterable and PDF exportable
- **Custom devices & templates** — build your own device types and save rack layouts for reuse across sites
- **Drive bay documentation** — slot-by-slot drive records for NVRs and servers, with built-in RAID calculator
- **Multi-site management** — organise multiple locations under one installation with instant site switching
- **PDF & CSV exports** — professional branded reports for client handover, as-built records, and compliance
- **Built-in tools** — CCTV storage calculator, RAID calculator, battery capacity calculator

---

## Free Plan

No credit card. No trial timer. Just download and go.

| Plan | Users | Sites | Racks | Price |
|------|-------|-------|-------|-------|
| **Free** | 3 | 5 | 10 | £0 forever |
| Starter | 5 | Unlimited | Unlimited | £149/yr |
| Pro | 15 | Unlimited | Unlimited | £349/yr |
| Team | 30 | Unlimited | Unlimited | £599/yr |

---

## Installation

### Windows

1. Download `Racketeer-Setup-0.3.2.exe` from the [latest release](https://github.com/Racketeer-io/Racketeer/releases/tag/latest)
2. Right-click → **Run as administrator**
3. Follow the wizard — choose your port (default 3000), optionally enter a licence key
4. Open your browser to `http://localhost:[your chosen port]`

No Docker required. Node.js is bundled. Starts automatically at boot as a Windows service.

To change the port after installation: open `C:\Program Files\Racketeer\`, right-click `reconfigure.ps1` → Run with PowerShell.

### Linux

1. Download `Racketeer-0.3.2-linux.zip` from the [latest release](https://github.com/Racketeer-io/Racketeer/releases/tag/latest)
2. Extract and run the installer:

```bash
unzip Racketeer-0.3.2-linux.zip -d racketeer-install
cd racketeer-install
chmod +x install.sh
sudo ./install.sh
```

Node.js 22 is installed automatically on Ubuntu/Debian and RHEL/Fedora.
Open `http://localhost:3000` — or `http://[server-ip]:3000` from another machine.

Runs as a systemd service, starts automatically on boot.

### macOS

1. Download `Racketeer-0.3.2-macos.zip` from the [latest release](https://github.com/Racketeer-io/Racketeer/releases/tag/latest)
2. Extract and run the installer:

```bash
unzip Racketeer-0.3.2-macos.zip -d racketeer-install
cd racketeer-install
chmod +x install.sh
sudo ./install.sh
```

Node.js 22 is installed automatically if Homebrew is present.
Open `http://localhost:3000`.

Runs as a LaunchDaemon, starts automatically at login.

---

## Default Login

| Field | Value |
|-------|-------|
| Username | `admin` |
| PIN | `1234` |

**Change the PIN immediately** after first login — Login → Admin Panel → Users → Edit.

---

## Licence Activation

The Free Plan is active by default — no key required.

To activate a purchased licence: **Admin Panel → License → Enter License Key**. Fully offline — no internet connection needed.

Purchase or upgrade at [racketeer.io](https://racketeer.io/#pricing) or email **hello@racketeer.io**.

---

## Data & Backup

| Platform | Data location |
|----------|--------------|
| Windows | `C:\Program Files\Racketeer\data\db.json` |
| Linux / macOS | `/opt/racketeer/data/db.json` |

Back up `db.json` regularly — it contains your entire database.
Restore by stopping the service, replacing the file, and restarting.

---

## What's New in v0.3.2

- **Free Plan** — 3 users, 5 sites, 10 racks, no licence key required, no expiry
- **Port selection during install** — choose the port Racketeer listens on (default 3000)
- **Post-install port change** — `reconfigure.ps1` lets you change the port at any time without reinstalling

See [CHANGELOG.md](CHANGELOG.md) for the full version history.

---

## Documentation

Full user guide: **[racketeer.io/docs](https://racketeer.io/docs.html)**

---

## Bugs & Feature Requests

Open an issue on [GitHub Issues](https://github.com/Racketeer-io/Racketeer/issues).
Include what you were doing, what you expected, and what happened. Screenshots always welcome.

---

## Licence

Commercial software. Free Plan available permanently at no cost.
See [racketeer.io](https://racketeer.io) for full pricing and licence terms.
