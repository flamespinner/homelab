# HomeLab

My homelab documentation, plans, network diagrams, useful scripts and just general experimental homelab stuff.

<br />

## Current Setup (as of 7/10/2026)

Everything lives in a 10" rack.

**Turing Pi 2** — cluster board hosting 2x Raspberry Pi CM4 and 2x Jetson Nano 2GB.
| Node | Role |
|--|--|
| CM4 #1 | Local dev environment. Hosts most of my main homelab apps — projects I'm actively working on/testing, dashboards, monitoring, Discord bots, Tandoor Recipes, Jorgejo, and various custom-built tools/full-stack apps for day-to-day life. |
| CM4 #2 | Runs my custom-written Kanban board that aggregates tasks from multiple sources (day job, freelance, Calico County, other personal projects). Also hosts my main MCP server with custom tools for automating daily tasks. |
| Jetson Nano 2GB x2 | Installed on the board. |

**File server** — custom-built box (specs TBD) running Unraid as primary file storage. Also hosts services like Pi-hole.

**LLM platform** *(new)* — Ryzen 5800X, 16GB RAM, ASUS ROG Strix (Phantom Gaming X) motherboard, dual Nvidia P40 GPUs. Runs Hermes as the primary agent along with llama.cpp for local LLM inference.

**Networking** — UniFi USG gateway + UniFi 24-port switch tying the whole rack together with an asymmetrical 1gig fiber connection.

<br />

## Historical Setup

Original lab, as of 5/21/2020:

| # | Device | Use |
|--|--|--|
| 1 | Poweredge 2950 | ESXi — 6x 75GB SCSI in RAID 5 |
| 2 | Poweredge 1950 | 2x 1TB SAS in RAID 1 — Ubuntu Server |
| 1 | Cisco 1812 Router | Cisco Lab |
| 1 | Cisco Catalyst 2950 | VLAN — Cisco Lab and office network |
| 1 | Cisco 1700 | Cisco Lab |
