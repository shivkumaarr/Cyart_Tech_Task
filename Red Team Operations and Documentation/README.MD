# Red Team Operations and Documentation

## Overview

This project demonstrates a structured approach to Red Team operations and documentation through attack-technique documentation, attack-flow visualization, operational task tracking, and Rules of Engagement (RoE).

The activities were performed in an authorized and isolated lab environment using **Metasploitable2** as the target system.

## Objectives

* Document Red Team attack techniques and methodology.
* Visualize an attack path from reconnaissance to post-exploitation.
* Create and apply an operational checklist for a controlled assessment.
* Document attack activities and completion status.
* Define Rules of Engagement for a mock Red Team engagement.
* Maintain clear and structured security documentation.

## Tools Used

* **HackMD** – Attack technique documentation
* **Draw.io** – Attack-flow visualization
* **Trello** – Red Team checklist and task tracking
* **Google Docs** – Rules of Engagement documentation
* **Metasploitable2** – Vulnerable lab environment
* **Nmap** – Network reconnaissance and service enumeration
* **Metasploit Framework** – Controlled exploitation and access validation

---

# Activities

## 1. Technique Summary

Documented a Metasploit-based exploitation technique in HackMD against an authorized Metasploitable2 target.

The documentation covers the objective, target, vulnerability, exploit, payload, exploitation process, initial access, access validation, impact, and remediation.

### Red Team Terms Used

* **Reconnaissance**
* **Exploit**
* **Payload**
* **Initial Access**
* **Post-Exploitation**
* **Persistence** — documented as a Red Team concept and not implemented in the lab

### Vulnerability Documented

**CVE-2011-2523 — VSFTPD 2.3.4 Backdoor**

The exercise demonstrated controlled exploitation of the vulnerable FTP service and validation of the resulting access.

---

## 2. Attack Flowchart

Created an attack-flow diagram in Draw.io to represent the Red Team attack path used during the assessment.

### Attack Flow

```text
Target
   ↓
Reconnaissance
   ↓
Service Enumeration
   ↓
FTP :21/TCP
VSFTPD 2.3.4
   ↓
Vulnerability Identification
CVE-2011-2523
   ↓
Exploitation
Metasploit
   ↓
Payload / Session Establishment
   ↓
Initial Access
   ↓
Command Execution
   ↓
Access Validation
getuid
```

The flowchart represents the progression from target identification and reconnaissance through exploitation and access validation.

**Diagram:** `Attack-Flowchart/attack-flowchart.png`

---

## 3. Checklist Creation

Created a Red Team operational checklist in Trello and applied it to the Metasploitable2 assessment.

The checklist was used to organize and track activities across:

* Reconnaissance
* Service Enumeration
* Vulnerability Identification
* Exploitation
* Initial Access
* Post-Exploitation
* Evidence Collection
* Documentation and Reporting

Completion status was recorded in Trello as the assessment progressed.

---

## 4. Rules of Engagement (RoE)

A Rules of Engagement (RoE) document was prepared to define the scope, objectives, authorized activities, limitations, and operational boundaries for the simulated Red Team assessment.

Engagement Scope
Target: Metasploitable 2 virtual machine

Target IP: 192.168.229.129

Environment: Isolated and authorized laboratory environment


Assessment Objective: Demonstrate controlled exploitation of the VSFTPD 2.3.4 vulnerability (CVE-2011-2523).

Reconnaissance: Network and service enumeration using Nmap.

Exploitation: Controlled exploitation using the Metasploit Framework.

Access Validation: Verification of the established session and security context using getuid.

Impact Assessment: Evaluate the potential security impact without performing destructive actions.

Authorized Activities
Network and service reconnaissance.
Vulnerability identification and analysis.
Controlled exploitation of the identified vulnerability.
Session establishment and access validation.
Collection of screenshots and relevant technical evidence.
Documentation of findings, impact, and remediation recommendations.
Restrictions
Testing was restricted exclusively to the authorized Metasploitable 2 target.
Data destruction or intentional modification of system data was prohibited.
Persistence mechanisms were not implemented.
Lateral movement to other systems was not performed.
Activities affecting systems outside the defined scope were prohibited.
Testing was limited to the isolated laboratory environment.
Evidence & Reporting

Relevant screenshots, technical observations, exploitation results, and access-validation evidence were documented for assessment purposes. Findings were recorded with appropriate impact and remediation recommendations.

Safety and Authorization

All activities were conducted within an authorized and isolated laboratory environment. The assessment was designed to demonstrate Red Team techniques while maintaining defined operational and safety boundaries.

The RoE served as the governing framework for the simulated engagement and ensured that all testing activities remained within the approved scope.

---

# Project Structure

```text
Red-Team-Operations-and-Documentation/
│
├── README.md
│
├── Technique-Summary/
│   ├── Report.md
│   └── screenshots/
│
├── Attack-Flowchart/
│   └── attack-flowchart.png
│
├── Operational-Checklist/
│   └── Trello-Checklist.md
│
└── Rules-of-Engagement/
    └── RoE.md
```

# Key Outcome

This project demonstrates a controlled Red Team workflow covering reconnaissance, service enumeration, vulnerability identification, exploitation, initial access, access validation, operational task tracking, attack-flow visualization, and engagement planning.

All activities were performed against an authorized and isolated laboratory environment.

# Conclusion

The project combines technical attack documentation with operational planning and visualization. It demonstrates how Red Team activities can be systematically documented, tracked, and presented while maintaining defined engagement boundaries through Rules of Engagement.
