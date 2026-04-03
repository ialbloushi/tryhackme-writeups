# SOC Level 1 – Systems as Attack Vectors (TryHackMe)

> Understanding how attackers exploit systems, vulnerabilities, and misconfigurations to gain access.

## Overview

This room focused on systems as attack vectors and how attackers target infrastructure instead of humans.

It explained how vulnerabilities and misconfigurations can lead to serious security breaches, even without user interaction.

---

## Definition of Systems

A system can be a physical server, virtual machine, or cloud platform where data is stored and processed.

If attackers compromise a system, the impact depends on its importance. For example:

* A personal device → Limited impact
* An admin machine → Access to internal systems
* A mail server → Access to thousands of accounts
* A core server → Full network compromise

### Key Insight

* Attacks can happen **without human interaction**
* A single compromised system can lead to **major damage**

---

## Attacks on Systems

Most attacks start by gaining access to a system, then the attacker executes their objective.

### Common Attack Methods

* **Weak Passwords**
  Reusing or using simple passwords increases the risk of compromise

* **Malicious Devices (e.g., USB Rubber Ducky)**
  Automatically executes malicious commands when plugged in

* **Exploiting Vulnerabilities**
  Attackers use known flaws in software to gain access

* **Supply Chain Attacks**
  Malware is introduced through trusted software or dependencies

### Key Terms

* **Vulnerability:** A security flaw that can be exploited
* **Supply Chain Attack:** Compromising trusted software to infect many systems

### Key Insight

* Systems are often the initial entry point for attackers
* Weak security practices increase the risk of compromise

---

## Software Vulnerabilities

All software contains flaws, but some are more critical than others.

### Important Concepts

* **Zero-Day Vulnerability**
  A vulnerability discovered before a patch is available

* **CVE (Common Vulnerabilities and Exposures)**
  A unique ID assigned to publicly known vulnerabilities

### Examples

* EternalBlue (SMB vulnerability)
* PrintNightmare (Windows Print Spooler vulnerability)
* Follina (Microsoft Office vulnerability)

### Responding to Vulnerabilities

* **Patch (Update the system)**

Additional measures include:

* Restricting access to trusted IPs
* Applying temporary mitigations
* Blocking attack patterns using firewalls or WAFs

### Key Insight

* Vulnerabilities are inevitable in software
* Regular patching is critical to reduce risk

---

## Misconfigurations

Misconfigurations are security mistakes in system setup, not software bugs.

### Examples

* Weak passwords (e.g., "1111")
* Unrestricted access
* Disabled or misconfigured security controls

### Real Impact

Even a secure system can be compromised if configured incorrectly.

### Responding to Misconfigurations

* **Penetration Testing**
  Simulates attacks to identify weaknesses

* **Vulnerability Scanning**
  Detects outdated or insecure configurations

* **Configuration Audits**
  Ensures systems follow security best practices

### Key Insight

* Misconfigurations are common and dangerous
* They require **proper configuration**, not patches

---

## Practical Simulation

In this task, I interacted with a simulated SOC environment focused on system security.

### Actions Performed

* Reviewed systems at risk
* Identified vulnerabilities and misconfigurations
* Applied mitigation strategies
* Updated and secured system configurations

---

## Investigation Results

* **Systems at Risk Flag:** THM{patch_or_reconfigure}
* **Remediation Plan Flag:** THM{best_systems_defender}

---

## Key Learnings

This lab expanded my understanding of how systems are targeted in cybersecurity.

I gained hands-on experience in:

* Identifying system vulnerabilities
* Understanding supply chain attacks
* Recognizing misconfigurations
* Applying mitigation and patching strategies

---

## Personal Reflection

This lab showed me that not all attacks rely on human mistakes — systems themselves can be the weakest point.

What stood out most is how a single vulnerability or misconfiguration can lead to full system compromise. It highlighted the importance of patching, proper configuration, and continuous monitoring.

This lab strengthened my understanding of blue team responsibilities in protecting infrastructure, not just users.
