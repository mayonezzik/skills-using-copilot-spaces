# Definition of Done (DoD) Checklist

This checklist defines the minimum conditions that must be satisfied before any backlog item, user story, or task can be marked **Done**. Teams should review and adapt this checklist during project kick-off and record any changes in the [Decision Log](../templates/decision-log-template.md).

Referenced by: [Project Planning](../octoacme-project-planning.md) | [Execution & Tracking](../octoacme-execution-and-tracking.md)

---

## Code Quality
- [ ] Code implements all acceptance criteria defined in the backlog item
- [ ] Code reviewed and approved by at least one peer (pull request approved)
- [ ] No unresolved review comments; all feedback addressed or explicitly deferred
- [ ] Code follows team style guide / linting rules (CI lint check passes)
- [ ] No new critical or high-severity static analysis / security scan findings introduced

## Testing
- [ ] Unit tests written for all new or changed logic
- [ ] Integration tests written or updated where applicable
- [ ] All existing tests pass in CI
- [ ] End-to-end / smoke tests pass for critical flows (if applicable)
- [ ] Manual QA completed for UI or user-facing changes (sign-off from QA/Testing role)
- [ ] Acceptance criteria verified by QA or PdM (Product Manager)

## Documentation
- [ ] Inline code comments added for complex logic
- [ ] Public APIs, configuration options, or user-facing changes documented
- [ ] Relevant process documents updated (if the change affects a workflow)
- [ ] Release notes entry drafted (see [Release Notes Template](../templates/release-notes-template.md))

## Deployment Readiness
- [ ] Feature flag or rollout strategy confirmed (if applicable)
- [ ] Database migrations or infrastructure changes tested in a non-production environment
- [ ] Rollback plan documented or confirmed
- [ ] Monitoring / alerting configured for new functionality (if applicable)

## Ownership & Tracking
- [ ] Backlog item updated to "Done" in the project board
- [ ] A single DRI (Directly Responsible Individual) confirmed as the owner throughout delivery
- [ ] Any outstanding risks or follow-up items captured in the Risk Register or backlog
- [ ] Stakeholders notified of completion (as agreed in the communication plan)

---

## Team-Specific Additions
<!-- Add any project- or team-specific criteria below. Agree on these during project kick-off. -->
- [ ] *(Team-specific item 1)*
- [ ] *(Team-specific item 2)*

---

*Template version: 1.0 — Review and update this checklist at each retrospective.*
