# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies. All risks should have a single **DRI** (Directly Responsible Individual) — the one named person accountable for tracking and driving mitigation.

## Risk Register
Use the [Risk Register Template](checklists/risk-register-template.md) to maintain and track all risks. The template provides a full table structure, risk scoring guide, and escalation triggers.

At a minimum, capture:
- **ID** — unique identifier (e.g., R-001)
- **Description** — concise summary of the risk
- **Impact** (High / Med / Low)
- **Likelihood** (High / Med / Low)
- **Owner (DRI)** — single named person responsible for this risk
- **Mitigation plan** — actions to reduce likelihood or impact
- **Status** — Open / Mitigated / Closed / Accepted

## Risk Lifecycle
- **Identify:** during planning and ongoing execution
- **Assess:** estimate impact and likelihood; assign risk score
- **Assign DRI:** one named owner per risk — no shared or unowned risks
- **Mitigate:** reduced via actions, contingency plans
- **Monitor:** review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based) using the [Weekly Status Update Template](templates/weekly-status-update-template.md)
- Use a single source of truth (project README or release doc) for status

## Communication Templates
Use the [Weekly Status Update Template](templates/weekly-status-update-template.md) for regular progress reports.

For meeting facilitation and action tracking, see the [Meeting Notes Template](templates/meeting-notes-template.md).

**Incident Communication**
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths

Escalation follows three levels based on the scope and severity of the issue:

| Level | Trigger | Who is Involved | Action |
|-------|---------|-----------------|--------|
| **Level 1** | Blocker surfaces in standup; expected resolution within 1–2 days | Team (DRI + Developer/QA) | Resolve in daily standup; DRI tracks resolution |
| **Level 2** | Blocker not resolved within 1–2 days; risk becomes 🔴 High/Critical; milestone at risk by < 1 sprint | PM escalates to Product Lead and dependent teams | PM documents in status update; PdM and Product Lead engaged for priority decisions |
| **Level 3** | Issue threatens project timeline by > 1 sprint; business-impacting incident; security breach | PM escalates to Sponsor/executive stakeholder | Sponsor briefed; formal decision logged in [Decision Log](templates/decision-log-template.md); scope or timeline formally adjusted |

**Additional escalation rules:**
- For **security incidents**, follow the security incident runbook and notify Security on-call immediately (treat as Level 3 regardless of timeline impact).
- Any risk that moves to 🔴 Critical in the Risk Register triggers Level 2 escalation by default.
- The DRI for the risk is responsible for driving escalation — do not wait for the PM to initiate.

