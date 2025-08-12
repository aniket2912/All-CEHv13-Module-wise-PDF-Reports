# Session Hijacking

## 📌 Introduction
Session Hijacking is a security attack where an attacker exploits an active session between a client and a server to gain unauthorized access to information or services. This is typically done by stealing or manipulating session tokens, cookies, or authentication credentials.

---

## 🎯 Objectives of Session Hijacking
- Understand the concept and types of session hijacking.
- Learn how attackers steal active sessions.
- Explore tools and techniques for detecting and preventing attacks.
- Perform hands-on practice to understand exploitation methods.

---

## 🛠️ Types of Session Hijacking
1. **Active Session Hijacking** – The attacker takes over an active session.
2. **Passive Session Hijacking** – The attacker monitors traffic without interfering.
3. **Session Fixation** – The attacker sets a known session ID before login.
4. **Session Sidejacking** – Stealing session cookies from network traffic.
5. **Cross-Site Scripting (XSS)-based Hijacking** – Injecting scripts to steal session data.

---

## ⚙️ Common Attack Vectors
- **Packet Sniffing** (e.g., HTTP traffic without encryption)
- **Man-in-the-Middle (MITM) Attacks**
- **Cross-Site Scripting (XSS)**
- **Predictable Session IDs**
- **Session Replay Attacks**

---

## 🔍 Methodology
1. **Identify Target Session** – Through sniffing or scanning.
2. **Steal Session ID** – Using tools like Wireshark, Burp Suite, or Ettercap.
3. **Inject Session** – Modify browser cookies or HTTP headers.
4. **Maintain Access** – Create persistence in the compromised session.
5. **Clear Tracks** – Delete logs and reset manipulated cookies.

---

## 🧪 Hands-on Labs
### **Lab 1: Capturing Session ID via Wireshark**
- Monitor network traffic.
- Filter HTTP requests.
- Identify session cookies.

### **Lab 2: Hijacking a Session with Cookie Injection**
- Extract session cookie using Burp Suite.
- Modify browser cookie using developer tools.
- Access the victim’s account.

### **Lab 3: Sidejacking over HTTP**
- Capture unencrypted session tokens.
- Replay captured token to gain access.

---

## 🛡️ Prevention & Mitigation
- Use **HTTPS** for all communications.
- Implement **Secure & HttpOnly Cookies**.
- Enable **Session Expiry & Rotation**.
- Use **Multi-Factor Authentication**.
- Detect anomalies in session behavior.

---

## 🧰 Tools for Session Hijacking
- **Wireshark** – Packet capture and analysis.
- **Ettercap** – MITM and sniffing.
- **Burp Suite** – Web traffic interception.
- **Cain & Abel** – Network sniffing and credential recovery.
- **Bettercap** – Advanced MITM attacks.

---

## 📄 Reporting & Documentation
When performing session hijacking in a penetration test:
- Document the method used.
- Provide captured evidence (screenshots, logs).
- Recommend specific fixes.

---

## ⚠️ Disclaimer
This repository is for **educational and ethical penetration testing purposes only**. Unauthorized attacks on systems without permission are illegal and punishable under cybercrime laws.
