# Sniffing

## 📌 Introduction
**Sniffing** is the process of monitoring and capturing network traffic to analyze data packets transmitted over a network.  
Attackers use sniffing to intercept sensitive information such as **usernames, passwords, credit card details, and confidential communications**.

---

## 🎯 Objectives of Sniffing
- Understand how sniffing works in wired and wireless environments.
- Learn different sniffing techniques used by attackers.
- Identify tools and methods used for packet capture.
- Detect and prevent sniffing attempts.
- Perform ethical sniffing in a controlled lab environment.

---

## ⚙️ Types of Sniffing
1. **Passive Sniffing**
   - Capturing data without altering the network traffic.
   - Usually done on a hub or in wireless mode.
2. **Active Sniffing**
   - Actively injecting traffic to redirect packets to the attacker.
   - Used in switched network environments.

---

## 🔍 Common Sniffing Techniques
- **ARP Poisoning** – Manipulating ARP tables to intercept packets.
- **MAC Flooding** – Overloading the switch MAC table to force it into hub mode.
- **DNS Spoofing** – Redirecting traffic to malicious servers.
- **MITM (Man-in-the-Middle)** – Intercepting communication between two parties.
- **DHCP Spoofing** – Providing malicious IP configurations to clients.

---

## 🧪 Hands-on Labs
### **Lab 1: Passive Packet Capture**
- Use Wireshark to capture network traffic in promiscuous mode.

### **Lab 2: ARP Poisoning**
- Use Ettercap to perform ARP spoofing and capture credentials.

### **Lab 3: Sniffing FTP & Telnet Traffic**
- Capture unencrypted FTP and Telnet usernames/passwords using Wireshark.

### **Lab 4: HTTPS Traffic Capture**
- Attempt to capture and analyze HTTPS traffic (requires MITM setup with SSL stripping in a legal lab environment).

---

## 🛡️ Prevention & Mitigation
- Use **encrypted protocols** (HTTPS, SSH, SFTP) instead of plaintext.
- Implement **switch port security** to prevent MAC flooding.
- Enable **dynamic ARP inspection** on switches.
- Use **VPN** to encrypt all network traffic.
- Monitor the network for unusual ARP or MAC address changes.

---

## 🧰 Tools for Sniffing
- **Wireshark** – Network packet analysis.
- **Tcpdump** – Command-line packet capture.
- **Ettercap** – MITM and sniffing.
- **dsniff** – Sniffing suite for capturing passwords.
- **Cain & Abel** – Password recovery and sniffing (Windows).

---

## 📄 Reporting & Documentation
When documenting sniffing activities:
- Mention the sniffing type (passive or active).
- Include tools used and packet capture results.
- Highlight any credentials or sensitive information captured.
- Provide recommendations for securing the network.

---

## ⚠️ Disclaimer
This repository is for **educational and authorized penetration testing only**.  
Sniffing without permission is **illegal** and can lead to severe consequences under cybercrime laws.
