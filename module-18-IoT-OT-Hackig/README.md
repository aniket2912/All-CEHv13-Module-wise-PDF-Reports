# IoT and OT Hacking

## 📌 Introduction
**IoT (Internet of Things) and OT (Operational Technology) hacking** involves discovering, analyzing, and exploiting vulnerabilities in connected devices, industrial control systems, and critical infrastructure.  
IoT devices include smart home gadgets, cameras, sensors, and wearables, while OT focuses on industrial systems like SCADA, PLCs, and ICS. Both environments are often poorly secured, making them attractive attack targets.

---

## 🎯 Objectives
- Understand IoT and OT architectures.
- Identify vulnerabilities in IoT devices and protocols.
- Analyze firmware and communication channels.
- Perform exploitation of insecure configurations and weak authentication.
- Assess industrial control systems (ICS/SCADA) for risks.
- Provide remediation to secure IoT/OT ecosystems.

---

## 🔍 Key Attack Vectors
- **Weak Authentication** – Default credentials, hardcoded passwords.
- **Insecure Protocols** – MQTT, CoAP, Modbus, DNP3 without encryption.
- **Firmware Exploits** – Reverse engineering firmware for backdoors.
- **Insecure APIs** – Poorly secured endpoints leaking sensitive data.
- **Unpatched Vulnerabilities** – Outdated firmware or OS.
- **Physical Access** – Serial, JTAG, UART interfaces.
- **Supply Chain Attacks** – Compromised components before deployment.

---

## 🛠️ Methodology
1. **Information Gathering**
   - Identify IoT/OT devices, network maps, firmware versions.
2. **Reconnaissance**
   - Discover open ports, protocols, and services.
3. **Vulnerability Assessment**
   - Scan for weak passwords, outdated firmware, misconfigurations.
4. **Exploitation**
   - Exploit insecure services, intercept traffic, reverse firmware.
5. **Post-Exploitation**
   - Extract sensitive data, escalate privileges, pivot to networks.
6. **Reporting**
   - Document vulnerabilities with remediation guidelines.

---

## ⚙️ Common Tools
- **Nmap** – Network discovery and port scanning.
- **Shodan/Censys** – IoT device search engines.
- **Burp Suite** – IoT API testing.
- **Wireshark** – Protocol analysis (MQTT, CoAP, Modbus, etc.).
- **Binwalk** – Firmware analysis and extraction.
- **Ghidra / IDA Pro** – Reverse engineering firmware binaries.
- **MQTT Explorer** – Inspect MQTT traffic.
- **Metasploit Framework** – Exploit known IoT vulnerabilities.
- **PLCScan** – ICS/SCADA system discovery.

---

## 📜 Useful Commands
- **Scan for IoT Devices in a Network**

      nmap -p 80,443,1883,5683,502,20000 --open <target-range>
  
- **Extract Firmware**

      binwalk -e firmware.bin

- **Check MQTT Broker (Unauthenticated)**

      mosquitto_sub -h <IP> -t '#' -v

- **Analyze Modbus Traffic with Wireshark Filter**

      modbus

- **Shodan Search Example**

      org:"<Company>" port:502

---

## 📊 Indicators of Compromise (IoCs)
- Unauthorized device connections.
- Unexpected control commands in ICS/SCADA.
- Unusual traffic patterns in IoT protocols.
- Firmware integrity mismatches.
- Devices operating outside normal schedules.

---

## 🛡️ Defensive Countermeasures
- Change default credentials and enforce strong authentication.
- Regularly update firmware and patch vulnerabilities.
- Segment IoT/OT networks from corporate IT networks.
- Use VPNs and TLS for IoT communications.
- Implement strict access control policies for OT environments.
- Monitor with IDS/IPS solutions tuned for ICS/IoT traffic.
- Conduct regular penetration testing and risk assessments.

---

## 📄 Reporting
When documenting IoT/OT hacking:
- Include network topology and device inventory.
- List vulnerabilities with CVSS severity ratings.
- Provide proof-of-concept evidence.
- Recommend patching, segmentation, and security monitoring solutions.

---

## ⚠️ Disclaimer
This repository is for **educational and authorized testing only**.  
Hacking IoT/OT devices without permission is **illegal** and may disrupt critical infrastructure. Always test in authorized labs or with explicit approval.
