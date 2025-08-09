🛑 Denial of Service (DoS) & Distributed Denial of Service (DDoS)

    DoS (Denial of Service) --- A Denial of Service attack is when an attacker tries to make a system, network, or application unavailable to legitimate users by overloading it with malicious traffic or exploiting resource bottlenecks.
    1) Single origin (one computer or network connection)
    2) Can target: a) Websites b) APIs c) Databases d) Networks

    DDoS (Distributed Denial of Service) --- A Distributed Denial of Service is an evolved version of DoS where multiple systems (often thousands/millions) attack a target simultaneously.
    1) Sources are usually botnets (infected devices like PCs, IoT devices, servers)
    2) Harder to block because traffic comes from many different IP addresses
    3) Often uses amplification/reflection techniques


2️⃣ Objectives
    
    1) Disruption of services
    2) Financial damage through downtime
    3) Reputation loss for target
    4) Extortion (“Pay us or we’ll keep the attack going”)
    5) Diversion for other attacks (e.g., data breach during chaos)
    6) Hacktivism (political or social statement)

3️⃣ Technical Background — How They Work
    
    1) Both DoS and DDoS attacks work by overwhelming a target’s finite resources:
    2) Bandwidth saturation (network pipe clogged)
    3) CPU/RAM exhaustion (server can't process requests)
    4) Application-level overload (web server threads maxed out)
    5) Protocol abuse (half-open TCP connections consume state tables)

4️⃣ Types of DoS/DDoS Attacks
    
     A. Volumetric Attacks (Layer 3 & 4)
         1) Goal: Saturate network bandwidth
         2) Examples:
            a) UDP Flood
            b) ICMP (Ping) Flood
            c) DNS Amplification
            d) NTP Amplification
            e) SSDP Reflection
         3) Amplification: Send small requests that cause much larger replies to the victim (ratio can be 1:50 or more)
   
     B. Protocol Attacks (Layer 3 & 4)
         1) Goal: Exhaust server or network device resources
         2) Examples:
            a) SYN Flood (TCP handshake abuse)
            b) ACK Flood
            c) Ping of Death
            d) Smurf Attack
            e) Teardrop Attack (IP fragmentation bugs)
    
     C. Application Layer Attacks (Layer 7)
         1) Goal: Target specific app functions
         2) Examples:
            a) HTTP GET Flood
            b) HTTP POST Flood
            c) Slowloris (keeps connections open indefinitely)
            d) RUDY (“R U Dead Yet?” — slow POST data transfer)
            e) Zero-day app vulnerabilities

5️⃣ Tools Commonly Used

           Tool	                           Type	                         Notes
1) LOIC (Low Orbit Ion Cannon)   ---       	DoS   ---     	      GUI, simple, easy to trace
2) HOIC (High Orbit Ion Cannon)  ---    	  DoS/DDoS ---          Booster scripts, higher power
3) Hping3	                       ---        DoS/DDoS	---         Custom packet crafting
4) Slowloris                     ---      	App Layer DoS	---Apache-targeted slow request attack
5) Xerxes	                       ---        DDoS	       ---       HTTP flooding
6) MHDDoS	                       ---        DDoS	   ---           Multi-method Python toolkit
7) Mirai                         ---        Botnet	DDoS	---      Famous IoT botnet
8) RUDY	                         ---        App Layer DoS	           Very slow HTTP POST floods




6️⃣  How to Detect a DoS/DDoS Attack

    Signs:
     1) Unusual traffic spikes
     2) Services slowing or becoming unresponsive
     3) Network latency increase
     4) Large number of connections from unusual locations
     5) Logs filled with repetitive request patterns

7️⃣ Defense and Mitigation Strategies
  
    Infrastructure Hardening
      1) Increase bandwidth capacity
      2) Use load balancers
      3) Redundant server locations (geo-distributed)

    Traffic Filtering
      1) Firewalls with anti-DDoS rules
      2) Intrusion Prevention Systems (IPS)
      3) Rate limiting
      4) Geo-blocking suspicious regions

    DDoS Protection Services
      1) Cloudflare
      2) AWS Shield
      3) Google Cloud Armor
      4) Akamai Kona Site Defender

    Application-Level Defenses
      1) CAPTCHA for suspicious requests
      2) Session validation
      3) Input throttling
      
    Network Tricks
      1) Blackhole routing (discard all traffic to target)
      2) Sinkhole routing (divert and analyze attack traffic)
      3) Anycast routing (distribute load globally)


