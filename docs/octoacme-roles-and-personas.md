# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

**Abbreviations used in this document:**
- **PM** — Project Manager
- **PdM** — Product Manager (also called Product Lead)
- **DRI** — Directly Responsible Individual (the single named owner accountable for an outcome)
- **QA** — Quality Assurance
- **DevOps** — Development Operations
- **SRE** — Site Reliability Engineering

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

### Interactions with Other Roles
- Works with **PdM** to clarify acceptance criteria and prioritization
- Coordinates with **PM** on timeline estimates and blockers
- Collaborates with **QA/Testing** on test coverage and defect resolution
- Partners with **Tech Lead** on architectural decisions

---

## Product Managers (PdM)

### Role Summary
Product Managers (PdM) define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

### Interactions with Other Roles
- Aligns with **PM** on delivery timelines, scope, and risk
- Partners with **UX Designer** on user research and design decisions
- Works with **Developers** and **Tech Lead** on feasibility trade-offs
- Reports outcomes to **Stakeholder/Sponsor**

---

## Project Managers (PM)

### Role Summary
Project Managers (PM) coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication
- Assign a **DRI** for each backlog item, risk, and action item

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates (see [Weekly Status Update Template](templates/weekly-status-update-template.md))
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

### Interactions with Other Roles
- Works with **PdM** on scope and priority alignment
- Coordinates **Scrum Master** on ceremony facilitation
- Escalates to **Stakeholder/Sponsor** when Level 2/3 escalation thresholds are reached
- Collaborates with **DevOps/SRE** on release readiness

---

## QA / Testing

### Role Summary
QA/Testing professionals validate that delivered features meet acceptance criteria, quality standards, and user expectations. They are the final quality gate before release.

### Responsibilities
- Review acceptance criteria during planning and flag ambiguities early
- Design and execute test plans (manual and/or automated)
- Report, track, and verify defects
- Sign off on features as part of the [Definition of Done](checklists/definition-of-done-checklist.md)
- Support regression testing and smoke tests before each release
- Contribute to the continuous improvement of test automation coverage

### Goals
- Prevent defect leakage to production
- Reduce cost of quality by catching issues early
- Build confidence in each release through repeatable, documented testing

### Typical Communication
- Coordinates with **Developers** on bug reproduction and test coverage
- Provides QA sign-off to **PM** before release deployment
- Reviews acceptance criteria with **PdM** before sprint start
- Flags quality risks in the [Risk Register](checklists/risk-register-template.md)

### Interactions with Other Roles
- Partners with **Developers** on unit/integration test coverage
- Works with **DevOps/SRE** on CI test pipeline configuration
- Aligns with **PdM** to confirm user acceptance

---

## Scrum Master / Agile Coach

### Role Summary
The Scrum Master (or Agile Coach) facilitates agile ceremonies, removes impediments, and coaches the team on best practices. They focus on team health and process effectiveness rather than direct delivery.

### Responsibilities
- Facilitate sprint planning, daily standups, sprint reviews, and retrospectives
- Identify and remove blockers and impediments
- Coach the team on agile principles and continuous improvement
- Track team velocity and highlight process inefficiencies
- Promote psychological safety and open communication

### Goals
- Enable a self-organizing, high-performing team
- Maximize flow and minimize waste
- Protect team focus from unplanned interruptions

### Typical Communication
- Facilitates all agile ceremonies (see [Meeting Notes Template](templates/meeting-notes-template.md))
- Reports team health and impediment status to **PM**
- Collaborates with **PM** to align sprint goals with project milestones

### Interactions with Other Roles
- Works with **PM** to coordinate sprint cadence and milestone alignment
- Partners with **PdM** to maintain a healthy, well-understood backlog
- Supports **Developers** in adopting engineering best practices

---

## UX Designer

### Role Summary
UX Designers ensure that features are usable, accessible, and aligned with user needs. They translate requirements into designs and prototypes that guide development.

### Responsibilities
- Conduct user research and usability testing
- Create wireframes, mockups, and interactive prototypes
- Define and maintain design standards and component libraries
- Review implemented features for design fidelity before QA sign-off
- Incorporate accessibility requirements into all designs

### Goals
- Deliver intuitive, accessible experiences that users value
- Reduce rework caused by late-stage design changes
- Bridge user needs with technical constraints

### Typical Communication
- Collaborates with **PdM** during discovery and requirement definition
- Reviews designs with **Developers** during implementation
- Participates in sprint demos to gather stakeholder feedback

### Interactions with Other Roles
- Works with **PdM** to translate user research into prioritized features
- Partners with **Developers** on implementation feasibility
- Coordinates with **QA/Testing** on usability acceptance criteria

---

## DevOps / SRE

### Role Summary
DevOps/SRE engineers own the reliability, delivery pipeline, and operational health of services. They bridge development and operations to enable safe, frequent deployments.

