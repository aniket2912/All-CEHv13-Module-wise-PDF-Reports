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
1) Mimikatz ---	Password dumping & pass-the-hash.
2) Cain & Abel ---	Cracking Windows passwords.
3) Metasploit ---	Exploiting vulnerabilities.
4) Netcat ---	Creating reverse shells/backdoors.
5) Nmap ---	Discovering open ports/services.
6) John the --- Ripper	Password brute force.
7) PsExec ---	Remote code execution.

🔸 4. Defensive Measures
1) Technique	Description.
2) Patch Management .
3) Keep OS and software up-to-date.
4) Account Lockout Policies.
5) Prevent brute-force attacks.
6) Multi-Factor Authentication.
7) Hardens login process.
8) IDS/IPS Systems	Detect intrusion.
9) Event Log Monitoring	Detect unauthorized access.
