# Network Security Threats Report

Author: Edith Mbomena
Track:Security Analyst
Task: Task 4 - Network Security Threats

 1. Introduction
Cyebersecuirty matters today because there has being an increased rate of computer breaches, theft and data being lost concerning personal data,business,financial systems and digital infrastructure.
As technology continues to advance, threats such as hacking, phishing, malware and breaches are arising cybersecurity will help mitigate and protect all information and data to ensure
safety of digital systems.

Modern businesses depend on their networks to run daily operations, from communicating with customers to storing sensitive records. Most work is now done online, so a network is a core part of how a company operates. When that network is compromised, critical data can be exposed, causing severe losses, and any disruption can mean downtime, lower productivity and lost money. Beyond the immediate financial hit, a breach can also cause reputational damage, because customers and partners are less willing to trust a company that failed to protect their information.

 3. DoS / DDoS Attacks
How it works: Hackers use many computers to send data traffic into the website or server at the same time. The goal is to overwhelm a system to cause delayment.

Real-World Example:
Imagine a samll company with 20 people and all of suddenly 2000 fake
customers rush into their system and so the system becomes overwhelmed. 

Impact:
Attackers take control of many devices often forming a botnet, those devices send massive amounts of requests to a target server, the website becomes slow and unavailable.


Mitigations:
1. use traffic filtering
2. Implement   firewalls
3. Monitor Unusual Network traffic

 3. Man-in-the-Middle (MITM) Attacks
How it work: Happens when an attacker positions himself between two people communicating with eachother with an aim to disrupt, steal or even change the info being exchanged.

Real-World Example: Imagine you are at an airport and you login to a free wifi an attacker has created hotspot that looks like free airport Wifi. 
The attacker has created a malicious hotspot and he may intercept and login into your data.

Impact: Data theft, data manipulation, identity theft, and privacy violation.

Mitigations:
1. use HTTPS
2. Digital Certifications
3. use trusted VPNs

 4. IP Spoofing
How it works:
The attacker prepares a data pocket, and replace with the actual source IP address with a fake one it then travels through the network and the recieving computer
sees the false address and the attacker hides the identity to another target.

Real-World Example:
the attacker sends requests to publicly accessible DNS server, the requests contain the company IP address as the fake sender the servers send the responses to the company
instead of the attacker. The company receives a large volume of unwanted traffic.

Impact:
Financial loss, data loss, data security risks, network disruption.

Mitigations:
1. Ingress Filtering
2. firewalls and access control lists.
3. Network monitoring 

 5. DNS Poisoning / Spoofing (Bonus)
DNS poisoning is dangerous because attackers can manipulate DNS information and redirect users to malicious websites.
How it works:
* You enter a website name into your browser.
* Your device sends a request to a DNS resolver.
* The resolver finds the IP address associated with that domain name.
* The IP address is returned to your device.
* Your browser connects to the website’s server.

Real-World Example:
 when you type www.google.com into your browser, DNS finds the corresponding IP address so your device can connect to Google’s server.
Impact:
 Hackers trying to steal information.
 Malware infecting computers.
  Attackers trying to shut down web
Mitigations:
1. . Ingress Filtering
2. firewalls and access control lists.
3. Network monitoring 
  
 6. Comparison Table

| Threat | Attack Vector | Who is at Risk | Difficulty to Execute | Ease of Mitigation |

| DoS/DDoS | DoS	Flooding a server or network with excessive requests or traffic.	Medium	|Medium |
| MITM | Intercepting communication through malicious Wi-Fi,|ARP spoofing or compromised network infrastructure | Medium–High| Medium|
| IP Spoofing |Forging the source IP address in network packets. | Medium	Medium–High| | |
| DNS Poisoning |Injecting false DNS records or compromising  | DNS infrastructure to redirect users.| Medium–High	Medium |

7. Conclusion
 Effective cybersecurity requires continuous monitoring,
awareness and proactive security measures to identify and prevent threats before they cause significant damage.


 9. References
1. NIST Secure DNS Deployment Guide (2026)⁠
2. Cybersecurity and Infrastructure Security Agency (CISA). Understanding and Responding to Distributed Denial-of-Service (DDoS) Attacks. Read CISA DDoS guidance
3.  NIST guidance on IP spoofing and DDoS mitigation⁠￼.
4.MITRE ATT&CK network traffic mitigation
