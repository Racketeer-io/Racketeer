<div align="center">

# Racketeer

**Visual rack documentation for AV and IT integrators.**

[![Latest Release](https://img.shields.io/badge/latest-v0.3.2-3ecf6b)](https://github.com/Racketeer-io/Racketeer/releases/tag/latest)
[![License](https://img.shields.io/badge/license-Commercial-5a6ad0)](https://racketeer.io/terms)
[![Platform](https://img.shields.io/badge/platform-Windows-lightgrey)](#download)

</div>

---

Racketeer is a self-hosted rack documentation tool that lets you build accurate, visual rack diagrams — fast. No Visio. No spreadsheets. No chasing colleagues for a diagram that's already out of date.

<div align="center">

![A Racketeer rack elevation showing a firewall, core switch, two servers, a NAS and a UPS, with the rack's power draw and heat output above it](assets/screenshots/rack-elevation.png)

</div>

## Contents

- [Features](#features)
- [See it in action](#see-it-in-action)
- [Screenshots](#screenshots)
- [Free Plan](#free-plan)
- [Download](#download)
- [Getting Started](#getting-started)
- [Data & Backup](#data--backup)
- [Licensing](#licensing)
- [Support](#support)
- [Changelog](#changelog)

---

## Features

- **Drag-and-drop rack builder** — position devices exactly where they sit in the rack
- **50+ device types** — servers, switches, patch panels, PDUs, UPS, AV equipment, cameras, and more
- **Multi-site management** — organise racks across unlimited sites and locations
- **PDF export** — generate client-ready rack diagrams in one click
- **Port mapping** — document every RJ45, fibre, HDMI, and USB connection
- **IP address management** — subnets, an IP registry, duplicate-address flagging, and colour-coded VLANs
- **Engineer tools** — built-in subnet, CCTV storage, RAID capacity, and UPS runtime calculators
- **Audit log** — see who changed what and when
- **Asset licensing** — track software and hardware licence expiry dates
- **Custom devices** — add any device type not in the built-in library
- **Rack templates** — save and reuse common rack configurations
- **Multi-user** — invite your team with admin or viewer roles
- **Maintenance log** — record planned and completed maintenance per device
- **Offline-first** — runs entirely on your network, no cloud dependency

---

## See it in action

### Build a rack from scratch

Add a site, add a rack, drop devices in from the palette, fill in the details, and watch the power and heat totals add up.

![Creating a site and a rack, dropping devices into a 42U elevation from the palette, and editing a device's details while the rack's power and heat totals update](assets/gifs/rack-builder.gif)

### Ports, patching and VLANs

Open any device to see its ports, pick where each cable goes, and tag the VLAN, cable type, cable ID and length. The link shows on both ends.

![Opening a switch's ports, connecting a port to a port on another device, tagging it with a VLAN, cable type, ID and length, and seeing the link on both devices](assets/gifs/ports-and-vlans.gif)

### IP address management

Subnets with live utilisation, a searchable registry of every IP, duplicate addresses flagged, and colour-coded VLANs.

![Browsing subnets and their usage, the IP registry with its filters, and the colour-coded VLAN list](assets/gifs/ip-management.gif)

### Maintenance logs

See the next service date on every site, then log a visit straight from the rack: who did it, what was done, when it's due next, and a built-in inspection checklist where failures get a note.

![Viewing next service dates on the dashboard, adding a maintenance entry, working through the inspection checklist, and seeing the entry in the maintenance history](assets/gifs/maintenance-log.gif)

### Engineer tools

Subnet, CCTV storage and bandwidth, RAID capacity, and UPS runtime calculators, built in. No spreadsheets.

![Using the IPv4 subnet, CCTV storage, RAID capacity and battery runtime calculators](assets/gifs/engineer-calculators.gif)

---

## Screenshots

### Dashboard

Every site, rack and device at a glance, with next service dates and IP conflict counts.

![The dashboard showing totals for sites, racks, devices, expiring licences and IP conflicts, with a card for each site and its racks](assets/screenshots/dashboard.png)

### IP registry

Every address with its gateway, VLAN, device, rack and site.

![The IP registry table listing each address with its gateway, MAC, VLAN, type, device, rack and site](assets/screenshots/ip-registry.png)

<table>
<tr>
<td width="50%" valign="top">
<img src="assets/screenshots/port-details.png" alt="The port details dialog with VLAN, cable type, cable ID, length and status fields"><br>
<sub><b>Port details</b> — connect a port and tag the VLAN, cable type, ID and length.</sub>
</td>
<td width="50%" valign="top">
<img src="assets/screenshots/maintenance-checklist.png" alt="The maintenance entry inspection checklist with ticked items and a failure note"><br>
<sub><b>Maintenance checklist</b> — tick items off, and add a note to anything that fails.</sub>
</td>
</tr>
</table>

### Engineer tools

![The battery calculator showing estimated UPS runtime and usable energy for a given load](assets/screenshots/engineer-calculators.png)

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

## Download

### Windows Installer

Download the latest `.exe` from the [Releases page](https://github.com/Racketeer-io/Racketeer/releases/tag/latest).

Run the installer — Racketeer starts on `http://localhost:3000` automatically. No Docker, no containers — Node.js is bundled and it installs as a native Windows service.

Requires Windows 10/11 (64-bit). macOS and Linux support is coming soon.

---

## Getting Started

1. Download and install
2. Open `http://localhost:3000`
3. Create your first site and add a rack
4. Start adding devices

No account registration. Your data stays on your machine.

---

## Data & Backup

All data lives in `data/db.json` in the install directory. Back it up by copying that file. Restore by dropping it back in p

---

## Licensing

Racketeer is commercial software. The Free Plan is permanently free — no expiry, no card required. Paid plans are licensed a

[View pricing →](https://racketeer.io/#pricing)

---

## Support

- Docs: [racketeer.io/docs](https://racketeer.io/docs.html)
- Email: hello@racketeer.io
- Issues: [Racketeer-io/Racketeer/issues](https://github.com/Racketeer-io/Racketeer/issues)

---

## Changelog

Full history on the [Releases page](https://github.com/Racketeer-io/Racketeer/releases).

- **v0.3.2** — Free Plan (3 users, 5 sites, 10 racks, no license key required)
- **v0.3.1** — Maintenance log, subnet/VLAN documentation, improved PDF export
- **v0.3.0** — Multi-user accounts, audit log, asset licensing

---

<div align="center">

*Built for the integrators who build the infrastructure everyone else relies on.*

</div>
