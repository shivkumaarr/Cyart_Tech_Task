# Red Team Operations and Documentation

## Overview

This project demonstrates a structured approach to Red Team operations and documentation through attack-technique documentation, attack-flow visualization, operational checklists, and Rules of Engagement (RoE).

The activities were performed in an authorized and isolated lab environment using **Metasploitable2** as the target system.

## Objectives

* Document Red Team attack techniques and methodology.
* Visualize an attack path from reconnaissance to post-exploitation.
* Create a repeatable Red Team operational checklist.
* Apply the checklist to a controlled Metasploitable2 attack.
* Draft Rules of Engagement for a mock Red Team engagement.
* Maintain structured documentation of activities, findings, and outcomes.

## Tools Used

* **HackMD** – Attack technique documentation
* **Draw.io** – Attack-flow visualization
* **Trello** – Operational checklist and task tracking
* **Google Docs** – Rules of Engagement documentation
* **Metasploitable2** – Authorized vulnerable lab environment
* **Nmap** – Network reconnaissance and service enumeration
* **Metasploit Framework** – Controlled exploitation and access validation

---

# Activities

## 1. Technique Summary

Documented a Metasploit-based exploitation technique in HackMD against an authorized Metasploitable2 target.

The documentation covers the attack objective, target, vulnerability, exploit, payload, exploitation process, initial access, access validation, impact, and remediation.

### Red Team Terms Used

* **Reconnaissance**
* **Exploit**
* **Payload**
* **Initial Access**
* **Post-Exploitation**
* **Persistence** *(documented as a Red Team concept; not implemented in the lab)*

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

**Attack Flowchart:** `Attack-Flowchart/attack-flowchart.png`

---

## 3. Checklist Creation

Created a Trello-based Red Team operational checklist and applied it to the Metasploitable2 assessment.

### Checklist Activities

* [x] Identify target system
* [x] Run Nmap reconnaissance
* [x] Enumerate exposed services
* [x] Identify vulnerable service
* [x] Research CVE-2011-2523
* [x] Select appropriate Metasploit exploit
* [x] Configure required options
* [x] Execute the exploit
* [x] Validate initial access
* [x] Document findings
* [x] Record remediation recommendations

The checklist was used to track the completion status of activities and maintain a consistent assessment workflow.

---

## 4. Rules of Engagement (RoE)

Drafted a Rules of Engagement document for a mock Red Team engagement using Google Docs.

### Scope

* **Target:** One authorized virtual machine
* **Environment:** Isolated laboratory
* **Objective:** Demonstrate controlled Red Team techniques
* **Data Destruction:** Not permitted
* **Out-of-Scope:** Systems outside the defined lab target
* **Evidence:** Screenshots and relevant technical observations
* **Safety:** Activities must remain within the authorized environment

The RoE establishes the boundaries, permitted activities, restrictions, and operational requirements for the simulated engagement.

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
│   └── checklist.md
│
└── Rules-of-Engagement/
    └── RoE.md
```

# Key Outcome

This project demonstrates the documentation and execution of a controlled Red Team workflow, including reconnaissance, service enumeration, vulnerability identification, exploitation, initial access, access validation, operational tracking, and engagement planning.

All activities were performed against an authorized and isolated laboratory environment.

# Conclusion

The project combines technical attack documentation with operational planning and visualization. It demonstrates how Red Team activities can be systematically documented, tracked, and presented while maintaining defined engagement boundaries through Rules of Engagement.
