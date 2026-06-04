# ThreatStrike Legion - Full Tool List

72 tools across 14 categories (57 offensive, 15 defensive), every one a real
form with the real flags exposed. Install any of them with one click from the
in-app Tool Status page.

---

## Red Team (57)

### Recon & OSINT (11)
- **subfinder** - Subdomain discovery
- **amass** - Attack-surface mapping
- **theHarvester** - Email and host OSINT
- **sherlock** - Username hunting across platforms
- **maigret** - Username profiling
- **holehe** - Email-account existence check
- **spiderfoot** - OSINT automation framework
- **recon-ng** - Modular recon framework
- **shodan** - Shodan search client
- **metagoofil** - Document metadata harvester
- **wafw00f** - WAF fingerprinting

### Web Recon (9)
- **httpx** - Fast HTTP probing
- **katana** - Web crawler
- **gau** - Historical URL fetch (getallurls)
- **ffuf** - Web fuzzer
- **feroxbuster** - Recursive content discovery
- **arjun** - HTTP parameter discovery
- **whatweb** - Web fingerprinting
- **wpscan** - WordPress vulnerability scanner
- **nikto** - Web server scanner

### Vuln Scanning (10)
- **nuclei** - Template-based vulnerability scanner
- **sqlmap** - SQL injection
- **dalfox** - XSS scanner
- **commix** - Command injection
- **corsy** - CORS misconfiguration scanner
- **wapiti** - Web app vulnerability scanner
- **jwt_tool** - Analyze, tamper, forge and crack JWTs
- **trivy** - CVE / misconfig / secret scanner
- **gitleaks** - Hardcoded-secret detection
- **searchsploit** - Exploit-DB search

### Network (6)
- **nmap** - Network and service scanner
- **rustscan** - Fast port scanner
- **masscan** - Mass port scanner
- **netdiscover** - ARP discovery (Linux only)
- **enum4linux** - SMB enumeration
- **smbmap** - SMB share enumeration

### Passwords (5)
- **hashcat** - GPU password cracking
- **john** - John the Ripper password cracking
- **hydra** - Online login brute force
- **cewl** - Wordlist generator from web content
- **crunch** - Wordlist builder

### Post Exploitation (4)
- **impacket** - Windows / AD attack suite
- **nxc / crackmapexec** - AD swiss-army knife (NetExec)
- **evil-winrm** - WinRM shell
- **smbclient** - SMB client

### Exploitation (1)
- **metasploit** - Exploitation framework (full GUI: module browser, workspace, host detail, sessions, console)

### Reverse Engineering (4)
- **ghidra** - NSA decompiler, headless auto-analysis
- **radare2** - Disassembler / binary analysis
- **jadx** - Android (APK/DEX) decompiler
- **apktool** - APK decode / rebuild

### Fuzzers (1)
- **gobuster** - Directory and DNS brute force

### Wireless (6)
- **aircrack-ng** - WPA/WPA2 PSK crack from capture
- **airodump-ng** - AP scan and handshake capture
- **hcxdumptool** - Modern PMKID and 4-way handshake capture
- **wifite** - Automated WPA/WPS cracking driver
- **bettercap** - Wi-Fi and BLE recon / MITM swiss-army
- **bluetoothctl** - Bluetooth scan and pair (Linux only)

---

## Blue Team (15)

### DFIR (3)
- **volatility3** - Memory forensics
- **sleuthkit** (fls) - Disk filesystem walk
- **log2timeline.py** (plaso) - Forensic timeline construction

### Threat Hunting (4)
- **yara** - Pattern matching
- **sigma-cli** - Detection-rule conversion
- **chainsaw** - Windows event-log hunt
- **hayabusa** - Windows event timeline

### Network Defense (3)
- **suricata** - IDS replay on pcap
- **zeek** - Protocol analyzer
- **tshark** - Command-line Wireshark

### Malware Analysis (5)
- **capa** - Capability detection
- **floss** - Deobfuscated string extraction
- **clamscan** - AV signature scan
- **ssdeep** - Fuzzy hashing
- **exiftool** - Metadata extraction

---

## Bundled wordlists

Six curated wordlists ship inside the app and appear in a dropdown right in the
tool forms (ffuf, gobuster, hashcat, john, hydra, and more):

- **web-common.txt** - Common web paths and files
- **web-raft-small.txt** - RAFT small web content
- **dns-subdomains-5000.txt** - Top 5,000 DNS subdomains
- **users-common.txt** - Common usernames
- **users-top-shortlist.txt** - Top usernames (shortlist)
- **pass-common.txt** - Common passwords

### Plus the full Kali wordlist set (one click)

The Tool Status page has a one-click **Kali Wordlists** download that pulls the entire SecLists collection (over **6,000 wordlists** covering web content, DNS, usernames, passwords, fuzzing, and more) plus **rockyou.txt** (about 14.3 million passwords), roughly 1 GB total. Once downloaded, every tool form and the AI agent can use them automatically.

---

**More coming soon. Email security@threatstrike.ai to request one.**
