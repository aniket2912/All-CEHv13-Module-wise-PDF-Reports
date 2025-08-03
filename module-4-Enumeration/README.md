🔍 What is Enumeration?
Enumeration is the process of actively connecting to a target system to discover usernames, shared resources, network services, and other information. It’s often performed after scanning and before exploitation.

📚 Types of Enumeration
1. NetBIOS Enumeration
Tools: nbtstat, nbtscan, enum4linux

Finds: Computer names, workgroups, shared drives

2. SNMP Enumeration
Tool: snmpwalk, snmp-check

Finds: Network device information (routers, switches, etc.)

3. LDAP Enumeration
Tool: ldapsearch, Softerra LDAP Browser

Finds: Domain users, groups, policies in Active Directory

4. SMTP Enumeration
Tools: smtp-user-enum, Telnet

Finds: Valid email accounts

5. NFS Enumeration
Tool: showmount

Finds: Shared directories on Unix/Linux systems

6. SMB Enumeration
Tools: smbclient, enum4linux, smbmap

Finds: Shared folders, users, groups

7. RPC Enumeration
Tools: rpcclient, nmap -sT -sU -p 135

Finds: Services and ports over Remote Procedure Call

8. DNS Enumeration
Tools: nslookup, dig, dnsenum, dnsrecon

Finds: Hostnames, IPs, subdomains, zone transfers

9. Linux/Unix Enumeration
Tool: Manual commands or scripts like LinEnum, Linux Exploit Suggester

Finds: Privilege escalation paths

10. Windows Enumeration
Tools: PowerView, Net commands, wmic, winPEAS

Finds: Users, groups, shares, tokens


