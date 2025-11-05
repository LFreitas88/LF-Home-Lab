# 🧠 LF-Home-Lab

![Debian](https://img.shields.io/badge/Debian-12%20Bookworm-A81D33?logo=debian&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Enabled-2496ED?logo=docker&logoColor=white)
![Security](https://img.shields.io/badge/Security-Hardened-green?logo=security&logoColor=white)
![License](https://img.shields.io/badge/License-CC0--1.0-lightgrey.svg)
![Last Commit](https://img.shields.io/github/last-commit/LFreitas88/LF-Home-Lab)

> **Cybersecurity homelab documentation: Debian server hardening, self-hosted services, and infrastructure setup**

---

## 👨‍💻 About Me

**Leandro Freitas** | Cybersecurity Student @ Bergen Community College
📍 New Jersey, USA | 🎓 Graduating 2026
💼 Former CNC Programmer → Cybersecurity Analyst (in progress)

**Why this repository exists:**
I learn best by building real infrastructure. This homelab started as a simple Debian server and evolved into a production environment running DNS security (Pi-hole), workflow automation (N8N), and various self-hosted services. Every configuration, security hardening step, and experiment is documented here.

---

## 💡 About this Repository

This is where I bring together everything I've been working on — from Python scripts to server hardening and infrastructure documentation.
Each folder represents part of my learning process and the structure I use in my homelab to keep things organized, reproducible, and easy to maintain.

**The goal of this repo:**
→ Learn by doing with real infrastructure
→ Build tools and services that actually work
→ Keep my lab clean, documented, and evolving
→ Create a professional portfolio for cybersecurity career transition

---

## 🧩 Repository Structure

| Folder | Description | Status |
|--------|-------------|--------|
| [**CollegePythonScripts/**](CollegePythonScripts) | Collection of Python scripts from my academic journey (INF-103) — includes exercises, automations, and OOP projects with full documentation | ✅ Completed |
| [**server_setup/**](server_setup) | Configuration files, hardening reports, and documentation for my Debian-based home server — includes network setup, SSH security, Lynis audits, and systemd hardening | 🔄 In Progress |

---

## 🎯 What's Inside

### Server Infrastructure (server-lf1)
- **OS**: Debian 12 (Bookworm) - minimal install
- **Services Running**:
  - 🛡️ **Pi-hole** - Network-wide DNS ad-blocking (Port 53, 80)
  - ⚙️ **N8N** - Workflow automation platform (Port 5678)
  - 🐳 **Docker** - Container orchestration for self-hosted services
- **Security Hardening**:
  - SSH key-only authentication
  - Lynis security audits (ongoing score improvements)
  - systemd service hardening
  - Firewall configuration (UFW)

### Academic Projects
- **Python Fundamentals** (INF-103, Bergen Community College)
  - 16+ functional Python scripts
  - OOP project: Mobile phone management system
  - Caesar cipher, password generator, file manipulation
  - Well-documented with learning context

---

## ⚙️ Tech Stack

**Infrastructure:**
- Debian 12 Bookworm (minimal install)
- Docker + Docker Compose
- SSH (key-based authentication only)

**Security Tools:**
- Lynis (security auditing)
- systemd-analyze security
- UFW (firewall)

**Services:**
- Pi-hole (DNS ad-blocking)
- N8N (workflow automation)

**Development:**
- Python 3.11+
- Git (SSH authentication)
- Ubuntu 24.04 (development environment)

---

## 📊 Current Status

| Metric | Value |
|--------|-------|
| **Server Uptime** | Production (server-lf1) |
| **Security Score** | Improving (Lynis audits tracked) |
| **Services Running** | Pi-hole, N8N, Docker containers |
| **Active Development** | Ongoing hardening & documentation |

---

## 🎓 Learning Journey

This homelab documents my progression:

1. **✅ Python Fundamentals** (INF-103) — Basic scripting, OOP concepts
2. **🔄 Linux System Administration** — Debian server setup, SSH, systemd
3. **🔄 Security Hardening** — Server hardening, auditing, best practices
4. **📅 Network Security** (INF-165, Upcoming) — Firewalls, DNS, network segmentation

---

## ⚖️ License

All content here is shared under the **CC0-1.0 License (Public Domain)**.
You're free to explore, reuse, or modify anything for educational or personal purposes.

---

## 💬 Final Note

This homelab keeps growing as I learn new tools and technologies.
It's my personal documentation hub — a place to experiment, break things, fix them, and document the entire journey from student to cybersecurity professional.

**Last Updated:** November 2025
**Status:** Active learning project

---

**Questions or suggestions?** Feel free to open an issue or reach out!