**DevOps** focuses on CI/CD pipelines, infrastructure automation, and developer experience. **SRE** (Site Reliability Engineering) focuses on service reliability, observability, and incident response.

### Responsibilities
- Design and maintain CI/CD pipelines and deployment automation
- Manage infrastructure provisioning and configuration
- Define and monitor Service Level Objectives (SLOs) and alerting
- Lead incident response and post-incident reviews
- Support the release process per the [Release & Deployment Guide](octoacme-release-and-deployment.md)
- Enforce security and compliance controls in the pipeline

### Goals
- Maximize deployment frequency while minimizing change failure rate
- Achieve reliability targets (SLOs)
- Reduce mean time to recovery (MTTR) for incidents

### Typical Communication
- Coordinates with **Developers** on deployment and infrastructure requirements
- Partners with **Security Champion** on pipeline security controls
- Provides release readiness confirmation to **PM**
- Participates in post-incident blameless retrospectives

### Interactions with Other Roles
- Works with **Developers** on build, test, and deployment automation
- Coordinates with **QA/Testing** on test pipeline orchestration
- Collaborates with **Security Champion** on infrastructure security
- Reports operational risks to **PM** via the [Risk Register](checklists/risk-register-template.md)

---

## Security Champion

### Role Summary
The Security Champion is a team member (often a Developer, DevOps, or Tech Lead) who advocates for security best practices, reviews for vulnerabilities, and acts as the first line of defense for security concerns.

### Responsibilities
- Review code and architecture for security vulnerabilities
- Ensure security scanning is integrated in CI/CD (e.g., SAST, dependency scanning)
- Track and prioritize security findings in the backlog
- Stay current on relevant threat landscape and communicate risks to the team
- Coordinate with external security teams during audits or incidents

### Goals
- Embed security into the development process ("shift left")
- Reduce the cost of fixing security issues by catching them early
- Ensure compliance with organizational and regulatory security requirements

### Typical Communication
- Reviews PRs for security concerns alongside **Developers**
- Coordinates with **DevOps/SRE** on pipeline security controls
- Escalates critical security risks to **PM** and **Stakeholder/Sponsor** immediately

### Interactions with Other Roles
- Partners with **Developers** on secure coding practices
- Works with **DevOps/SRE** on infrastructure and pipeline security
- Reports security risks to **PM** using the [Risk Register](checklists/risk-register-template.md) with appropriate escalation

---

## Tech Lead / Engineering Lead

### Role Summary
The Tech Lead (or Engineering Lead) provides technical direction and architectural guidance. They are the DRI for technical decisions and ensure the codebase stays maintainable and scalable.

### Responsibilities
- Define technical direction and architecture for the project
- Review and approve significant technical decisions (logged in [Decision Log](templates/decision-log-template.md))
- Mentor developers and facilitate technical knowledge sharing
- Balance technical debt reduction with feature delivery
- Represent engineering perspective in cross-functional discussions
- Ensure the team's technical approach aligns with organizational standards

### Goals
- Maintain a healthy, evolvable codebase
- Unblock developers and reduce technical risk
- Enable the team to deliver at a sustainable pace

### Typical Communication
- Technical design reviews and architecture decision records
- Code review guidance and mentorship
- Represents engineering in planning sessions with **PM** and **PdM**

### Interactions with Other Roles
- Works with **PM** and **PdM** to surface technical risks and trade-offs
- Guides **Developers** on architectural patterns and code quality
- Partners with **DevOps/SRE** on infrastructure and deployment architecture
- Collaborates with **Security Champion** on technical security standards

---

## Stakeholder / Sponsor

### Role Summary
Stakeholders and Sponsors are individuals or groups with a vested interest in the project's outcome. The **Sponsor** is the executive champion who authorizes the project and provides escalation authority. **Stakeholders** are broader groups (e.g., sales, support, customers) who are impacted by or provide input to the project.

### Responsibilities
- Provide strategic direction and business context
- Approve the Project One-pager and major scope changes
- Participate in milestone reviews and key demos
- Make decisions on escalated blockers (Level 3 escalation)
- Communicate project outcomes to their respective teams or customers

### Goals
- Ensure the project delivers expected business value
- Maintain organizational alignment and support
- Enable the team with resources and decision-making authority

### Typical Communication
- Monthly stakeholder updates (or milestone-based)
- Briefings on major risks and decisions via [Decision Log](templates/decision-log-template.md)
- Approvals on Project One-pager and major scope changes

### Interactions with Other Roles
- Receives status updates from **PM** via [Weekly Status Update](templates/weekly-status-update-template.md)
- Provides approval and sponsorship to **PdM** for roadmap priorities
- Acts as the final escalation authority for **PM** and **PdM**

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Refer to individual templates and checklists linked throughout this document for concrete tooling each role uses.

