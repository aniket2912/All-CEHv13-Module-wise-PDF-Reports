# 🔥 Firewall, IDS, and IPS – Module Notes

## 📌 Introduction
Firewalls, Intrusion Detection Systems (IDS), and Intrusion Prevention Systems (IPS) are essential components in network security.  

- **Firewall**: Controls incoming and outgoing network traffic based on predetermined rules.  
- **IDS**: Monitors network/system activities for malicious actions and policy violations.  
- **IPS**: Detects and actively prevents identified threats in real-time.  

---

## 🎯 Objectives
- Understand the role of firewalls, IDS, and IPS in cybersecurity.
- Learn the differences between IDS and IPS.
- Explore firewall types, architectures, and deployment methods.
- Perform practical exercises to analyze, detect, and prevent attacks.

---

## 🛡️ Firewall

### Types of Firewalls
1. **Packet-Filtering Firewall**
2. **Stateful Inspection Firewall**
3. **Proxy Firewall**
4. **Next-Generation Firewall (NGFW)**

### Firewall Architectures
- Bastion Host
- Screened Subnet (DMZ)
- Dual-Homed Host

**Architecture Diagram:**
![Firewall Architecture](https://i.ibb.co/NZy38Cm/firewall-architecture.png)

### Example Commands
```bash
# View firewall rules (Linux - iptables)
sudo iptables -L

# View firewall rules (Windows)
netsh advfirewall firewall show rule name=all

👁️ IDS (Intrusion Detection System)
Types of IDS
NIDS: Network-based IDS

HIDS: Host-based IDS

Detection Methods
Signature-Based Detection

Anomaly-Based Detection

Hybrid Detection

IDS Workflow Diagram:

Example Tool – Snort
# Run Snort in packet capture mode
snort -i eth0 -A console


🛑 IPS (Intrusion Prevention System)
Functions
Detect and block malicious traffic.

Automatically update rule sets.

Prevent known attack signatures.

IPS Workflow Diagram:

Example Tool – Suricata
# Run Suricata in IPS mode
suricata -c /etc/suricata/suricata.yaml -i eth0

🧪 Hands-On Labs
Lab 1 – Configure Linux Firewall (iptables)
# Block incoming traffic from an IP
sudo iptables -A INPUT -s 192.168.1.100 -j DROP

Lab 2 – Detect Suspicious Traffic with Snort
snort -i eth0 -A console -c /etc/snort/snort.conf

Lab 3 – Prevent Attack with Suricata
suricata -c /etc/suricata/suricata.yaml -q 0 -i eth0
