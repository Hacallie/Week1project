# 🔐 Cybersecurity Lab Environment Setup

### Networkwalks Cybersecurity Internship — Week 01

Building an isolated virtual laboratory using VirtualBox and Kali Linux for cybersecurity learning and authorized security testing.

---

## 📌 Project Overview

As part of my Week 01 cybersecurity internship work, I built and configured a virtual cybersecurity laboratory using Oracle VirtualBox and Kali Linux.

The purpose of the lab is to provide a controlled environment where I can safely practice cybersecurity concepts, networking, reconnaissance, security tools, and vulnerability assessment without targeting unauthorized systems.

The lab is designed so that additional virtual machines can be added later as targets for authorized security testing.

---

## 🎯 Objectives

The main objectives of this project were to:

- Install and configure Oracle VirtualBox.
- Import and configure Kali Linux.
- Create a dedicated NAT Network.
- Connect Kali Linux to the isolated lab network.
- Verify network connectivity.
- Verify DNS resolution.
- Verify cybersecurity tools such as Nmap.
- Create a clean VM snapshot for recovery.
- Document the setup and troubleshooting process.
- Prepare the environment for future cybersecurity labs.

---

## 🛡️ Purpose of the Lab

This laboratory is intended for cybersecurity education and authorized security testing.

Future exercises may include:

- Network reconnaissance
- Port scanning
- Vulnerability assessment
- Packet analysis
- Web security testing
- Security-tool experimentation
- Controlled exploitation practice

> ⚠️ **Ethical Use:** This laboratory and its tools will only be used against systems that I own or have explicit authorization to test.

---

## 🏗️ Lab Architecture

```text
                    Internet
                       │
                       ▼
                 ┌─────────────┐
                 │   Windows   │
                 │ Host Machine│
                 └──────┬──────┘
                        │
                 ┌──────▼──────┐
                 │  VirtualBox │
                 └──────┬──────┘
                        │
                 ┌──────▼──────────┐
                 │  CyberLab-NAT   │
                 │   10.0.0.0/24   │
                 └──────┬──────────┘
                        │
                 ┌──────▼──────┐
                 │ Kali Linux  │
                 │ 2026.2      │
                 └─────────────┘

        Future target VMs can be added
        to the same virtual network.
