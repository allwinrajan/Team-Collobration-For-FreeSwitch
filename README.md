# FreeSWITCH Learning – Day 1

This repository documents my journey in learning FreeSWITCH, an open-source telephony platform. Each day, I will add new notes, configurations, and examples.

---

## What is FreeSWITCH?

FreeSWITCH is an open-source telephony platform that supports:

- VoIP solutions (SIP, RTP, WebRTC)
- PBX systems
- IVR (Interactive Voice Response)
- Conference bridges
- Gateway services between VoIP and PSTN

---

## Day 1 Objectives

- Understand the purpose and features of FreeSWITCH
- Install FreeSWITCH on a Linux system (Ubuntu/Debian recommended)
- Explore the basic configuration files
- Verify installation by starting the FreeSWITCH CLI

---

## Prerequisites

- **Operating System:** Ubuntu/Debian preferred
- **Required Packages:** `git`, `wget`, `curl`, `build-essential`
- Basic knowledge of Linux commands

---

## Installation Steps

### 1. Update System
```bash
sudo apt update && sudo apt upgrade -y

### 2. Install Dependencies

```bash
sudo apt install -y git wget curl gnupg2 lsb-release

3. Install FreeSWITCH

```bash
sudo apt install -y freeswitch freeswitch-mod-conference freeswitch-lang-en
4. Start FreeSWITCH

```bash
sudo systemctl start freeswitch
sudo fs_cli

If you see the FreeSWITCH CLI prompt, the installation was successful.

Explore Key Directories
Configuration folder: /etc/freeswitch/

Main configuration file: freeswitch.xml

SIP profiles: /etc/freeswitch/sip_profiles/

Resources
Official FreeSWITCH Documentation

FreeSWITCH GitHub Repository

Day 1 Summary
Installed FreeSWITCH

Explored configuration files

Connected to FreeSWITCH CLI


Day 2 continue by Alvin from B

