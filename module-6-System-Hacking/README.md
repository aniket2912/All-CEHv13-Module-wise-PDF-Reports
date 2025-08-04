🔐 System Hacking: 
🔸 1. What is System Hacking?
System hacking is the process of exploiting system-level vulnerabilities to gain unauthorized access to computer systems. It is usually conducted in four main phases:

Gaining Access

Escalating Privileges

Maintaining Access

Clearing Tracks

🔸 2. Phases of System Hacking
📌 Phase 1: Gaining Access
Objective: Crack user or admin credentials.

Password Cracking Techniques:

Brute Force Attack

Dictionary Attack

Rainbow Table Attack

Hybrid Attack

Keylogger-based attack

Social Engineering

Tools: Hydra, Medusa, John the Ripper, Mimikatz

📌 Phase 2: Privilege Escalation
Objective: Obtain elevated access (Admin/Root).

Types:

Vertical (User ➝ Admin)

Horizontal (User ➝ Another User)

Techniques:

Exploiting misconfigured services

Kernel exploits

DLL hijacking

Scheduled tasks abuse

Tools: PowerUp, Linux Exploit Suggester, WinPEAS

📌 Phase 3: Maintaining Access
Objective: Keep long-term access.

Techniques:

Backdoors

Rootkits

Creating hidden users

Scheduled jobs

Tools: Netcat, Metasploit, Ngrok, Web Shells

📌 Phase 4: Clearing Tracks
Objective: Erase all evidence of intrusion.

Techniques:

Clearing logs (Event Viewer, Syslog)

Timestamp modification

Disabling auditing

Tools: Meterpreter, Auditpol, Winzapper

🔸 3. Key Tools Used in System Hacking
Tool	           Purpose
Mimikatz ---	Password dumping & pass-the-hash
Cain & Abel ---	Cracking Windows passwords
Metasploit ---	Exploiting vulnerabilities
Netcat ---	Creating reverse shells/backdoors
Nmap ---	Discovering open ports/services
John the --- Ripper	Password brute force
PsExec ---	Remote code execution

🔸 4. Defensive Measures
Technique	Description
Patch Management 
Keep OS and software up-to-date
Account Lockout Policies
Prevent brute-force attacks
Multi-Factor Authentication	Hardens login process
IDS/IPS Systems	Detect intrusion
Event Log Monitoring	Detect unauthorized access

🔸 
