# pfSense-firewall-penetration-testing

### pfSense Firewall Penetration Testing & DMZ Security Analysis

> This repository documents a hands-on penetration testing and security assessment lab conducted on a pfSense firewall and DMZ environment.

> The project focuses on firewall rule analysis, vulnerability scanning, network reconnaissance, and security hardening recommendations, aligned with real-world enterprise security practices.

> ⚠️ This is a security lab and architecture analysis project, not an exploitation guide.

### Scope of the Project

- Firewall rule inspection (WAN / DMZ)

- Network reconnaissance (traceroute, port scanning)

- Vulnerability assessment using Nessus and OpenVAS

- IDS visibility and attack surface evaluation

- DMZ security best practices and misconfiguration analysis

- Security hardening recommendations

###  Tools & Technologies

- pfSense Firewall

- Nessus Vulnerability Scanner

- OpenVAS (Greenbone)

- Nmap

- Linux (Attack VM)

- DMZ-based network topology

- Key Activities Performed
 
### Firewall & DMZ Analysis

- Reviewed WAN firewall rules and exposed services

Verified NAT and port exposure on DMZ interfaces

- Reconnaissance & Scanning

- Traceroute analysis to identify network path

- Nmap scans with OS detection

- Port enumeration on DMZ services

- Vulnerability Assessment

- Nessus scans (pre- and post-hardening)

OpenVAS vulnerability analysis

Validation of firewall rule effectiveness after changes

Security Evaluation

Identification of unnecessary exposed services

Analysis of least-privilege enforcement

DMZ segmentation and isolation assessment

### Security Findings & Recommendations

Key recommendations derived from the assessment include:

Enforcing least-privilege firewall rules

Restricting administrative access to management networks only

Hardening DMZ servers (service reduction, patching)

Deploying WAF and IDS monitoring

Scheduling regular authenticated vulnerability scans

### Visual Evidence

The screenshots/ directory contains sanitized screenshots demonstrating:

Firewall rule configuration

Vulnerability scan results

Port scan outputs

Traceroute and network visibility

These visuals are provided for educational and architectural reference only.


### Disclaimer

This repository does not contain:

Exploit code

Credentials

Production configurations

Confidential infrastructure details

All information is shared strictly for educational and portfolio purposes.

### Why This Matters

This project demonstrates:

Practical firewall security assessment skills

Understanding of DMZ design and attack surface reduction

Hands-on experience with industry-standard security tools

Ability to analyze, document, and recommend security improvements
