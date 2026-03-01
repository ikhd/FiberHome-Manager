# FiberHome Manager

<p align="center">
  <img src="assets/logo.png" width="120" alt="FiberHome Manager Logo">
</p>

<p align="center">
  <strong>Advanced Desktop Management Tool for FiberHome LTE / 5G Routers</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows-blue">
  <img src="https://img.shields.io/badge/Type-Desktop%20Application-darkgreen">
  <img src="https://img.shields.io/badge/Status-Closed%20Source-red">
  <img src="https://img.shields.io/badge/Version-v1.0-orange">
</p>

---

## Overview

FiberHome Manager is a professional Windows desktop application built for advanced users who require full visibility and control over FiberHome LTE / 5G routers.

The application provides real-time signal analytics, Carrier Aggregation monitoring, neighbor cell inspection, and advanced network control tools through a modern dashboard interface.

> The project is currently distributed as a standalone EXE and is not open source.

---

## Core Features

### Real-Time Signal Analytics
- RSRP
- RSRQ
- SINR
- Device Temperature
- EARFCN / Channel
- Band
- PCI
- Firmware Version
- Uptime

### Carrier Aggregation (CA)
- PCC / SCC monitoring
- LTE & NR aggregation visibility
- Activation state tracking

### Neighbor Cell Monitoring
- Nearby LTE / 5G tower detection
- SINR & RSRP comparison
- EARFCN identification
- Band & PCI mapping
- Signal strength analysis for tower optimization

### Advanced Network Controls
- Band Locking
- AT Command execution
- IMEI management
- IP monitoring
- Automated login/logout handling

---

## Screenshots

### Dashboard
![Dashboard](assets/screenshots/dashboard.png)

### Carrier Aggregation
![Carrier Aggregation](assets/screenshots/ca.png)

### Neighbor Cells Monitoring
![Neighbor Cells](assets/screenshots/neighbor-cells.png)

---

## Installation

1. Download the latest EXE from the **Releases** section.
2. Run the application.
3. No additional installation required.

---

## Build (Internal Use Only)

```bash
python -m PyInstaller --noconsole --onefile ^
--icon=templates/static/icon.ico ^
--add-data "templates;templates" ^
--distpath ./APP ^
--name "Fiberhome Manager" ^
desktop_app.py
