# ☁️ Cloud Computing

## 📌 Introduction
**Cloud Computing** is the on-demand delivery of computing services like servers, storage, databases, networking, software, and analytics over the internet (“the cloud”).  
Instead of owning and maintaining physical infrastructure, organizations can rent resources from cloud service providers (CSPs) such as AWS, Microsoft Azure, and Google Cloud.  

---

## 🎯 Objectives of Cloud Computing
- Enable **scalable and flexible IT resources**.  
- Reduce **infrastructure costs** by using pay-as-you-go models.  
- Improve **business agility** and **time-to-market**.  
- Provide **high availability and redundancy**.  
- Enhance **collaboration** and **remote access**.  
- Strengthen **data security** and **compliance** through cloud governance.  

---

## 🏗️ Cloud Computing Service Models
1. **IaaS (Infrastructure as a Service)**  
   - Provides virtualized computing resources (VMs, storage, networking).  
   - Example: AWS EC2, Azure VMs.  

2. **PaaS (Platform as a Service)**  
   - Provides application development platforms with OS, DB, and runtime environment.  
   - Example: Google App Engine, Heroku.  

3. **SaaS (Software as a Service)**  
   - Provides fully managed software accessible via browser.  
   - Example: Gmail, Microsoft 365, Salesforce.  

---

## 🌐 Cloud Deployment Models
- **Public Cloud** – Resources owned and managed by CSP (e.g., AWS, Azure).  
- **Private Cloud** – Dedicated infrastructure for a single organization.  
- **Hybrid Cloud** – Combination of public and private for flexibility.  
- **Community Cloud** – Shared infrastructure among organizations with common needs.  

---

## 🔐 Security Concerns in Cloud Computing
- **Data Breaches** – Unauthorized access to sensitive information.  
- **Data Loss** – Due to accidental deletion or provider outage.  
- **Insider Threats** – Malicious insiders exploiting cloud systems.  
- **Insecure APIs** – Exploitable cloud interfaces and APIs.  
- **Misconfigurations** – Common cause of cloud security incidents.  
- **DDoS Attacks** – Targeting cloud-hosted applications.  

---

## 🛠️ Cloud Security Best Practices
- Use **multi-factor authentication (MFA)**.  
- Encrypt **data at rest and in transit**.  
- Apply **least privilege principle** for user access.  
- Regular **cloud configuration audits**.  
- Enable **logging and monitoring** for visibility.  
- Use **WAFs, IDS/IPS** in cloud workloads.  
- Adopt **shared responsibility model** awareness.  

---

## 📂 Common Cloud Pentesting Methodology
1. **Reconnaissance** – Identify CSP, services, and public-facing assets.  
2. **Service Enumeration** – Find open buckets, exposed APIs, cloud services.  
3. **Vulnerability Identification** – Detect misconfigured storage, weak IAM roles.  
4. **Exploitation** – Attempt privilege escalation, lateral movement.  
5. **Post-Exploitation** – Data exfiltration, persistence.  
6. **Reporting** – Document risks and suggest mitigations.  

---

## 🧰 Tools for Cloud Security & Pentesting
- **ScoutSuite** – Multi-cloud security auditing tool.  
- **CloudSploit** – Detect misconfigurations.  
- **Pacu** – AWS exploitation framework.  
- **CS Suite** – Security assessment toolkit.  
- **Burp Suite / OWASP ZAP** – API and web app testing in the cloud.  
- **AWS CLI / GCP CLI / Azure CLI** – Cloud service enumeration.  

---

## 🧪 Practical Labs
### Lab 1: Identify Cloud Deployment Model
- Analyze whether the target is **public, private, or hybrid cloud**.

### Lab 2: Enumerate S3 Buckets (AWS Example)

    aws s3 ls

### Lab 3: Scan for Misconfigured Cloud Storage

    Check publicly accessible blobs/buckets

### Lab 4: Exploit Weak IAM Policies

    Attempt privilege escalation using misconfigured IAM roles.

### Lab 5: Cloud Security Monitoring

    Enable and analyze CloudTrail / CloudWatch / Security Center logs.

---

## 📊 Compliance Standards in Cloud

ISO 27017 / 27018 – Cloud-specific security and privacy controls.

PCI-DSS – Protect payment data in the cloud.

HIPAA – Secure healthcare data in the cloud.

GDPR – Protect personal data in the EU cloud environments.

---

## 🛡️ Defensive Countermeasures

Implement Zero Trust Security in cloud environments.

Regular patch management of cloud workloads.

Use cloud-native security tools like GuardDuty (AWS), Defender (Azure).

Enforce data backup and disaster recovery.

Apply continuous monitoring with SIEM.

---

## ⚠️ Disclaimer

This repository is for educational purposes only.
Do not attempt unauthorized cloud exploitation. Always test in authorized labs or accounts.
