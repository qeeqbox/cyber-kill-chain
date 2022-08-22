<p align="center"> <img src="https://raw.githubusercontent.com/qeeqbox/kill-chain/main/kill-chain.png"></p>

## Kill Chain


## Steps
#### Reconnaissance
Threat actor gathers information about the target
- Passive
- Active

##### Security controls
- Detect: NIDS, Threat Intelligence, Logs (SIEM)
- Deny: Information Sharing Policies, Firewall ACL
- Disrupt: Active Defenses
- Degrade: Honeypot, Redirect Loops, Active Defenses
- Deceive: Create Fake Posting, Degrade cell

#### Weaponization
Threat actor creates an attack vector (malware, email attachments, web pages, links, pop-ups, messages, social engineering, etc..) that can exploit the vulnerabilities from the reconnaissance step. The attack vector will be the entry point

##### Security controls
- Detect: NIDS, Threat Intelligence
- Deny: NIPS

#### Delivery
The threat actor delivers the attack vector to the target

##### Security controls
- Detect: NIDS, HIDS\AV
- Deny: Web/Email/Proxy Filter, Application Whitelisting, AV
- Disrupt: Web/Email/Proxy Filter, AV
- Degrade: Sinkhole, Queuing, Deny, and Distrubt cells
- Deceive: Honeypot

#### Exploitation
Once the attack vector is on the target, the target is either breached or ready to be breached (The threat actor needs to execute the attack vector)

- Detect: NIDS, HIDS\AV
- Deny: HIPS, AV, Secure Password, Hardened systems (Patch Management)
- Disrupt: Deny cell, DEP
- Degrade: Restrict User Accounts
- Deceive: Honeypot

#### Installation
The attack vector will be installed on the victim’s system

##### Security controls
- Detect: HIDS\AV, Logs (SIEM), AV
- Deny: Application Whitelisting, Block Execution, Firewall ACL, Privilege separations
- Disrupt: HIPS, DEP
- Degrade: Deny cell, Disrupt cell
- Deceive: Honeypot

#### Command & Control (C2) 
The threat actor is now controlling the victim’s system, and this is where the threat actor moves laterally

##### Security controls
- Detect: HIDS\AV, NIDS
- Deny: Firewall ACL, Egress Filter, Sinkhole, Network Segmentation
- Disrupt: DEP, Sinkhole
- Degrade: Deny cell, Disrupt cell
- Deceive: Honeypot, Sinkhole, DNS Redirect

#### Actions on Objective
The threat actor will carry out their objectives (Data exfiltration, destruction, and extortion)

##### Security controls
- Detect: Logs (SIEM)
- Deny: Firewall ACL, Egress Filter, Network Segmentation
- Disrupt: Network Segmentation, DLP, NIPS, HIPS
- Degrade: Network Segmentation, Quality of Service
- Deceive: Honeypot

## ID
b35c2204-7d11-4472-8923-91fdb380b454

## References
- https://en.wikipedia.org/wiki/Kill_chain
- https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html
- https://csrc.nist.gov/CSRC/media/Presentations/The-Cyber-OODA-Loop-How-Your-Attacker-Should-Help/images-media/day3_security-automation_930-1020.pdf
