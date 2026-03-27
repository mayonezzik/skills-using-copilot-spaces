# Risk Register Template

Use this template to track project risks and dependencies throughout the project lifecycle. Maintain it as a living document and review it at every weekly delivery sync.

Referenced by: [Project Planning](../octoacme-project-planning.md) | [Risk Management & Communication](../octoacme-risks-and-communication.md)

---

## [Project Name] — Risk Register

| ID | Date Identified | Description | Category | Impact (H/M/L) | Likelihood (H/M/L) | Risk Score | Owner (DRI) | Mitigation Plan | Contingency Plan | Status | Last Updated |
|----|-----------------|-------------|----------|----------------|--------------------|------------|-------------|-----------------|------------------|--------|--------------|
| R-001 | YYYY-MM-DD | Brief description of risk | Schedule / Scope / Technical / Resource / External | H / M / L | H / M / L | (see scoring below) | [Name] | Steps to reduce likelihood or impact | What to do if risk materializes | Open / Mitigated / Closed / Accepted | YYYY-MM-DD |

---

## Risk Score Guide

| Impact \ Likelihood | High | Medium | Low |
|---------------------|------|--------|-----|
| **High**            | 🔴 Critical | 🔴 High | 🟡 Medium |
| **Medium**          | 🔴 High | 🟡 Medium | 🟢 Low |
| **Low**             | 🟡 Medium | 🟢 Low | 🟢 Very Low |

- 🔴 **Critical / High** — escalate immediately; requires active mitigation plan
- 🟡 **Medium** — monitor weekly; assign owner and mitigation steps
- 🟢 **Low** — log and monitor; revisit monthly

---

## Risk Categories
- **Schedule** — risks that may delay milestones or release dates
- **Scope** — risks related to expanding or unclear requirements
- **Technical** — architecture, integration, or technical debt risks
- **Resource** — staffing, skill gaps, or third-party availability
- **External** — regulatory, vendor, or market risks

---

## Risk Lifecycle

1. **Identify** — surface during planning, standups, or retrospectives
2. **Assess** — determine impact and likelihood; assign risk score
3. **Assign Owner (DRI)** — one named person responsible for tracking and mitigation
4. **Mitigate** — execute mitigation steps; update the register
5. **Monitor** — review at weekly sync; update status
6. **Close** — mark closed when risk is resolved or accepted with full awareness

---

## Escalation Triggers

See [Risk Management & Communication](../octoacme-risks-and-communication.md#escalation-paths) for full escalation guidance.

| Trigger | Action |
|---------|--------|
| Risk score becomes 🔴 Critical | Escalate to PM immediately; update stakeholders in next status report |
| Mitigation plan not actionable within 1 week | Escalate to Product Lead (Level 2) |
| Risk threatens project timeline > 1 sprint | Sponsor-level escalation (Level 3); update Project One-pager |

---

*Template version: 1.0 — Store this register alongside the [Project One-Pager](../templates/project-one-pager-template.md).*
