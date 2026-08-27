<a href="https://tcm-sec.com/"><img src="https://raw.githubusercontent.com/finnianmoore/Security-Engineering-Projects/main/images/TCM_Security_logo.svg" height="28" style="vertical-align: middle; background-color: #652d90; padding: 4px 8px; border-radius: 4px;" alt="PNPT Certified"></a>
![PNPT Certified](https://img.shields.io/badge/PNPT-Certified-652d90?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNDQwIiBoZWlnaHQ9IjE0NDAiIHZlcnNpb249IjEuMCIgdmlld0JveD0iMCAwIDEwODAgMTA4MCI+PHBhdGggZD0ibTUyNSA5MC01NyAxNi00NyAxNC04OCAyNS0xMDUgMzFxLTU1IDE2LTU3IDE4bC0xIDEzOXYxMzdoMmwzOS05IDM2LTdWMzUzYzAtOTQgMC0xMDAgMi0xMDJzNi0zIDEwMS0zMWwxOTAtNTMgMzEgNyA0OSAxNCA1NyAxNyAzNCAxMCAxOS0xNCA1OS00My0xMS00LTY1LTE5LTg0LTI0LTUwLTE1LTI1LTdxLTE0LTUtMzAgMU04MTggMTYwYy00NCAzMS03OCA1Ni0yMTEgMTU2TDQ1MCA0MzJsMjEgMjEgMjAgMjFjMCAyIDkgNiAxOSA3IDI0IDQgMzIgNyA0NCAxOSA2IDcgOSAxMCAxMiAxN3ExMSAyMSA1IDQyLTUgMjUtMjYgMzdjLTEyIDgtMjkgMTQtNDIgMTRoLTZsLTEgOC0xNyAxMDkgMzMtMjEgODYtNTUgMTQtOSAyNyAyIDEzMyA5aDZsMTAtOWE1NzggNTc4IDAgMCAwIDUyLTU5bDgtOS01LTEtMzEtOS02My0xOWMtNS0yLTctNC0yNy0yNGwtOTgtMTExIDM3LTQ2IDE0NC0xNzYgMzctNDUgMS0yek02NDkgNDk0bDI4IDMwYTUzOSA1MzkgMCAwIDEtNjktOWgtNWwxNy0xNSAxOS0xNHoiLz48cGF0aCBkPSJNODQ3IDE3OWwtMzEgNjYgNyAyYzExIDMgMTAtMTUgMTAgMTU2djE0OWwyNCA4IDI1IDctMTYgMTdhODIyIDgyMiAwIDAgMC02NCA3NyA2MDcgNjA3IDAgMCAxLTE4NCAxOTVsLTQgMyA5IDMxIDggMzJhNDIwIDQyMCAwIDAgMS0yNDUtMjcgNzQzIDc0MyAwIDAgMCAxMTkgNzlsMzUgMTlxMiAxIDM1LTE5YTk3OCA5NzggMCAwIDAgMjMwLTE4MmM0My01MSA3MS05OCA4OC0xNTAgNi0xOCA4LTI2IDE1LTcwbDItMTkzLTEtMTg1cTAtMy0yOC0xMGwtMzAtOHEtMi0yLTQgM3oiLz48cGF0aCBkPSJNODE0IDE5NGwtNzEgODktMTAzIDEzMXEtMiAwIDE2IDIybDI0IDI3IDYgNiAxMS0yMWM0Mi04MSAxMzUtMjcwIDEzMy0yNzJ6TTQyMyA0MzVsLTMxIDctMjA2IDUwLTE0IDN2OGE5ODAgOTgwIDAgMCAwIDI2IDE1OWwyNDEtMTA1cTMtMSAyLTggMS0xOCAxNS00MCA1LTcgMTctMTkgMjUtMjNsNi00LTE2LTE2LTI2LTI0Yy0xMC0xMC0xMC0xMC0yMi03Ii8+PHBhdGggZD0iTTQ5MiA0OTVhNTEgNTEgMCAwIDAtMzUgNTBxMCAyMyAxNSAzOGM1IDUgMTUgMTAgMjIgMTIgOSAzIDI0IDIgMzItMSAyMS03IDM0LTI3IDM0LTQ5cS0xLTM4LTM2LTUwYy05LTMtMjMtMy0zMiAwTTQzMyA1NzRsLTY0IDI4Yy03NiAzMS0xMTcgNTAtMTU1IDY3bC0xMSA1IDE1IDMzYTM3NSAzNzUgMCAwIDAgODIgMTEwIDE5MzEzIDE5MzEzIDAgMCAxIDE0MS0yMDBsMjAtMjgtNy0xMS03LTEweiIvPjxwYXRoIGQ9Ik00NDIgNjM3bC02MiA4OS01MyA3NC0xNyAyNmEzOTMgMzkzIDAgMCAwIDExOCA2NmwxMCA0IDEtNiA0Ny0yODQtOC01LTgtM3pNNTM3IDcwMWwtNjAgMzktNSAyNy0yMyAxMzIgMjkgNmE0MTYgNDE2IDAgMCAwIDEzMCAyYzEtMS01OC0yMTQtNTktMjE0eiIvPjwvc3ZnPg==)


# PNPT Penetration Test Report

## Overview

This repository contains the final penetration test report from my Practical Network Penetration Tester (PNPT) certification examination, conducted between May 20–27, 2026.

The report documents a full-scope internal penetration test against a fictional company, The Pasta Mentors (TPM), demonstrating the complete attack chain from initial reconnaissance to full Active Directory domain compromise.

---

## Report Highlights

The assessment successfully achieved full domain compromise through a multi-stage attack chain:

- **OSINT & External Reconnaissance:** Gathered employee information and mapped the external attack surface using open-source intelligence techniques.
- **Web Application Exploitation:** Gained initial access by credential spraying an exposed administrative portal and retrieving sensitive information from compromised mailboxes.
- **Network Pivoting:** Used compromised SSH keys to pivot from the external mail gateway into the internal network segment.
- **Kerberoasting Attack:** Extracted and cracked service account tickets, obtaining cleartext credentials for privileged accounts.
- **Credential Harvesting:** Discovered hardcoded application credentials within network shares and extracted plaintext passwords from local system secrets.
- **Domain Takeover:** Intercepted cached Domain Administrator credentials from a proprietary application, gaining full control of the Active Directory domain.
- **Persistence:** Forged a Kerberos Golden Ticket, demonstrating the ability to maintain long-term, undetectable access to the entire domain.

---

## Key Findings

| Finding ID | Title | Severity |
|------------|-------|----------|
| IPT-001 | Cleartext Credential Extraction from Proprietary Connection Tool | Critical |
| IPT-002 | Total Active Directory Domain Database Extraction via ntdsutil | Critical |
| IPT-003 | Domain Kerberos Service Identity Compromise via Offline Kerberoasting | Critical |
| IPT-004 | Plaintext Credential Exposure within Public Mapped Network Share Files | Critical |
| IPT-005 | External Management Interface Credential Fuzzing Takeover | High |
| IPT-006 | Insecure Network Architecture via Dual-Homed Gateway | High |
| IPT-007 | Cleartext Fallback Administrative Passphrase Storage in LSA Secrets | High |

---

## Tools & Techniques

- **Reconnaissance:** Sublist3r, WhatWeb, TheHarvester, Wayback Machine
- **Network Scanning:** Nmap, Gobuster, custom Bash scripts
- **Exploitation & Credential Attacks:** ffuf (credential spraying), John the Ripper (password cracking), ssh2john
- **Lateral Movement & Privilege Escalation:** impacket (secretsdump, GetUserSPNs, psexec, ticketer), Netexec, Kerbrute
- **Post-Exploitation & Persistence:** ntdsutil, Evil-WinRM, SharpHound, BloodHound

---

## Repository Contents

- [`Finnian-Moore-PNPT-Report.pdf`](./Finnian-Moore-PNPT-Report.pdf) – The final penetration test report
- [`certificate/`](./certificate/) – Contains my PNPT certification credential

---

## Verification

- [View Certificate](https://github.com/finnianmoore/Security-Engineering-Projects/blob/main/certificates/Finnian-Moore-PNPT-Certificate.pdf)
- [Verify on TCM Security's Website](https://tcm-sec.com/verify)

---

## Certifications

- **PNPT** – Practical Network Penetration Tester (TCM Security, 2026)
- **PJPT** – Practical Junior Penetration Tester (TCM Security, 2026)
- **Security+** – CompTIA (2025)

---

## Disclaimer

This report is from a simulated, authorized penetration test conducted against a fictional company (The Pasta Mentors) as part of the PNPT certification exam. No real client data or intellectual property is included. All systems and data described are part of a controlled lab environment.

---

**Note:** This report demonstrates my ability to conduct a full-scope penetration test, document findings, and deliver a professional report suitable for both technical and executive audiences.

---

*Report Author: Finnian Moore*  
*Date: May 27, 2026*  
*Classification: CONFIDENTIAL*# PNPT Penetration Test Report

## Overview

This repository contains the final penetration test report from my Practical Network Penetration Tester (PNPT) certification examination, conducted between May 20–27, 2026.

The report documents a full-scope internal penetration test against a fictional company, The Pasta Mentors (TPM), demonstrating the complete attack chain from initial reconnaissance to full Active Directory domain compromise.

---

## Report Highlights

The assessment successfully achieved full domain compromise through a multi-stage attack chain:

- **OSINT & External Reconnaissance:** Gathered employee information and mapped the external attack surface using open-source intelligence techniques.
- **Web Application Exploitation:** Gained initial access by credential spraying an exposed administrative portal and retrieving sensitive information from compromised mailboxes.
- **Network Pivoting:** Used compromised SSH keys to pivot from the external mail gateway into the internal network segment.
- **Kerberoasting Attack:** Extracted and cracked service account tickets, obtaining cleartext credentials for privileged accounts.
- **Credential Harvesting:** Discovered hardcoded application credentials within network shares and extracted plaintext passwords from local system secrets.
- **Domain Takeover:** Intercepted cached Domain Administrator credentials from a proprietary application, gaining full control of the Active Directory domain.
- **Persistence:** Forged a Kerberos Golden Ticket, demonstrating the ability to maintain long-term, undetectable access to the entire domain.

---

## Key Findings

| Finding ID | Title | Severity |
|------------|-------|----------|
| IPT-001 | Cleartext Credential Extraction from Proprietary Connection Tool | Critical |
| IPT-002 | Total Active Directory Domain Database Extraction via ntdsutil | Critical |
| IPT-003 | Domain Kerberos Service Identity Compromise via Offline Kerberoasting | Critical |
| IPT-004 | Plaintext Credential Exposure within Public Mapped Network Share Files | Critical |
| IPT-005 | External Management Interface Credential Fuzzing Takeover | High |
| IPT-006 | Insecure Network Architecture via Dual-Homed Gateway | High |
| IPT-007 | Cleartext Fallback Administrative Passphrase Storage in LSA Secrets | High |

---

## Tools & Techniques

- **Reconnaissance:** Sublist3r, WhatWeb, TheHarvester, Wayback Machine
- **Network Scanning:** Nmap, Gobuster, custom Bash scripts
- **Exploitation & Credential Attacks:** ffuf (credential spraying), John the Ripper (password cracking), ssh2john
- **Lateral Movement & Privilege Escalation:** impacket (secretsdump, GetUserSPNs, psexec, ticketer), Netexec, Kerbrute
- **Post-Exploitation & Persistence:** ntdsutil, Evil-WinRM, SharpHound, BloodHound

---

## Repository Contents

- [`Finnian-Moore-PNPT-Report.pdf`](./Finnian-Moore-PNPT-Report.pdf) – The final penetration test report
- [`certificate/`](./certificate/) – Contains my PNPT certification credential

---

## Verification

- [View Certificate](./certificate/Finnian-Moore-PNPT-Certificate.pdf)
- [Verify on TCM Security's Website](https://tcm-sec.com/verify)

---

## Certifications

- **PNPT** – Practical Network Penetration Tester (TCM Security, 2026)
- **PJPT** – Practical Junior Penetration Tester (TCM Security, 2026)
- **Security+** – CompTIA (2025)

---

## Disclaimer

This report is from a simulated, authorized penetration test conducted against a fictional company (The Pasta Mentors) as part of the PNPT certification exam. No real client data or intellectual property is included. All systems and data described are part of a controlled lab environment.

---

**Note:** This report demonstrates my ability to conduct a full-scope penetration test, document findings, and deliver a professional report suitable for both technical and executive audiences.

---

*Report Author: Finnian Moore*  
*Date: May 27, 2026*  
*Classification: CONFIDENTIAL*
