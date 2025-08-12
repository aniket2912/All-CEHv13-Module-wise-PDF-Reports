# DoS & DDoS Attacks

## 📌 Introduction
**Denial of Service (DoS)** and **Distributed Denial of Service (DDoS)** are cyberattacks designed to make a network service, server, or application unavailable to its intended users.  
- **DoS Attack**: A single system sends a flood of requests to overload the target.  
- **DDoS Attack**: Multiple compromised systems (botnet) send traffic simultaneously to exhaust resources.

---

## 🎯 Objectives of DoS/DDoS Attacks
- Understand how DoS and DDoS attacks work.
- Learn the types and techniques used by attackers.
- Identify vulnerabilities that allow these attacks.
- Explore detection and prevention methods.
- Perform controlled lab simulations for learning.

---

## ⚙️ Types of DoS/DDoS Attacks
1. **Volume-Based Attacks**
   - UDP Flood
   - ICMP Flood (Ping Flood)
   - Amplification Attacks (DNS, NTP, SNMP)
2. **Protocol Attacks**
   - SYN Flood
   - Smurf Attack
   - Ping of Death
3. **Application Layer Attacks**
   - HTTP Flood
   - Slowloris
   - RUDY (R U Dead Yet?)

---

## 🔍 Methodology
1. **Reconnaissance** – Identify target IP/Domain.
2. **Resource Enumeration** – Determine bandwidth, services, and open ports.
3. **Attack Execution** – Use single or distributed sources.
4. **Impact Assessment** – Observe downtime and resource usage.
5. **Cleanup & Analysis** – Stop attack and analyze logs.

---

## 🧪 Hands-on Labs
### **Lab 1: Perform a SYN Flood Attack (Hping3)**
- Use `hping3` to send rapid TCP SYN requests.
- Monitor ser
