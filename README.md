# PNPT Penetration Test Report

## Overview

This repository contains the final penetration test report from my Practical Network Penetration Tester (PNPT) certification examination, conducted between May 20-27, 2026.

The report documents a full-scope internal penetration test against a fictional company, The Pasta Mentors (TPM), demonstrating the complete attack chain from initial reconnaissance to full Active Directory domain compromise.

## Report Highlights

The assessment successfully achieved full domain compromise through a multi-stage attack chain:

- **OSINT & External Reconnaissance:** Gathered employee information and mapped the external attack surface using open-source intelligence techniques.
- **Web Application Exploitation:** Gained initial access by credential spraying an exposed administrative portal and retrieving sensitive information from compromised mailboxes.
- **Network Pivoting:** Used compromised SSH keys to pivot from the external mail gateway into the internal network segment.
- **Kerberoasting Attack:** Extracted and cracked service account tickets, obtaining cleartext credentials for privileged accounts.
- **Credential Harvesting:** Discovered hardcoded application credentials within network shares and extracted plaintext passwords from local system secrets.
- **Domain Takeover:** Intercepted cached Domain Administrator credentials from a proprietary application, gaining full control of the Active Directory domain.
- **Persistence:** Forged a Kerberos Golden Ticket, demonstrating the ability to maintain long-term, undetectable access to the entire domain.

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

## Tools & Techniques

- **Reconnaissance:** Sublist3r, WhatWeb, TheHarvester, Wayback Machine
- **Network Scanning:** Nmap, Gobuster, custom Bash scripts
- **Exploitation & Credential Attacks:** ffuf (credential spraying), John the Ripper (password cracking), ssh2john
- **Lateral Movement & Privilege Escalation:** impacket (secretsdump, GetUserSPNs, psexec, ticketer), Netexec, Kerbrute
- **Post-Exploitation & Persistence:** ntdsutil, Evil-WinRM, SharpHound, BloodHound

## Repository Contents

- `Finnian-Moore-PNPT-Report.pdf` – The final penetration test report

## Certifications

- **PNPT** – Practical Network Penetration Tester (TCM Security, 2026)
- **PJPT** – Practical Junior Penetration Tester (TCM Security, 2026)
- **Security+** – CompTIA (2025)

## Disclaimer

This report is from a simulated, authorized penetration test conducted against a fictional company (The Pasta Mentors) as part of the PNPT certification exam. No real client data or intellectual property is included. All systems and data described are part of a controlled lab environment.

---

**Note:** This report demonstrates my ability to conduct a full-scope penetration test, document findings, and deliver a professional report suitable for both technical and executive audiences.

---

*Report Author: Finnian Moore*
*Date: May 27, 2026*
*Classification: CONFIDENTIAL*
