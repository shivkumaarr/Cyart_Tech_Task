# CyArt Tech – Cybersecurity Practical Tasks

## Overview

This repository contains the practical cybersecurity tasks assigned by **CyArt Tech** and the corresponding work completed in controlled lab environments.

The tasks covered network scanning, vulnerability scanning, exploitation, post-exploitation, malware analysis, password security, security assessment reporting, and Red Team documentation.

---

## 1. Network Scanning

**Task:** Scan a local network device such as Metasploitable2 using Nmap. Perform service enumeration and compare stealth and aggressive scanning techniques.

**Work Completed:**
- Performed service and version detection.
- Enumerated services using Nmap scripts.
- Documented discovered ports, services, and versions.
- Compared stealth (`-sS`) and aggressive (`-A`) scans.

**Tool:** Nmap

---

## 2. Vulnerability Scanning

**Task:** Scan Metasploitable2 using OpenVAS and prioritize identified vulnerabilities based on CVSS scores.

**Work Completed:**
- Performed vulnerability scanning.
- Reviewed and prioritized security findings.
- Documented vulnerability details and CVSS scores.
- Cross-referenced an OpenVAS finding with Metasploit to verify exploitability.

**Tool:** OpenVAS

---

## 3. Exploitation Practice

**Task:** Exploit a known vulnerability on Metasploitable2 using the Metasploit Framework and document the exploitation process.

**Work Completed:**
- Performed controlled exploitation of a vulnerable service.
- Tested the vsftpd 2.3.4 backdoor vulnerability (CVE-2011-2523).
- Documented exploitation steps and results.
- Performed a basic privilege-escalation assessment.

**Tool:** Metasploit Framework

---

## 4. Post-Exploitation and Persistence

**Task:** Simulate credential dumping, persistence, and reverse-shell communication in controlled virtual environments.

**Work Completed:**
- Performed credential-dumping testing using Mimikatz.
- Simulated persistence using a scheduled task and a harmless script.
- Established and tested a controlled reverse-shell connection using Netcat.
- Documented the results.

**Tools:** Mimikatz, Netcat

---

## 5. Malware Analysis

**Task:** Analyze a harmless test file using VirusTotal and Hybrid Analysis and document the detection and behavior results.

**Work Completed:**
- Used the EICAR test file for antivirus testing.
- Reviewed detection results on VirusTotal.
- Analyzed the sample using Hybrid Analysis.
- Documented the observed sandbox behavior.

**Tools:** VirusTotal, Hybrid Analysis

---

## 6. Password Security

**Task:** Create secure passwords using KeePassXC and perform controlled weak-password testing against a lab environment.

**Work Completed:**
- Created a secure password vault.
- Generated five strong passwords with 16+ characters.
- Tested password authentication in a virtual-machine environment.
- Performed weak-password testing using Hydra.
- Documented the results.

**Tools:** KeePassXC, Hydra

---

## 7. Security Assessment Report

**Task:** Create a security assessment report based on Nmap and OpenVAS findings using a professional reporting format.

**Work Completed:**
- Documented Nmap and OpenVAS findings.
- Prepared an executive summary.
- Documented the attack path.
- Included security findings and recommendations.

**Tool:** Google Docs

---

## 8. Red Team Operations and Documentation

**Task:** Document attack techniques, create attack-flow diagrams, build Red Team checklists, and prepare a Rules of Engagement document.

**Work Completed:**
- Documented a Metasploit exploitation technique.
- Created an attack-flow diagram.
- Developed and applied a Red Team checklist to a Metasploitable2 assessment.
- Prepared a mock Rules of Engagement document.

**Tools:** HackMD, Draw.io, Trello, Google Docs

---

## 9. MITRE ATT&CK Mapping

**Task:** Map a demonstrated Metasploit exploitation activity to a relevant MITRE ATT&CK technique.

**Work Completed:**
- Identified the relevant MITRE ATT&CK technique.
- Documented the technique ID and rationale.
- Prepared a concise technique summary.

**Tool:** MITRE ATT&CK

---

## Tools Used

**Nmap · OpenVAS · Metasploit Framework · Mimikatz · Netcat · VirusTotal · Hybrid Analysis · KeePassXC · Hydra · HackMD · Draw.io · Trello · Google Docs · MITRE ATT&CK**

---

## Disclaimer

All practical security testing activities documented in this repository were performed in authorized and controlled laboratory environments for cybersecurity training purposes.
