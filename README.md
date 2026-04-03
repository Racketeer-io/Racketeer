# Racketeer

**Offline-first rack documentation for fire & security, IT, and AV integrators.**

Racketeer is a self-hosted rack management system that runs as a background service on your local network. Document racks, map port connections, track cameras and PAVA systems, manage assets, and generate professional PDF reports - with zero cloud dependency and no data ever leaving your network.

---

## Features

- **Visual rack builder** - drag-and-drop device placement with front and back views, 1U–42U, half and quarter-width slots
- **Port & cable mapping** - document every connection, colour-coded by cable type, with status tracking (active / reserved / disconnected)
- **Camera & CCTV documentation** - full NVR camera records including IP, MAC, VLAN, channel, patch location, and cable ID
- **PAVA system documentation** - horn speakers, bi-directional units, fist mics, and yellow phones with full field capture
- **IP conflict detection** - real-time duplicate IP alerts across all devices, cameras, and PAVA units
- **Asset licence tracking** - software, hardware, and subscription licences per site with expiry alerts on the dashboard
- **Audit log** - every change recorded with user, timestamp, and detail - filterable and PDF exportable
- **Custom devices & templates** - build your own device types and save rack layouts for reuse across sites
- **Drive bay documentation** - slot-by-slot drive records for NVRs and servers, with built-in RAID calculator
- **Multi-site management** - organise multiple locations under one installation with instant site switching
- **PDF & CSV exports** - professional branded reports for client handover, as-built records, and compliance
- **Import & export** - full JSON backup and restore, no data locked to one machine
- **Connections report** - cross-site port connection report filterable by site, rack, cable type, or status
- **Built-in tools** - CCTV storage calculator, RAID calculator, battery capacity calculator

---

## Installation

### Windows

1. Download `Racketeer-Setup-x.x.x.exe` from the [latest release](../../releases/latest)
2. Run the installer - Racketeer registers as a Windows Service automatically
3. Open your browser to **http://localhost:3000** or The IP of the machine.

No Docker required. No configuration needed. Starts automatically at boot.

### macOS / Linux (Docker)

Download the platform package from the [latest release](../../releases/latest):

```bash
# Load the image
docker load -i racketeer-image.tar.gz

# Start the service
docker-compose up -d
```

Open **http://localhost:3000**

**Requirements:** Docker Desktop · macOS 12+ · Ubuntu 20.04+

---

## Default Login

| Field | Value |
|----------|---------|
| Username | `admin` |
|   PIN    | `0000`  |

**Change the PIN immediately** after first login via Admin → Accounts.

---

## Licence Activation

The beta build ships pre-activated with a 999-seat licence valid until March 2027. No activation required to evaluate.

To activate a purchased licence: **Admin → License → paste your key**. Fully offline - no internet connection required.

For production licences visit **[racketeer.io](https://racketeer.io)** or email **hello@racketeer.io**.

---

## Data & Backup

All data is stored in `data/db.json`. Back up the `data/` folder regularly — it contains your entire database and licence key.

---

## What's New in v0.3.1

- **Asset Licence Tracking** (Pro+) - track software/hardware/subscription licences per site with expiry alerting
- **Branded PDF exports** (Pro+) - company logo on all exported PDFs when App Branding is configured
- **Expiring Licences dashboard card** - amber alert for licences expiring within 30 days

See [CHANGELOG.md](CHANGELOG.md) for the full version history.

---

## Documentation

Full user guide and feature documentation: **[racketeer.io](https://racketeer.io)**

---

## Feedback & Bugs

Open an issue and include what you were doing, what you expected, and what happened. Screenshots always welcome.

---

## Licence

Commercial software. See [racketeer.io](https://racketeer.io) for pricing and licence terms.
