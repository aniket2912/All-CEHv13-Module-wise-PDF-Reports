# 🔐 Cryptography

## 📌 Introduction
**Cryptography** is the practice of securing information by transforming it into a form that is unreadable to unauthorized users.  
It ensures confidentiality, integrity, authentication, and non-repudiation of data, forming the backbone of modern cybersecurity.

---

## 🎯 Objectives of Cryptography
- Protect sensitive data from unauthorized access.
- Ensure secure communication over untrusted networks.
- Verify authenticity of users, devices, and systems.
- Guarantee data integrity against tampering.
- Provide non-repudiation (cannot deny actions taken).

---

## 🧩 Types of Cryptography
1. **Symmetric Key Cryptography (Secret Key)**
   - Uses the same key for encryption and decryption.
   - Example: AES, DES, 3DES, RC4.
   
2. **Asymmetric Key Cryptography (Public Key)**
   - Uses a public key for encryption and a private key for decryption.
   - Example: RSA, ECC, Diffie-Hellman.

3. **Hash Functions**
   - One-way encryption used for integrity verification.
   - Example: MD5, SHA-1, SHA-256, SHA-512.

4. **Digital Signatures**
   - Provide authenticity, integrity, and non-repudiation.
   - Example: RSA signatures, DSA, ECDSA.

5. **Hybrid Cryptography**
   - Combination of symmetric and asymmetric encryption.
   - Example: SSL/TLS (uses RSA + AES).

---

## 📚 Key Concepts
- **Plaintext** – Original readable data.  
- **Ciphertext** – Encrypted, unreadable data.  
- **Key** – A secret value used in encryption/decryption.  
- **Cipher** – Algorithm used to perform encryption/decryption.  
- **Salt** – Random value added to hashing for better security.  
- **Initialization Vector (IV)** – Random value used in encryption to ensure randomness.  

---

## 🧪 Cryptographic Algorithms
### Symmetric Algorithms
- DES (Data Encryption Standard) – obsolete but historical.
- 3DES – more secure than DES but slower.
- AES (Advanced Encryption Standard) – widely used, secure.
- Blowfish, Twofish – fast block ciphers.

### Asymmetric Algorithms
- RSA – encryption, digital signatures.
- ECC (Elliptic Curve Cryptography) – smaller key sizes, strong security.
- Diffie-Hellman – secure key exchange.

### Hashing Algorithms
- MD5 (128-bit, insecure).  
- SHA-1 (160-bit, insecure).  
- SHA-2 family (SHA-256, SHA-512, secure).  
- SHA-3 (latest secure standard).  

---

## 🔐 Cryptography in Real Life
- **HTTPS / SSL / TLS** – Secure web browsing.  
- **VPNs** – Encrypted communication tunnels.  
- **Email Security** – PGP, S/MIME encryption.  
- **File Encryption** – BitLocker, VeraCrypt.  
- **Digital Certificates** – PKI, X.509.  
- **Blockchain & Cryptocurrency** – Hashing + digital signatures.  

---

## 🛠️ Common Tools for Cryptography
- **OpenSSL** – Encryption, certificates, hashing.  
- **GPG (GNU Privacy Guard)** – File and email encryption.  
- **Hashcat / John the Ripper** – Password hash cracking.  
- **VeraCrypt** – Disk and file encryption.  
- **Wireshark** – Inspect encrypted traffic.  

---

## 🧪 Hands-on Labs
### Lab 1: Symmetric Encryption using OpenSSL
- Encrypt a file using AES.
- Decrypt it using the same key.

### Lab 2: Asymmetric Encryption (RSA)
- Generate RSA keys with OpenSSL.
- Encrypt and decrypt messages.

### Lab 3: Hashing and Integrity Verification
- Generate MD5, SHA-256 hashes for files.
- Verify file integrity using hashes.

### Lab 4: Digital Signatures
- Create and verify signatures with GPG/openssl.

### Lab 5: SSL/TLS Certificates
- Generate a self-signed certificate with OpenSSL.
- Configure a web server to use HTTPS.

---

## 🛡️ Defensive Practices
- Use strong algorithms (AES, RSA, ECC, SHA-2/3).  
- Avoid deprecated algorithms (DES, MD5, SHA-1).  
- Use long, random keys and rotate them periodically.  
- Implement PKI (Public Key Infrastructure) for secure key management.  
- Use SSL/TLS certificates from trusted Certificate Authorities.  

---

## 📄 Reporting & Documentation
When documenting cryptography labs or findings:
- Describe the algorithm used.  
- Provide the purpose (encryption, integrity, authentication).  
- Attach screenshots of commands and outputs.  
- Explain key sizes and security considerations.  

---

## ⚠️ Disclaimer
This repository is for **educational and authorized purposes only**.  
Cryptographic experiments must be performed in **controlled environments** and never misused for unauthorized access.  

---

