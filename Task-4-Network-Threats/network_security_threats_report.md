# Research Report: Common Network Security Threats

## 📌 Objective
This report explores three of the most common network security threats—DoS/DDoS attacks, Man-in-the-Middle (MITM) attacks, and spoofing. The goal is to explain how they work, why they matter, and what can be done to stop them.

---

## 🔐 Threat 1: Denial of Service (DoS) / Distributed DoS (DDoS)
- **How it works:** In a DoS attack, an attacker overwhelms a system or network with traffic until it can’t respond to real users. In a DDoS, the attack comes from many compromised systems at once, making it harder to block.  
- **Impact:** Websites and online services become slow or completely unavailable. For businesses, this means downtime, lost revenue, and unhappy customers.  
- **Real-world example:** In 2018, GitHub was hit with one of the largest DDoS attacks ever recorded—1.3 Tbps of traffic—but survived thanks to strong defenses.  
- **How to defend:** Use rate limiting, load balancing, CDNs (like Cloudflare/Akamai), firewalls, and intrusion prevention systems to filter out bad traffic before it causes damage.  

---

## 🔐 Threat 2: Man-in-the-Middle (MITM)
- **How it works:** In a MITM attack, the attacker secretly places themselves between two communicating parties (like you and your bank). They can eavesdrop, steal sensitive info, or even alter data in real time.  
- **Impact:** Stolen credentials, intercepted communications, and compromised sessions. Imagine logging into a banking app over insecure Wi-Fi—your data could be intercepted without you realizing it.  
- **Real-world example:** Public Wi-Fi hotspots are notorious for MITM attacks, where attackers capture login details or redirect users to fake sites.  
- **How to defend:** Always use HTTPS/TLS, VPNs for untrusted networks, and certificate pinning in applications to ensure the server is really who it says it is.  

---

## 🔐 Threat 3: Spoofing (IP / ARP / DNS)
- **How it works:** Spoofing means faking digital identity. With IP spoofing, attackers send packets that look like they’re from a trusted source. With ARP spoofing, they trick devices on a local network. With DNS spoofing, they redirect you to malicious websites.  
- **Impact:** Redirected traffic, stolen data, and successful phishing attacks. Victims think they’re talking to a safe server, but really, they’re interacting with the attacker.  
- **Real-world example:** DNS cache poisoning has been used to redirect users from real banking sites to fake ones that steal login details.  
- **How to defend:** Enable DNSSEC, use packet filtering, and apply ARP protection features on switches. On the user side, verifying site certificates also helps.  

---

## 🔍 Conclusion
DoS, MITM, and spoofing attacks remind us that networks are constantly under pressure from attackers trying to exploit weak spots. The best defense is layered: strong technical safeguards (firewalls, TLS, IDS/IPS), regular patching, and user awareness. In security, prevention always costs less than recovery.

