# SOC Level 1 – Alert Reporting (TryHackMe)

> Hands-on SOC simulation focused on alert reporting, escalation, and communication.

## Overview

This room focused on what happens after alert triage within a SOC environment.

It explained how a Junior Security Analyst handles alerts by writing reports, escalating incidents, and communicating with other teams.

The lab also included practical interaction with a simulated SOC dashboard.

---

## Alert Funnel

The SOC workflow follows a structured pipeline to handle alerts efficiently.

### Flow Explanation

* **L1 Analysts:**
  Handle large volumes of alerts and perform initial triage

* **L2 Analysts:**
  Investigate escalated alerts and confirm true positives

* **DFIR Team:**
  Handles incident response, forensics, and advanced threats

### Key Insight

* Alerts are filtered through multiple layers
* The goal is to reduce noise and focus on real threats

---

## Alert Reporting

Before escalating an alert, proper documentation is required.

### Purpose of Reporting

* Provide context for L2 analysts
* Reduce investigation time
* Preserve important evidence
* Improve analytical and reporting skills

### Key Insight

* A clear report improves investigation efficiency
* Poor documentation can delay response

---

## Report Format (5W Method)

A well-written report follows the 5Ws:

* **Who:** The user or account involved
* **What:** The suspicious activity
* **When:** The time of the event
* **Where:** The source (IP, device, or URL)
* **Why:** The reasoning behind the verdict

### Key Insight

* Structured reporting ensures consistency
* The 5W method simplifies investigations

---

## Practical Simulation

In this task, I interacted with a simulated SOC environment.

### Actions Performed

* Reviewed the alert details
* Identified suspicious email activity
* Analysed user and sender information
* Submitted an alert report

### Key Insight

* Clear reporting is essential before escalation
* Accurate analysis improves SOC decision-making

---

## Investigation Results

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

### Key Insight

* Escalation ensures proper handling of incidents
* Critical alerts require higher-level investigation

---

## Escalation Results

* **Assigned L2 Analyst:** E. Fleming
* **First Flag:** THM{good_job_escalating_your_first_alert}
* **Second Flag:** THM{looks_like_webshell_via_old_exchange}

### Key Insight

* Proper escalation ensures incidents are handled by the right team
* Clear reporting supports faster investigation at higher levels

---

## SOC Communication

Communication is critical in SOC operations.

### Key Scenarios

* Escalate to higher levels if L2 is unavailable
* Validate suspicious activity with users securely
* Prioritize alerts during high-volume situations
* Report mistakes immediately
* Report system issues such as SIEM failures

### Key Insight

* Effective communication improves incident response
* Coordination between teams is essential

---

## Communication Results

* **Contact Manager First:** No
* **Report Missed Attack to L2:** Yes

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

What stood out most is how important clear reporting and communication are. A well-written report helps speed up investigations and improves collaboration between teams.

The escalation process also highlighted the importance of teamwork within a SOC environment.

Overall, this room helped me better understand how real SOC operations function beyond basic alert handling.
