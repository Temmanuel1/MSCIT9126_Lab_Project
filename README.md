# MSCIT 9126 Lab Project

Secure version-control and network-security laboratory for the University of Kigali MSCIT 9126 module.

> Approved substitution required: Metasploitable 2 replaces the original Windows XP target. Obtain lecturer approval because the assignment names Windows XP and MS08-067.

## Architecture
- Internal LAN: 10.0.0.0/24 - Kali Linux workstation
- Guest VLAN: 172.16.0.0/24 - Windows 10 client
- DMZ: 192.168.1.0/24 - Metasploitable 2 target
- OPNsense enforces segmentation, default-deny policy, least privilege, and logging.

## Repository structure
- docs/security_policy.md - access, review, incident-response, and compliance policy
- docs/network_diagram.md - architecture and trust boundaries
- docs/test_results.md - evidence-based testing template
- configs/firewall_rules.txt - documented rule set
- configs/opnsense_backup.xml - redacted-backup placeholder
- screenshots/lab_setup - lab evidence
- screenshots/test_results - scan, exploit, traffic, log, and VPN evidence

## Setup
1. Build isolated VirtualBox internal networks.
2. Place Kali on LAN_NET, Windows 10 on GUEST_NET, and Metasploitable 2 on DMZ_NET.
3. Configure OPNsense interfaces and rules.
4. Run only authorised tests and record actual results.
5. Add screenshots with student ID and date/time visible.

## Test summary
| Area | Expected | Actual |
|---|---|---|
| Guest to LAN | Blocked | Add evidence |
| DMZ to LAN | Blocked | Add evidence |
| Metasploitable service scan | Findings documented | Add evidence |
| Controlled Metasploit exploit | Success or documented failure | Add evidence |
| VPN to approved LAN service | Allowed | Add evidence |

## Evidence rule
Never invent scan results or screenshots. Replace placeholders using output from the isolated authorised lab.

## References
NIST CSF 2.0; NIST SP 800-207; ISO/IEC 27001:2022; official Rapid7, OPNsense, Kali, Wireshark, and Git documentation.
