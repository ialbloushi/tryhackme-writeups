SOC Level 1 – Alert Triage (TryHackMe)

```
Understanding SOC alerts, their lifecycle, and how to properly triage them as an L1 analyst.
```

## Overview

This room focused on SOC alerts and how analysts handle them within a Security Operations Center (SOC).

It explained how alerts are generated from events, how they are analysed, and how analysts prioritise and investigate them.

The lab also included a practical simulation using a SOC dashboard to perform real alert triage tasks.

---

## SOC Alerts

An alert is a notification triggered by security systems when suspicious activity is detected.

Alerts are generated from events such as:

```
User logins
File activity
Network traffic
```

Key Insight

```
Not all events are alerts
Alerts highlight suspicious activity that requires investigation
```

---

## From Events to Alerts

Security systems generate large volumes of events, but only some become alerts.

Process:

```
Events are generated from systems
SIEM collects and analyses events
Suspicious activity is converted into alerts
```

Key Insight

```
Alerts reduce noise and focus on threats
Analysts work with alerts, not raw logs
```

---

## Alert Properties

Each alert contains important information required for analysis.

Important Properties

```
Alert Time → When the alert was triggered
Alert Name → Summary of the activity
Severity → Risk level (Low to Critical)
Status → Progress of the alert
Verdict → True Positive or False Positive
Assignee → Analyst responsible
Description → Details of the alert
Fields → Technical data (IP, user, hostname)
```

---

## Alert Prioritisation

When multiple alerts are present, analysts must decide which to handle first.

Common Approach

```
Filter new and unassigned alerts
Prioritise based on severity (Critical → Low)
Start with older alerts first
```

Key Insight

```
High severity alerts are more likely to be real threats
Proper prioritisation improves response time
```

---

## Alert Triage

Alert triage is the process of analysing and handling alerts.

Steps

```
Assign the alert
Move status to In Progress
Review alert details
Investigate activity
Determine verdict
Document findings
Close or escalate
```

Key Insight

```
Triage ensures proper handling of alerts
Documentation is essential for tracking incidents
```

---

## Practical Simulation

In this task, I interacted with a simulated SOC dashboard and performed alert triage.

Actions Performed

```
Reviewed alerts in the dashboard
Analysed alert properties
Prioritised alerts
Assigned and investigated alerts
Determined verdicts
Completed alert triage workflow
```

---

## Investigation Results

```
Number of alerts: 5
Most recent alert: Double Extension File Creation
```

---

## Alert Properties Results

```
Verdict (Unusual VPN Login Location): False Positive
User: M.Clark
```

---

## Alert Prioritisation Results

```
Prioritise medium/low first: Yes
Start with newest alerts: No
First priority alert: Potential Data Exfiltration
```

---

## Alert Triage Flags

```
THM{looks_like_lots_of_zoom_meetings}
THM{how_could_this_user_fall_for_it}
THM{should_we_allow_github_for_devs}
```

---

## Key Learnings

This lab improved my understanding of SOC alert handling.

I gained hands-on experience in:

```
Understanding how alerts are generated
Analysing alert properties
Prioritising alerts
Performing alert triage
Identifying false positives and real threats
```

---

## Personal Reflection

This lab showed how SOC analysts handle alerts in real environments.

What stood out most is how structured the triage process is, from prioritisation to investigation and final decision.

It also highlighted that not every alert is a real threat, and proper analysis is required before making decisions.

This lab strengthened my understanding of blue team operations, especially in alert handling and investigation.
