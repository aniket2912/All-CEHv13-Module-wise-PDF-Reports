# Enumeration

## 📌 Introduction
**Enumeration** is the process of actively connecting to a target system to gather detailed information such as usernames, machine names, network resources, shares, and services.  
It is a crucial step after scanning in the penetration testing lifecycle because it reveals system details that can be exploited in later stages.

---

## 🎯 Objectives of Enumeration
- Identify active network services and their versions.
- Gather usernames, groups, and domain information.
- List shared resources, files, and printers.
- Discover network topology and system architecture.
- Identify security misconfigurations.
- Collect data for potential exploitation.

---

## 🔍 Types of Enumeration
1. **NetBIOS Enumeration**
   - Gathers network shares, user lists, and system names.
2. **SNMP Enumeration**
   - Retrieves device details using Simple Network Management Protocol.
3. **LDAP Enumeration**
   - Extracts directory service information.
4. **NTP Enumeration**
   - Discovers network time protocol configurations and connected hosts.
5. **SMTP Enumeration**
   - Identifies valid email addresses and usernames.
6. **SMB Enumeration**
   - Lists shared files, printers, and services.
7. **DNS Enumeration**
   - Maps domain names to IP addresses, zone transfers.
8. **HTTP Enumeration**
   - Finds web directories, subdomains, and server details.

---

## 🛠️ Enumeration Methodology
1. **Port Scanning**
   - Identify open ports and available services.
2. **Service Fingerprinting**
   - Determine versions and configurations of services.
3. **Protocol-Specific Enumeration**
   - Use tools for NetBIOS, SNMP, SMB, etc.
4. **User and Group Enumeration**
   - Collect valid usernames for password attacks.
5. **Share Enumeration**
   - Identify accessible shared resources.
6. **Banner Grabbing**
   - Retrieve software details from services.
7. **Data Analysis**
   - Consolidate and filter results for exploitation.

---

## 🧰 Tools for Enumeration
- **Nmap** – Service version detection.
- **Enum4linux** – SMB and NetBIOS enumeration.
- **SMBclient** – Access SMB shares.
- **Net view** – List network resources (Windows).
- **SNMPwalk** – SNMP data gathering.
- **SMTP-user-enum** – SMTP username enumeration.
- **Dirbuster / Gobuster** – Web directory enumeration.
- **DNSenum / Fierce** – DNS enumeration.

---

## 🧪 Practical Enumeration Tasks
### **Task 1: NetBIOS Enumeration**
```bash
nbtstat -A <IP>
nmblookup -A <IP>
