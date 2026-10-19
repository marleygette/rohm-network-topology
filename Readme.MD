<div align="center">

# ROHM Electronics Philippines Inc.
### Enterprise & Factory Network Topology — Interactive 3D

An animated 3D visualization of a Cisco Packet Tracer hybrid network, built with Three.js.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=three.js&logoColor=white)
![Cisco](https://img.shields.io/badge/Cisco_Packet_Tracer-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-d6101f?style=for-the-badge)

**[Live Demo](https://marleygette.github.io/rohm-network-topology/)** · **[Report a Bug](../../issues)**

</div>

---

## Overview

This project turns the `MARGARETTE.pkt` Packet Tracer file into a 3D scene you can orbit, zoom, and click. It shows how ROHM Electronics' office, server, and factory networks connect, with live packets moving along every link.

## Features

- Four network zones laid out on a 3D floor
- Models for firewalls, core switches, servers, PCs, printers, access points, and the SMT line
- Packets animate along links, colored by VLAN
- Click any device to see its IP address, subnet mask, and VLAN
- Auto-rotate, top view, pause packets, and reset camera controls
- Light and dark mode, and a layout that works on phones

## Network zones

| # | Zone | Main devices |
|---|------|--------------|
| 1 | Enterprise Core & Internet | WAN cloud, redundant ASA 5506 firewalls, redundant Catalyst 3650 core switches |
| 2 | Server Farm | Server access switches, ERP, MES, main database, AD/DNS |
| 3 | Administrative & Office | Cisco 2960 aggregation switch, PCs, workstations, printers, access point, smartphones |
| 4 | Factory Floor & Industrial | C3332 industrial switch, rugged Ethernet switches, SMT line, AOI system |

## VLAN plan

| VLAN | Purpose | Subnet |
|------|---------|--------|
| 10 | Server Farm | 192.168.10.0/24 |
| 20 | Office & Departments | 192.168.20.0/24 |
| 30 | Industrial SMT | 192.168.30.0/24 |
| 40 | Wireless & IoT | 192.168.40.0/24 |

## Run it

No build step. Open `index.html` in any modern browser.

```bash
git clone https://marleygette.github.io/rohm-network-topology/
cd rohm-network-topology-3d
# open index.html
```

To host it free, go to **Settings → Pages**, choose the `main` branch and the `/ (root)` folder, then save.

## Controls

| Action | Input |
|--------|-------|
| Orbit | Left-drag |
| Pan | Right-drag |
| Zoom | Scroll |
| Device details | Click a device |

## Project team

| Role | Name |
|------|------|
| Team Leader | Mary Leydi Margarette C. Fernandez |
| Member | Kevin Russell Samson |
| Member | Junaid Baunto |
| Member | Wendal Alcantara |
| Member | RJ Cea |

## License

Released under the MIT License. This is a school project; ROHM branding belongs to its owner.
