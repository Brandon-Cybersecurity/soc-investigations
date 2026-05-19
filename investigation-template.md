# SOC Investigation Template

This template is used for all SOC-style security investigations in this repository.

It represents a consistent SOC workflow for triaging alerts, analyzing logs, and determining incident severity in alignment with organization-defined SOPs (or runbooks) and SLA-driven prioritization.

---

## 1. Alert Triage
- What triggered the alert?
- What user/system is involved?
- Is this expected or unusual behavior?
- Initial triage performed following SOC SOP guidelines

---

## 2. Initial Log Review
- Authentication logs
- Endpoint logs (if applicable)
- Network/IP context
- Time range of activity

---

## 3. Event Timeline
- Reconstruct sequence of events
- Identify failed vs successful actions
- Note any anomalies in timing or source

---

## 4. Pattern Analysis
- Is this single event or repeated behavior?
- Are there multiple IPs, devices, or locations?
- Any escalation patterns?

---

## 5. Hypothesis
- Brute force attack
- Credential stuffing
- Misconfiguration
- Insider activity
- Benign / false positive

---

## 6. Validation
- What evidence supports the hypothesis?
- What evidence contradicts it?

---

## 7. Severity Assessment
- Low / Medium / High / Critical
- Justification based on impact and confidence
- Severity aligned with SLA definitions where applicable

---

## 8. Recommended Actions
- Account disable / reset password
- IP blocking
- MFA enforcement
- Escalation to IR team
- Monitoring for recurrence
- Actions executed or recommended in accordance with SOC SOPs

---

## 9. Analyst Notes
- Additional observations
- Uncertainties or gaps
- Follow-up actions if needed

---

## 10. Operational Context (SOC I Perspective)

In SOC I environments, especially in MSSP settings, analysts often encounter a high volume of repetitive or similar alerts across multiple clients.

Over time, many alerts may appear to be duplicates or low-risk events, which can contribute to alert fatigue if not managed carefully under SOC procedures.

Case handling and closure decisions should be based on:
- Matching entities (user, IP, host, timestamp)
- Confirming event correlation across logs
- Verifying whether the alert is part of an existing known pattern or incident
- Alignment with SOC SOP guidelines and escalation procedures

When uncertainty exists, escalation or additional validation is preferred over premature closure in accordance with standard SOC operating procedures.