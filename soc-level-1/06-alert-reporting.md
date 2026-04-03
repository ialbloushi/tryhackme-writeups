# SOC Level 1 – Alert Reporting (TryHackMe)

> Hands-on SOC simulation focused on alert reporting, escalation, and communication.

## Overview

This room builds on the fundamentals of alert triage by introducing what happens after an alert is classified.

It focuses on how a Junior Security Analyst handles alerts in a real SOC environment, including writing professional reports, escalating incidents, and communicating with other teams.

The lab also includes practical interaction with a simulated SOC dashboard to reinforce these concepts.

---

## Learning Objectives

By completing this room, I learned:

* The importance of alert reporting and escalation in a SOC
* How to write clear and structured alert reports
* Best practices for escalation and communication
* How alerts move through the SOC workflow
* Improved confidence working in a SOC simulation environment

---

## Alert Funnel

The SOC workflow follows a structured pipeline to handle alerts efficiently.

### Flow Explanation

* **L1 Analysts:**
  Handle large volumes of alerts, most of which are false positives, and perform initial triage

* **L2 Analysts:**
  Investigate escalated alerts and confirm true positives

* **DFIR Team:**
  Handles incident response, forensics, and advanced threats

The goal is to filter out noise and focus only on real security incidents.

---

## Alert Reporting

Before escalating an alert, proper documentation is required.

### Purpose of Reporting

* Provide context for L2 analysts
* Reduce investigation time
* Preserve important evidence
* Improve analytical and reporting skills

---

## Report Format (5W Method)

A well-written report follows the 5Ws:

* **Who:** The user or account involved
* **What:** The suspicious activity
* **When:** The time of the event
* **Where:** The source (IP, device, or URL)
* **Why:** The reasoning behind the verdict

---

## Practical Investigation Results

During the simulation, I identified the following:

* **Leaked Email User:** [m.boslan@tryhackme.thm](mailto:m.boslan@tryhackme.thm)
* **Suspicious Email Sender:** [support@microsoft.com](mailto:support@microsoft.com)
* **Flag:** THM{nice_attempt_faking_microsoft_support}

---

## Alert Escalation

Escalation is required when an alert needs deeper analysis or action.

### When to Escalate

* The alert is a True Positive
* Remediation actions are required
* The impact is significant
* Additional expertise is needed

### Actions Performed

* Assigned the alert to an L2 analyst
* Selected the appropriate verdict
* Submitted a detailed report

---

## Escalation Results

* **Assigned L2 Analyst:** E. Fleming
* **First Flag:** THM{good_job_escalating_your_first_alert}
* **Second Flag:** THM{looks_like_webshell_via_old_exchange}

---

## SOC Communication

Communication is critical in SOC operations.

### Key Scenarios

* Escalate to higher levels if L2 is unavailable
* Validate suspicious activity with users securely
* Prioritize alerts during high-volume situations
* Report mistakes immediately
* Report system issues such as SIEM failures

---

## Communication Results

* **Contact Manager First:** Nay
* **Report Missed Attack to L2:** Yea

---

## Key Learnings

This lab provided deeper insight into SOC operations beyond alert triage.

I gained hands-on experience in:

* Writing structured and professional reports
* Applying the 5W methodology
* Escalating alerts correctly
* Understanding the SOC workflow in practice
* Handling communication scenarios within a SOC team

---

## Personal Reflection

This lab showed that alert triage is only the first step in a SOC analyst’s workflow.

The most important takeaway was how critical clear reporting and communication are. A poorly written report can slow down the entire investigation process, even if the alert is correctly identified.

The escalation process also highlighted the importance of teamwork within a SOC environment.

Overall, this room helped me better understand how real SOC operations function beyond basic alert handling.
