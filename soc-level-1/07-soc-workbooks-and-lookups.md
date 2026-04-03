# SOC Level 1 – SOC Workbooks and Lookups (TryHackMe)

> Discovering how SOC analysts use workbooks and lookup data (identity, assets, and network diagrams) to improve alert triage and investigation.

## Overview

This room focused on how SOC analysts gather context using internal resources such as identity inventory, asset inventory, and network diagrams.

It also introduced SOC workbooks, which provide structured workflows to ensure consistent and accurate alert investigation.

---

## Identity & Asset Context

To properly investigate alerts, analysts must understand both the user and the system involved.

### Identity Inventory

Identity inventory contains information about users and accounts within the organisation.

Examples include:

* Active Directory (on-prem / Azure AD)
* SSO providers (Okta, Google Workspace)
* HR systems (BambooHR, SAP)
* Custom solutions (CSV / Excel)

### Key Insight

* Helps identify user roles and access levels
* Provides context for suspicious activity

---

### Asset Inventory

Asset inventory contains information about systems and devices in the environment.

Examples include:

* Active Directory
* SIEM / EDR tools (Elastic, CrowdStrike)
* MDM solutions (Intune, Jamf)
* Custom asset tracking systems

### Key Insight

* Helps understand what systems store or process
* Critical for determining impact of an alert

---

## Investigation Scenario

In this task, an alert involved a user downloading a financial report from a server.

### Findings

* **User Role:** US Financial Adviser
* **Server Data:** Financial records
* **Legitimacy:** Yes (expected behaviour)

### Key Insight

* Context determines whether activity is malicious or normal
* Not all alerts indicate threats

---

## Network Diagrams

Network diagrams help analysts understand infrastructure and traffic flow.

### Investigation Flow

* External attacker performed VPN brute force
* Gained access through VPN
* Attempted to scan database subnet
* Moved laterally to office subnet

### Findings

* **Exposed Service (TCP/10443):** VPN
* **Target Subnet:** Database subnet
* **Verdict:** True Positive

### Key Insight

* Network visibility is critical for detecting lateral movement
* Helps reconstruct attacker behaviour

---

## SOC Workbooks

SOC workbooks (playbooks/runbooks) are structured guides used during investigations.

They ensure:

* Consistent analysis
* No missed steps
* Faster decision making

### Investigation Stages

* **Enrichment:** Gather context (user, IP, host)
* **Investigation:** Analyse logs and activity
* **Escalation:** Send to L2 if needed

### Findings

* **Role using workbooks most:** SOC L1 Analyst
* **Context gathering process:** Enrichment
* **Identity source example:** BambooHR

### Key Insight

* Workbooks standardise investigations
* Essential for junior analysts

---

## Practical Simulation

In this task, I applied SOC workbook steps in a simulated investigation environment.

### Actions Performed

* Used identity inventory to verify user details
* Checked asset inventory for system context
* Analysed network activity using diagrams
* Applied workbook stages (Enrichment → Investigation → Escalation)

### Flags

* THM{the_most_common_soc_workbook}
* THM{be_vigilant_with_powershell}
* THM{asset_inventory_is_essential}

### Key Insight

* Structured workflows significantly improve investigation accuracy
* Combining multiple data sources leads to better decision-making

---

## Key Learnings

This room enhanced my understanding of how SOC analysts use internal data sources and structured workflows.

I gained hands-on experience in:

* Using identity and asset inventory
* Understanding network diagrams
* Analysing real-world attack scenarios
* Applying SOC workbooks in investigations

---

## Personal Reflection

This lab showed how important context is in SOC investigations.

What stood out most is how multiple data sources (users, assets, network) come together to form a complete picture.

It also highlighted that structured workflows like workbooks are essential for consistency, especially for L1 analysts.

This lab strengthened my ability to investigate alerts using real-world SOC methodologies.
