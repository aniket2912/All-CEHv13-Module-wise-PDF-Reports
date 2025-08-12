# Scanning

## 📌 Introduction
**Scanning** is the second phase of ethical hacking, following reconnaissance.  
It involves actively interacting with the target network or system to identify live hosts, open ports, services, and vulnerabilities.  
The main purpose is to create a network map that will guide further enumeration and exploitation activities.

---

## 🎯 Objectives of Scanning
- Identify live hosts in a network.
- Discover open ports and running services.
- Detect operating systems and service versions.
- Map network topology.
- Identify potential vulnerabilities.
- Gather intelligence for enumeration and exploitation.

---

## 🔍 Types of Scanning
1. **Port Scanning**
   - Detects open and closed ports on a target system.
2. **Network Scanning**
   - Finds active hosts and devices on a network.
3. **Vulnerability Scanning**
   - Checks for known security flaws in services and systems.
4. **Service Version Detection**
   - Identifies specific versions of running services.
5. **OS Fingerprinting**
   - Determines the operating system of a target host.

---

## 🛠️ Scanning Methodology
1. **Preparation**
   - Define scope and permissions.
2. **Host Discovery**
   - Identify active systems (ping sweep, ARP scan).
3. **Port Scanning**
   - Use tools to check for open, closed, or filtered ports.
4. **Service Enumeration**
   - Identify the type and version of running services.
5. **Vulnerability Mapping**
   - Match detected services to known vulnerabilities.
6. **Reporting**
   - Document findings for further penetration testing.

---

## 🧰 Common Scanning Tools
- **Nmap** – Port scanning, OS detection, and service versioning.
- **Masscan** – High-speed port scanning.
- **Netcat** – Port scanning and banner grabbing.
- **Unicornscan** – Asynchronous network scanning.
- **Angry IP Scanner** – GUI-based network scanning.
- **Zenmap** – Nmap’s graphical interface.
- **Nessus/OpenVAS** – Vulnerability scanning.

---

## 📊 Types of Nmap Scans
- **TCP Connect Scan** (`-sT`) – Full TCP connection.
- **SYN Scan** (`-sS`) – Stealth scan without completing handshake.
- **UDP Scan** (`-sU`) – Checks UDP ports.
- **Service Version Detection** (`-sV`) – Detects application versions.
- **OS Detection** (`-O`) – Identifies operating system.
- **Aggressive Scan** (`-A`) – Enables OS detection, version detection, scripts, and traceroute.

---

## 🧪 Practical Scanning Labs

### **Lab 1: Discover Live Hosts**
```bash
nmap -sn 192.168.1.0/24
