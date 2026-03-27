
# Week 1 — 27/03/2026 to 03/04/2026
---
## Session 1 — 27/03/2026
**Goal:** Install Proxmox on EliteDesk
### What I Did
- Downloaded Proxmox VE 9.1 ISO Installer
- Flashed USB with Rufus (Etcher failed)
- Configured static IP 192.168.1.200
- Accessed Proxmox web UI via browser at https://192.168.1.200:8006/
- Disabled enterprise repos, added no-subscription
- Updated system with apt-get dist-upgrade
## What Broke and How I Fixed It
**Problem:** Balena Etcher failed with requestMetadata error  
**Fix:** Switched to Rufus

**Problem:** apt-get update returned 401 on enterprise repos  
**Fix:** Disabled both enterprise repos, added no-subscription repo

### Key Commands
```bash
apt-get update # Refresh the list of available packages
apt-get dist-upgrade -y
```
### What I Learned
- Learned what an ISO file is and how to flash one onto a USB using Rufus
- Understood the difference between Type 1 and Type 2 hypervisors and why Proxmox is the professional choice for homelabs
- Learned how client-server architecture works - browser sends request, Proxmox listen on port 8006 and responds
- APT package manager basics
### Next Session
Upload Windows Server 2022 ISO and create first VM.
---
## Session 2 — 28/03/2026
**Goal:** ...
