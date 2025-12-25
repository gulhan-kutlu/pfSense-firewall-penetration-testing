# pfSense-firewall-penetration-testing

## Penetration Testing a pfSense Firewall

This repository documents a hands-on penetration testing and firewall hardening case study conducted in a controlled academic lab environment.

The project focuses on analyzing, testing, and improving the security posture of a network protected by a pfSense firewall using industry-standard penetration testing methodologies and tools.

> ⚠️ This is a **defensive security lab and architecture case study**, not an exploitation guide.


### Project Overview

The objective of this project was to:
- Assess firewall rule effectiveness
- Identify exposed services and misconfigurations
- Perform vulnerability scanning
- Apply remediation steps
- Validate security improvements through re-scanning

The environment simulates a real-world enterprise network including:
- DMZ
- Internal LAN
- Firewall perimeter
- External attacker perspective


### Lab Environment

**Firewall**
- pfSense (Firewall & Router)

**Operating Systems**
- Windows Server 2019 (Target systems)
- Kali Linux (Attacker)
- Linux-based vulnerability scanner

**Security Tools**
- Nessus
- OpenVAS / Greenbone
- Nmap
- Traceroute


### Penetration Testing Methodology

The project follows a structured penetration testing lifecycle:

1. **Reconnaissance**
   - Traceroute analysis
   - Network discovery
2. **Port Scanning**
   - Nmap default and advanced scans
3. **Vulnerability Scanning**
   - Nessus vulnerability assessment
   - OpenVAS full and fast scans
4. **Analysis**
   - Identification of medium and low-risk vulnerabilities
   - Firewall rule evaluation
5. **Remediation**
   - Removal of overly permissive firewall rules
   - Tightening inbound and outbound access policies
6. **Validation**
   - Re-running vulnerability scans
   - Confirming risk reduction

## Key Findings
- Overly permissive WAN firewall rules exposed internal systems
- Default “allow all” LAN rules increased attack surface
- Public-facing services required stricter port-level control
- IDS visibility improved early attack detection

### Remediation Actions
- Removed unrestricted WAN access rules
- Restricted inbound services to required ports only
- Hardened LAN outbound firewall policies
- Revalidated security posture using vulnerability rescans

### Security Concepts Demonstrated
- Firewall rule analysis and hardening
- DMZ security principles
- Defense-in-depth
- Vulnerability management lifecycle
- Difference between white-box and black-box penetration testing
- Secure network architecture reasoning

### Vulnerability Scan Validation (OpenVAS)
The screenshot below shows the results of an OpenVAS (Greenbone) vulnerability scan
performed against the DMZ target after firewall hardening.

No high, medium, or low severity vulnerabilities were detected,
indicating an improved security posture following configuration changes.

<img width="652" height="467" alt="Screenshot 2025-12-25 at 12 27 58 PM" src="https://github.com/user-attachments/assets/5fe56cdb-f98a-41e3-9177-1e24707973bb" />



### Vulnerability Scan Results (Nessus)

The screenshot below shows the results of a Nessus vulnerability scan
performed against DMZ assets protected by a pfSense firewall.

Only informational findings were detected, indicating that no critical,
high, or medium-risk vulnerabilities were present after firewall hardening
and service exposure reduction.

<img width="657" height="469" alt="Screenshot 2025-12-25 at 12 25 03 PM" src="https://github.com/user-attachments/assets/29944b06-cd58-45ef-bbc5-52df65a742d8" />

### Outcome
> Firewall hardening actions successfully reduced the attack surface,
with post-remediation scans confirming no critical or high-risk vulnerabilities.

 
### Visual Documentation
This repository includes:
- Network topology diagrams
- Firewall rule screenshots
- Vulnerability scan summaries

> Screenshots are provided **for documentation purposes only**.  
> No credentials, proprietary configurations, or production systems are exposed.


### Disclaimer
- This project was completed in an **academic lab environment**
- No real-world organization or production network was tested
- No exploitation beyond controlled scanning was performed
- Shared strictly for **educational and portfolio purposes**


