
1. Introduction to Sniffing
Sniffing is the process of monitoring and capturing network packets to analyze the data transmitted over a network.
It can be legitimate (network troubleshooting, performance monitoring) or malicious (stealing sensitive data like credentials).

Types of Sniffing
   1) Passive Sniffing ---
      i) Listens to traffic without modifying it.
     ii) Works in a hub-based network or using promiscuous mode.
         Example: Wireshark capture of broadcast traffic.

   2) Active Sniffing ---
      i) Interferes with network traffic to redirect it to the attacker’s machine.
      ii) Works in switch-based networks.
      iii) Techniques include ARP Poisoning, MAC Flooding, and DHCP Spoofing.

2. How Sniffing Works
   i) Network Interface Card (NIC) is set to Promiscuous Mode to capture all packets.
   ii) Sniffer tools read raw packets at Data Link Layer (Layer 2) or Network Layer (Layer 3).
   iii) Data is decoded into a human-readable form for analysis.

3. Protocols Vulnerable to Sniffing
   1) Clear-text protocols are most vulnerable:
       a) HTTP
       b) FTP
       c) Telnet
       d) SMTP
       e) POP3
       f) IMAP
       g) SNMP v1 & v2
       h) DNS (queries in plain text)

   2) Secure alternatives:--
      --> HTTPS, SFTP, SSH, SMTPS, POP3S, SNMPv3

4. Active Sniffing Techniques
   1) MAC Flooding --> Overloads switch CAM table → Switch acts like a hub.
      Tools: macof.

   2) ARP Poisoning / ARP Spoofing --> Sends fake ARP replies to associate attacker MAC with victim’s IP.
      Tools: Ettercap, Cain & Abel, arpspoof.

   3) DHCP Spoofing --> Rogue DHCP server assigns attacker-controlled IP settings.

   4) DNS Poisoning --> Redirects victim to malicious sites by spoofing DNS replies.

   5) MITM (Man-in-the-Middle) via Sniffing --> Intercepts and modifies traffic between two parties.

5. Sniffing Tools
   1) Wireshark – Deep packet inspection and protocol analysis.
   2) tcpdump – CLI-based packet capture.
   3) Ettercap – Active sniffing, MITM attacks.
   4) Cain & Abel – ARP poisoning + password sniffing.
   5) dsniff – Suite for capturing passwords over network.
   6) Kismet – Wireless network sniffing.
   7) TShark – CLI version of Wireshark.
   8) Snort – IDS/IPS with packet logging capability.

6. Wireless Sniffing
   1) Involves capturing packets from wireless networks.
   2) Modes: Monitor Mode for packet capture.
   3) Tools: Aircrack-ng, Kismet, Wireshark.
   4) Vulnerable networks: Open Wi-Fi, WEP, WPA/WPA2 with weak passphrases.

7. Detecting Sniffing
   1) ARP Inspection: Detect unusual ARP entries.
   2) Ping Test: Send a ping with wrong MAC → Sniffer in promiscuous mode responds.
   3) Network Scanning Tools: Nmap with --script=sniffer-detect.
   4) IDS/IPS Systems: Detect unusual traffic patterns.

8. Preventing Sniffing
   1) Use Encryption (HTTPS, SSH, VPN, TLS).
   2) Use Switches instead of hubs.
   3) Enable Port Security on switches (MAC binding).
   4) Use Static ARP entries where possible.
   5) Use Network Segmentation (VLANs).
   6) Deploy IDS/IPS for suspicious activity.
   7) Regular ARP table monitoring.
