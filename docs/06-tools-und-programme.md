# Tools, Apps & Programme 🛠️

Eine umfassende Übersicht aller notwendigen und hilfreichen Tools für deine C|PENT Vorbereitung und Praxis.

## 🖥️ Basis-Setup

### Virtualisierung

#### VirtualBox (Empfohlen für Anfänger)
- **Kosten**: Kostenlos
- **OS**: Windows, macOS, Linux
- **Download**: [virtualbox.org](https://www.virtualbox.org)

**Vorteile:**
- ✅ Komplett kostenlos
- ✅ Einfache Bedienung
- ✅ Gute Community-Support
- ✅ Snapshots

**Nachteile:**
- ⚠️ Performance nicht optimal
- ⚠️ Weniger Features als VMware

---

#### VMware Workstation/Fusion
- **Kosten**: ~$200 (Player kostenlos)
- **OS**: Windows, Linux (Workstation) / macOS (Fusion)
- **Download**: [vmware.com](https://www.vmware.com)

**Vorteile:**
- ✅ Bessere Performance
- ✅ Mehr Features
- ✅ Professional Grade
- ✅ Bessere Netzwerk-Optionen

**Nachteile:**
- ⚠️ Kostenpflichtig (außer Player)
- ⚠️ Komplexer für Anfänger

---

#### UTM (für Apple Silicon Macs)
- **Kosten**: Kostenlos
- **OS**: macOS (ARM)
- **Download**: [mac.getutm.app](https://mac.getutm.app)

**Für M1/M2/M3 Macs:**
- ✅ Native ARM Unterstützung
- ✅ Kostenlos
- ✅ Kali ARM-Version läuft gut

---

### Betriebssysteme

#### Kali Linux (Hauptsystem)
- **Download**: [kali.org](https://www.kali.org)
- **Empfehlung**: ⭐⭐⭐⭐⭐

**Versionen:**
- **Kali VM** - Vorkonfiguriert, einfach
- **Kali Installer** - Custom Installation
- **Kali on WSL2** - Für Windows-User
- **Kali ARM** - Für Apple Silicon

**Vorinstallierte Tools**: 600+

---

#### Parrot OS (Alternative)
- **Download**: [parrotsec.org](https://www.parrotsec.org)
- **Empfehlung**: ⭐⭐⭐⭐

**Unterschiede zu Kali:**
- Leichtgewichtiger
- Anderes Tool-Set
- Privacy-fokussiert

---

#### Windows 10/11 VM
- **Download**: [microsoft.com/evalcenter](https://www.microsoft.com/en-us/evalcenter/)
- **Kosten**: 90-Tage Trial kostenlos

**Warum benötigt?**
- Windows-spezifische Tools
- Active Directory Testing
- PowerShell Development
- Target für Exploitation

---

#### Ubuntu/Debian Server
- **Download**: [ubuntu.com](https://ubuntu.com)
- **Kosten**: Kostenlos

**Verwendung:**
- Custom Lab-Umgebungen
- Vulnerable VMs
- Service Testing

---

## 🔍 Reconnaissance & OSINT

### Information Gathering

| Tool | Beschreibung | Kosten | In Kali? |
|------|--------------|--------|----------|
| **Nmap** | Port Scanner | Kostenlos | ✅ |
| **Masscan** | Fast Port Scanner | Kostenlos | ✅ |
| **Rustscan** | Ultra-fast Scanner | Kostenlos | ⚠️ |
| **theHarvester** | Email/Subdomain Harvester | Kostenlos | ✅ |
| **Recon-ng** | Recon Framework | Kostenlos | ✅ |
| **Maltego** | OSINT Tool | Freemium | ✅ |
| **Shodan** | Internet Scanner | Freemium | - |
| **Amass** | Subdomain Enumeration | Kostenlos | ✅ |
| **Subfinder** | Subdomain Finder | Kostenlos | ⚠️ |

### DNS Enumeration
- **DNSRecon** (Kali ✅)
- **Fierce** (Kali ✅)
- **DNSenum** (Kali ✅)
- **DNSdumpster** (Web)

---

## 🌐 Web Application Testing

### Proxy & Interception

#### Burp Suite
- **Version**: Community (Free) / Professional ($449/Jahr)
- **Download**: [portswigger.net](https://portswigger.net)
- **Empfehlung**: ⭐⭐⭐⭐⭐

**Community Features:**
- Proxy
- Repeater
- Decoder
- Comparer
- Sequencer (Limited)

**Professional zusätzlich:**
- Scanner
- Intruder (unbegrenzt)
- Collaborator
- Extensions

**Muss ich Professional kaufen?**
- Für C|PENT: **Nein**
- Community reicht für Vorbereitung
- Manual Testing im Fokus

---

#### OWASP ZAP
- **Kosten**: Komplett kostenlos
- **Download**: [zaproxy.org](https://www.zaproxy.org)
- **Empfehlung**: ⭐⭐⭐⭐

**Features:**
- Automated Scanner
- Proxy
- Spider
- Fuzzer
- Open Source Alternative zu Burp Pro

---

### Web Scanners & Enumeration

| Tool | Zweck | Kosten | In Kali? |
|------|-------|--------|----------|
| **Nikto** | Web Server Scanner | Kostenlos | ✅ |
| **Dirb/Dirbuster** | Directory Bruteforce | Kostenlos | ✅ |
| **Gobuster** | Fast Directory/DNS Bruteforce | Kostenlos | ✅ |
| **Ffuf** | Fast Fuzzer | Kostenlos | ✅ |
| **Wfuzz** | Web Fuzzer | Kostenlos | ✅ |
| **WPScan** | WordPress Scanner | Kostenlos | ✅ |
| **Nuclei** | Vulnerability Scanner | Kostenlos | ⚠️ |

### Exploitation Tools

| Tool | Zweck | Kosten |
|------|-------|--------|
| **SQLMap** | SQL Injection | Kostenlos ✅ |
| **Commix** | Command Injection | Kostenlos ✅ |
| **XSStrike** | XSS Scanner | Kostenlos ⚠️ |
| **NoSQLMap** | NoSQL Injection | Kostenlos ⚠️ |

---

## 💥 Exploitation Frameworks

### Metasploit Framework
- **Version**: Community (Free) / Pro (Paid)
- **Included**: In Kali Linux
- **Empfehlung**: ⭐⭐⭐⭐⭐

**Must-Know für C|PENT!**

**Komponenten:**
- msfconsole
- msfvenom (Payload Generator)
- meterpreter
- Exploit Modules
- Post-Exploitation Modules

---

### Other Frameworks

| Framework | Beschreibung | Kosten |
|-----------|--------------|--------|
| **Empire/Starkiller** | PowerShell Post-Exploitation | Kostenlos |
| **Covenant** | .NET C2 Framework | Kostenlos |
| **PoshC2** | C2 Framework | Kostenlos |
| **Cobalt Strike** | Commercial C2 | $$$$ |

**Hinweis**: Cobalt Strike nicht notwendig für C|PENT

---

## 🔐 Password Cracking

### Hash Cracking

| Tool | Typ | Geschwindigkeit | GPU Support |
|------|-----|-----------------|-------------|
| **Hashcat** | Advanced | Sehr schnell | ✅ |
| **John the Ripper** | Traditional | Mittel | Jumbo: ✅ |
| **Hydra** | Online Bruteforce | Mittel | ❌ |
| **Medusa** | Online Bruteforce | Mittel | ❌ |
| **CrackMapExec** | Network Auth | - | ❌ |

### Wordlists

**Vorinstalliert in Kali:**
- `/usr/share/wordlists/rockyou.txt` ⭐
- `/usr/share/wordlists/dirb/`
- `/usr/share/wordlists/dirbuster/`
- `/usr/share/wordlists/metasploit/`

**Zusätzlich empfohlen:**
- **SecLists** - [GitHub](https://github.com/danielmiessler/SecLists)
  ```bash
  git clone https://github.com/danielmiessler/SecLists.git
  ```

---

## 🔄 Post-Exploitation

### Privilege Escalation

| Tool | OS | Zweck |
|------|-----|-------|
| **LinPEAS** | Linux | Automated Enumeration |
| **WinPEAS** | Windows | Automated Enumeration |
| **Linux Exploit Suggester** | Linux | Kernel Exploit Finder |
| **Windows Exploit Suggester** | Windows | Patch Level Check |
| **GTFOBins** | Linux | Binary Exploitation Reference |
| **LOLBAS** | Windows | Living Off The Land |

### Persistence & Lateral Movement

| Tool | Beschreibung |
|------|--------------|
| **Mimikatz** | Windows Credential Dumping |
| **BloodHound** | AD Attack Path Analysis |
| **Impacket** | Network Protocol Scripts |
| **CrackMapExec** | Swiss Army Knife für AD |
| **Evil-WinRM** | WinRM Exploitation |

---

## 📡 Wireless & Network

### Wireless Tools

| Tool | Zweck | In Kali? |
|------|-------|----------|
| **Aircrack-ng Suite** | WiFi Cracking | ✅ |
| **Wifite** | Automated Wireless Attacks | ✅ |
| **Reaver** | WPS Cracking | ✅ |
| **Bully** | WPS Bruteforce | ✅ |
| **Kismet** | Wireless Detector | ✅ |
| **Fern Wifi Cracker** | GUI WiFi Tool | ⚠️ |

**Hardware benötigt:**
- WiFi Adapter mit Monitor Mode
- Empfehlung: Alfa AWUS036ACH (~€40)

---

### Network Analysis

| Tool | Beschreibung |
|------|--------------|
| **Wireshark** | Packet Analyzer |
| **tcpdump** | CLI Packet Capture |
| **Ngrep** | Network Grep |
| **Netcat** | Swiss Army Knife |
| **Socat** | Enhanced Netcat |

---

## 🐳 Container & Cloud

### Container Security

| Tool | Zweck |
|------|-------|
| **Docker** | Container Platform |
| **Kubectl** | Kubernetes CLI |
| **Trivy** | Container Vulnerability Scanner |
| **Hadolint** | Dockerfile Linter |

### Cloud Tools

| Tool | Cloud Provider |
|------|----------------|
| **AWS CLI** | Amazon Web Services |
| **Azure CLI** | Microsoft Azure |
| **gcloud** | Google Cloud Platform |
| **ScoutSuite** | Multi-Cloud Audit |
| **Prowler** | AWS Security Assessment |

---

## 📝 Documentation & Reporting

### Note-Taking Apps

#### Cherry Tree (Empfohlen)
- **Kosten**: Kostenlos
- **OS**: Windows, macOS, Linux
- **Features**: Hierarchical notes, Syntax highlighting
- **Empfehlung**: ⭐⭐⭐⭐⭐

---

#### Obsidian
- **Kosten**: Kostenlos (Sync kostenpflichtig)
- **OS**: Windows, macOS, Linux, Mobile
- **Features**: Markdown, Graph view, Plugins
- **Empfehlung**: ⭐⭐⭐⭐⭐

---

#### Joplin
- **Kosten**: Kostenlos + Open Source
- **OS**: Cross-Platform
- **Features**: Markdown, Sync, E2E Encryption
- **Empfehlung**: ⭐⭐⭐⭐

---

#### OneNote
- **Kosten**: Kostenlos (mit Microsoft Account)
- **OS**: Cross-Platform
- **Features**: Rich editing, Cloud sync
- **Empfehlung**: ⭐⭐⭐

---

### Screenshot & Recording

| Tool | Zweck | OS |
|------|-------|----|
| **Flameshot** | Screenshots | Linux |
| **Greenshot** | Screenshots | Windows |
| **Sharex** | Screenshots + Recording | Windows |
| **Peek** | GIF Recording | Linux |
| **OBS Studio** | Screen Recording | All |
| **Asciinema** | Terminal Recording | Linux/macOS |

---

### Report Templates

**Wo finden?**
- **GitHub**: "pentest report template"
- **TCM Security**: Free Report Template
- **Offensive Security**: OSCP Report Template (adaptierbar)

**Tools für Reports:**
- **Microsoft Word** / **LibreOffice Writer**
- **LaTeX** (für Professional Look)
- **Markdown → PDF** (Pandoc)

---

## 🔧 Development & Scripting

### Code Editors

| Editor | Beschreibung | Kosten |
|--------|--------------|--------|
| **VS Code** | Modern, extensible | Kostenlos |
| **Sublime Text** | Fast, lightweight | Freemium |
| **Vim/Neovim** | Terminal-based | Kostenlos |
| **PyCharm Community** | Python IDE | Kostenlos |

**Empfohlene VS Code Extensions:**
- Python
- Markdown All in One
- GitLens
- Remote - SSH

---

### Programming Languages

**Must-Know:**
- **Python** ⭐⭐⭐⭐⭐
  - Exploitation Scripts
  - Automation
  - Tool Development

- **Bash** ⭐⭐⭐⭐⭐
  - System Administration
  - Automation
  - Quick Scripts

- **PowerShell** ⭐⭐⭐⭐
  - Windows Post-Exploitation
  - AD Enumeration
  - Automation

**Nice-to-Have:**
- **JavaScript** (für Web)
- **Go** (für Tool Development)
- **Ruby** (Metasploit)

---

## 🗄️ Database Clients

| Client | Datenbank | GUI? |
|--------|-----------|------|
| **DBeaver** | Multi-DB | ✅ |
| **MySQL Workbench** | MySQL | ✅ |
| **pgAdmin** | PostgreSQL | ✅ |
| **mongosh** | MongoDB | ❌ |
| **redis-cli** | Redis | ❌ |

---

## 📦 Package Managers & Repos

### Linux (Kali/Debian)
```bash
apt update && apt upgrade
apt install <package>
```

### Python
```bash
pip3 install <package>
pipx install <tool>  # Isolated environments
```

### Go Tools
```bash
go install github.com/user/tool@latest
```

### GitHub Tools
```bash
git clone https://github.com/user/repo
cd repo
./install.sh  # or pip install -r requirements.txt
```

---

## 🌐 Browser Extensions

### Für Pentesting

| Extension | Zweck | Browser |
|-----------|-------|---------|
| **FoxyProxy** | Proxy Switching | Firefox, Chrome |
| **Wappalyzer** | Tech Stack Detection | Firefox, Chrome |
| **Cookie-Editor** | Cookie Management | Firefox, Chrome |
| **HackBar** | Web Testing | Firefox |
| **Retire.js** | JS Library Vulnerability | Firefox, Chrome |

**Empfohlener Browser**: Firefox Developer Edition

---

## 📱 Mobile Apps

### Android (Hilfreich)

| App | Zweck |
|-----|-------|
| **Termux** | Linux Terminal auf Android |
| **NetHunter** | Kali auf Android |
| **Fing** | Network Scanner |
| **WiFi Analyzer** | WiFi Analysis |

### iOS

| App | Zweck |
|-----|-------|
| **iSH** | Linux Shell |
| **Fing** | Network Scanner |
| **Prompt** | SSH Client |

---

## 💾 Storage & Backup

### Cloud Storage (für Notizen)
- **NextCloud** (Self-hosted, empfohlen)
- **Google Drive** (15 GB kostenlos)
- **Dropbox** (2 GB kostenlos)
- **OneDrive** (5 GB kostenlos)

**Wichtig**: Niemals sensitive Pentest-Daten in Public Cloud!

### Backup Solutions
- **Timeshift** (Linux)
- **rsync** (CLI)
- **Duplicati** (Cross-platform)
- **Borg Backup** (Deduplicated)

---

## 🎮 Practice Platforms (Apps/Websites)

| Platform | App? | Kosten |
|----------|------|--------|
| **HackTheBox** | ✅ Mobile App | Freemium |
| **TryHackMe** | ✅ Mobile App | Freemium |
| **PentesterLab** | ❌ | Freemium |
| **VulnHub** | ❌ | Kostenlos |

---

## 🛡️ Defensive Tools (Hilfreich)

| Tool | Zweck |
|------|-------|
| **Fail2Ban** | Intrusion Prevention |
| **Snort** | IDS/IPS |
| **OSSEC** | HIDS |
| **Wazuh** | Security Monitoring |

**Warum als Pentester wichtig?**
- Verstehe die andere Seite
- Evasion-Techniken
- Report Recommendations

---

## 📊 Monitoring & Organization

### Time Tracking
- **Toggl Track** - Time tracking
- **RescueTime** - Automatic tracking
- **Clockify** - Free time tracking

### Task Management
- **Notion** - All-in-one workspace
- **Trello** - Kanban boards
- **Todoist** - To-do lists
- **Obsidian** - Knowledge base + Tasks

---

## 🎯 Essential Toolkit (Minimum Setup)

Wenn du nur das Nötigste willst:

### Software
1. **VirtualBox** - Virtualisierung
2. **Kali Linux** - Main OS
3. **Windows VM** - Testing target
4. **Burp Suite Community** - Web testing
5. **Cherry Tree** / **Obsidian** - Notes

### Tools (alle in Kali inkludiert)
1. **Nmap** - Scanning
2. **Metasploit** - Exploitation
3. **SQLMap** - SQL Injection
4. **Hashcat** - Password Cracking
5. **Gobuster** - Directory Enumeration

**Kosten**: €0 🎉

---

## 💰 Premium Tools (Optional)

Falls Budget vorhanden:

| Tool | Kosten/Jahr | Lohnt sich? |
|------|-------------|-------------|
| **Burp Suite Pro** | $449 | ⚠️ Nur wenn du viele Web Apps testest |
| **HTB VIP** | $12-15/Monat | ✅ Sehr empfohlen! |
| **IDA Pro** | $$$$ | ❌ Nicht für C\|PENT nötig |
| **Cobalt Strike** | $$$$ | ❌ Nicht nötig |

---

## 🔄 Tool Updates

**Wichtig**: Tools regelmäßig updaten!

```bash
# Kali System Update
sudo apt update && sudo apt upgrade -y

# Tool-spezifische Updates
cd /opt/tool-name
git pull

# Python Tools
pip3 list --outdated
pip3 install --upgrade <package>
```

**Empfehlung**: Wöchentlich updaten

---

## 🎓 Learning Tools

### Flashcards & Spaced Repetition
- **Anki** - Flashcard App (Cross-platform)
  - Erstelle Decks für:
    - Commands
    - Exploit-Techniken
    - Port Numbers
    - CVE Details

### Mind Mapping
- **XMind** - Mind mapping
- **Obsidian** (mit Graph View)
- **Draw.io** - Diagramme

---

## 📖 Zusammenfassung: Dein Setup

### Tag 1: Basis-Setup
1. VirtualBox installieren
2. Kali Linux VM erstellen
3. Updates durchführen
4. Snapshots erstellen

### Tag 2: Essential Tools
1. Burp Suite installieren
2. Cherry Tree / Obsidian einrichten
3. SecLists clonen
4. Browser Extensions installieren

### Tag 3: Practice Environment
1. Windows VM aufsetzen
2. Vulnerable VMs herunterladen (VulnHub)
3. HTB Account erstellen
4. TryHackMe Account erstellen

### Danach: Continuously
- Tools nach Bedarf installieren
- Nicht alles auf einmal!
- Lerne ein Tool richtig, bevor du das nächste installierst

---

**💡 Tipp**: Du brauchst nicht alle Tools! Starte mit den Basics und erweitere nach Bedarf. Beherrsche wenige Tools gut, statt viele Tools schlecht!

---

[← Zurück zu Wochenplänen](05-wochenplaene.md) | [Weiter zu AuDHD Lernstrategien →](07-audhd-lernstrategien.md)
