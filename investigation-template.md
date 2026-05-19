# SOC Investigation Template

This template is used for all SOC-style security investigations in this repository.

It represents a consistent workflow for triaging alerts, analyzing logs, and determining incident severity in alignment with organization-defined SOPs (or runbooks) and SLA-driven prioritization.

---

## 1. Alert Triage
- What triggered the alert?
- What user/system is involved?
- Is this expected or unusual behavior?
- Initial triage performed following SOC procedures

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
- Is this a single event or repeated behavior?
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
- Severity aligned with SLA requirements where applicable

---

## 8. Recommended Actions
- Account disable / password reset
- IP blocking
- MFA enforcement
- Escalation to incident response team
- Monitoring for recurrence
- Actions executed or recommended in accordance with SOC procedures

---

## 9. Analyst Notes
- Additional observations
- Uncertainties or gaps
- Follow-up actions if needed

---

## 10. Operational Context

In SOC environments, analysts frequently encounter high volumes of alerts across multiple systems and clients. Many alerts may appear repetitive or low-risk, requiring effective prioritization to manage alert fatigue.

Case handling and closure decisions should be based on:
- Matching entities (user, IP, host, timestamp)
- Confirming event correlation across logs
- Determining whether the alert aligns with known patterns or existing incidents
- Adherence to SOC procedures and escalation guidelines

When uncertainty exists, escalation or additional validation is preferred over premature closure in accordance with standard SOC operating practices.