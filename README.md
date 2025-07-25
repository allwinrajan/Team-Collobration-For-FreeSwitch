Here’s your **Day 1 README.md** in one **single copyable Markdown block**:

---

````markdown
# FreeSWITCH Learning – Day 1 🚀

Welcome to **Day 1** of learning **FreeSWITCH**, an open-source telephony platform designed to route and interconnect communication protocols. This repository will track my learning journey, practical exercises, and resources.

---

## ✅ What is FreeSWITCH?

FreeSWITCH is an **open-source telephony platform** that enables:
- VoIP solutions (SIP, RTP, WebRTC)
- PBX systems
- IVR (Interactive Voice Response)
- Conference bridges
- Gateway services between VoIP and PSTN

---

## 📌 Objectives for Day 1
- Understand what FreeSWITCH is and why it’s used
- Install FreeSWITCH on my system (Linux recommended)
- Explore basic configuration files
- Verify installation by starting the FreeSWITCH CLI

---

## 🛠 Prerequisites
- **OS:** Ubuntu/Debian preferred
- **Packages:** `git`, `wget`, `curl`, `build-essential`
- Basic knowledge of **Linux commands**

---

## 📥 Installation Steps

### 1. Update System
```bash
sudo apt update && sudo apt upgrade -y
````

### 2. Install Dependencies

```bash
sudo apt install -y git wget curl gnupg2 lsb-release
```

### 3. Install FreeSWITCH

```bash
sudo apt install -y freeswitch freeswitch-mod-conference freeswitch-lang-en
```

### 4. Start FreeSWITCH

```bash
sudo systemctl start freeswitch
sudo fs_cli
```

✅ If you see the FreeSWITCH CLI, you are ready!

---

## 🔍 Explore

* Configuration folder: `/etc/freeswitch/`
* Main config: `freeswitch.xml`
* SIP profiles: `/etc/freeswitch/sip_profiles/`

---

## 📚 Resources

* [Official FreeSWITCH Docs](https://freeswitch.com/confluence/)
* [FreeSWITCH GitHub](https://github.com/signalwire/freeswitch)

---

## ✅ Day 1 Summary

✔ Installed FreeSWITCH
✔ Explored basic configs
✔ Connected to FreeSWITCH CLI

---

**Next Step (Day 2):** Learn about SIP profiles and creating a simple dialplan.

---

👉 *Follow this repo for daily updates on my FreeSWITCH learning journey!*

```

---

✅ Copy this entire block and save it as **`README.md`** in your Day 1 folder.  

---

Do you want me to **prepare Day 2 README right now** or **create a 7-day complete roadmap README for the master repo**?
```
