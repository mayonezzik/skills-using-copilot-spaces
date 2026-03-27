# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Ownership & DRI Assignment
Every backlog item, risk, and action item must have a single **DRI** (Directly Responsible Individual) — one named person who is accountable for driving that item to completion. DRIs are assigned during sprint planning and reviewed at each weekly delivery sync. If a DRI cannot be identified, the PM resolves this before the item enters "In Progress".

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks; use [Weekly Status Update Template](templates/weekly-status-update-template.md)
- Demo/Review at the end of each sprint or milestone
- Capture meeting outcomes using the [Meeting Notes Template](templates/meeting-notes-template.md)

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed
- All items must meet the [Definition of Done Checklist](checklists/definition-of-done-checklist.md) before being marked Done

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
Escalation levels apply when blockers are not resolved within their expected window:

| Level | Trigger | Action |
|-------|---------|--------|
| **Level 1** | Blocker identified; can be resolved within 1–2 days | DRI resolves in daily standup; PM tracks |
| **Level 2** | Unresolved after 1–2 days; milestone at risk within current sprint | PM escalates to Product Lead and dependent teams; log in status update |
| **Level 3** | Issue threatens project timeline > 1 sprint; business-impacting | PM escalates to Sponsor; log decision in [Decision Log](templates/decision-log-template.md) |

See [Risk Management & Communication](octoacme-risks-and-communication.md#escalation-paths) for the full escalation path and additional triggers.

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly (see [Risk Register Template](checklists/risk-register-template.md))
- [ ] DRI assigned for every active backlog item and risk
- [ ] Decision log maintained for significant choices (see [Decision Log Template](templates/decision-log-template.md))
