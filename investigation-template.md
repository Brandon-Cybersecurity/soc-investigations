# SOC Investigation Template

This template is used for all SOC-style security investigations in this repository.

It represents a consistent workflow for triaging alerts, analyzing logs, and determining incident severity in alignment with organization-defined SOPs (or runbooks) and SLA-driven prioritization.

This workflow is intended as a flexible investigation reference and does not replace organization-specific SOPs, escalation procedures, or incident response guidance.

---

## 1. Alert Triage
- What triggered the alert?
- What user/system is involved?
- Is this expected or unusual behavior?
- Initial triage performed following SOC procedures

---

## 2. Priority Assessment
- Active compromise indicators
- Successful suspicious authentication
- Privileged account involvement
- Multiple affected systems
- Ongoing malicious activity
- User or business impact
- SLA escalation requirements

---

## 3. Initial Log Review
- Authentication logs
- Endpoint telemetry
- Network/IP context
- Time range of activity

---

## 4. Event Timeline
- Reconstruct sequence of events
- Identify failed vs successful actions
- Note anomalies in timing or source

---

## 5. Pattern Analysis
- Single event or repeated behavior?
- Multiple IPs, devices, or locations?
- Related escalation patterns?

---

## 6. Potential Threat Scenarios
- Brute force attack
- Credential stuffing
- Misconfiguration
- Insider activity
- Benign / false positive

---

## 7. Validation & Correlation
- IOC validation
- Cross-log confirmation
- Entity correlation
- Behavioral consistency
- Environmental context validation

---

## 8. Severity Assessment
- Low / Medium / High / Critical
- Justification based on impact and confidence
- Severity aligned with SLA requirements

---

## 9. Recommended Containment / Escalation Actions
- Recommend account disable or password reset
- Recommend IP blocking where applicable
- MFA enforcement review
- Escalation to incident response team
- Continued monitoring for recurrence

---

## 10. Escalation / Handoff Notes
- Findings requiring follow-up
- Additional enrichment or validation needed
- Pending customer communication
- Shift handoff considerations
- Remaining uncertainties or investigative gaps

---

## 11. Investigation Continuity
- Document findings during active investigations
- Avoid tunnel vision during simultaneous alert handling
- Reconfirm scope when switching client contexts
- Maintain visibility of incoming alerts
- Escalate when confidence is low

---

## 12. Operational Considerations

SOC analysts frequently manage alerts across multiple systems and client environments while balancing investigation depth, prioritization, and alert fatigue.

Case handling decisions should consider:
- Entity correlation across logs
- Existing incidents or known patterns
- Escalation guidelines and SOPs
- Scope and operational impact

## 13. Quick Investigation Reminders

- Slow down before escalating
- Validate before assuming compromise
- Prioritize active threats over alert volume
- Maintain visibility across open investigations
- Avoid tunnel vision during active cases
- Document findings as investigation progresses
- Reconfirm scope when pivoting between entities
- Escalate when confidence is low
- Follow SOPs and escalation guidelines (know your client)
- Investigation quality is more important than rushing queue closure

When uncertainty exists, additional validation or escalation is preferred over premature closure.
