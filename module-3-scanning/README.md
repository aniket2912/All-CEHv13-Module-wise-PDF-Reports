Nmap commands and switches

HOST DISCOVERY

-sn -- no port scanning
-Pn -- disable ICMP echo request
-PS -- TCP SYN packet
-PA -- TCP ACK
-PU -- UDP 
-PE -- ICMP ECHO
-PP -- Timestamp
-PM -- net mask request
-n  -- disable dns resolution

--traceroute -- trace hop path to each host 


SCAN TECHNIQUES

-sS -- send SYK packet to target ( two way handshake ) or half scanning
-ST -- send TCP packets (three way handshake) or full scanning
-sA -- send ACK packet
-sW -- for windows 
-sM -- maimon scans
-sU -- scan UDP ports
-SN -- send null packet
-sF -- send FIN packet
-sX -- xmass scan , sends at a time three packets (FIN , PSH, RST)


PORT  SPECIFICATION AND SCAN ORDER 

-p -- FOR PORT SCAN AND ALSO SCAN A SPECIFIC PORT LIKE -p21 ,-p22
--excluded-ports -- excluded the specified port from scanning
-F -- fast scanning , scan first 100 ports
-r -- scan port sequantually
--top-ports -- scan most common ports


SERVICE VERSION DETECTION 

-sV -- service version detetction ...show running ports versions


SCRIPTS SCANS

-sC -- default script
--scripts = files and script categories


OS DETECTIONS 

-O -- to checks operating system of target system
--osscan-limit : limit os detection to promising targets
--osscan-guess -- guess OS more aggressively


TIMING AND PERFORMANCE

-T<0-5> -- Set time tamplate 
--scan-delay / --max-scan-delay --adjust delay between time
--min-rate <number> --sends packet no slower than <number> per second
--max-rate <number> -- sends packets no faster than <number> per second


FIREWALL / IDS EVANSION AND SPOOFING

-f -- fragmentation ( divide a single packet into multiple pieces 
-D RND:<number> -- Decoy ( hide our real ip address and generate random ip address
-S < ip add > -- spoof source address 
-g / --source-port <port num> -- for post spoofing and hide our ip and generate duplicate
--spoof-mac -- 0 -- to replace source mac with random mac


OUTPUT 

-oN -- save output in normal format
-oX -- save output in xml format
-oS -- greapable format
-oA -- output in the three major format at once
-v  -- verbocity 

MISC 

-A -- perform os detection ,service version detection ,script scanning 
-V -- print version number
-h -- print help massage


HPING3 Commads 
hping3 -- genereate fake packets 
smurf / land / broadcasting attack
certend watch video

man hping3 

hping3 -S -- for SYN packet
-1 --icmp packet
-8 -- 
-a -- spoofing 
-c -- count
--rand-source  
hping3 -1 162.241.216.11 -a 162.241.216.11 -p 80 --fast
hping3 -8 1-1000 162.241.216.11 -S -X -- for scanning 1000 ports

websites for attack --
testfire.net
certifiedhacker.com
hackthissite.org
hackerone.com


