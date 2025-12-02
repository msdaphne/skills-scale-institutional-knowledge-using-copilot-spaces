# OctoAcme Project Management Guide

Welcome to OctoAcme's project management documentation! This guide provides new and existing team members with clarity on how projects are executed at OctoAcme and how institutional knowledge is maintained using Copilot Spaces.

## Purpose

This README serves as the central hub for understanding OctoAcme's project management processes, workflows, and best practices. Whether you're joining the team or need a refresher, this guide will help you navigate our approach to delivering high-quality software.

## Quick Start

- **New to OctoAcme?** Start with [Project Lifecycle](#project-lifecycle-phases) to understand how we run projects
- **Starting a new project?** See [Project Initiation](octoacme-project-initiation.md)
- **Need to understand roles?** Check [Key Personas & Roles](#key-personas--roles)
- **Looking for communication guidelines?** Jump to [Communication & Escalation](#communication--escalation)

---

## Project Lifecycle Phases

OctoAcme projects follow a five-phase lifecycle designed for iterative delivery and continuous improvement:

### 1. Initiation
**Goal:** Validate the business need and authorize work to proceed

- Define problem statement and measurable outcomes
- Identify stakeholders and champions
- Create Project One-pager with success metrics
- Establish high-level timeline and key milestones
- Assess initial risks and resource needs
- **Decision Gate:** Move to planning when success metrics are clear and stakeholders agree on priority

📄 **Details:** [Project Initiation Guide](octoacme-project-initiation.md)

### 2. Planning
**Goal:** Turn approved initiatives into actionable plans and backlogs

- Hold kickoff meeting with stakeholders and delivery team
- Break work into shippable increments with acceptance criteria
- Estimate scope (T-shirt sizing or story points)
- Define Definition of Done (DoD)
- Identify dependencies and integration points
- Create release plan and milestone map
- Develop initial test plan and QA approach

📄 **Details:** [Project Planning](octoacme-project-planning.md)

### 3. Execution
**Goal:** Build, test, and iterate toward project milestones

- Follow team rhythm: daily standups, weekly syncs, sprint/milestone demos
- Use project boards (GitHub Projects) with clear workflow states
- Implement small PRs with clear acceptance criteria
- Run automated tests and security scans in CI
- Track velocity, burndown, and success metrics
- Escalate blockers promptly through defined paths

📄 **Details:** [Execution & Tracking](octoacme-execution-and-tracking.md)

### 4. Release & Deployment
**Goal:** Deliver features to production with minimal risk

- Ensure all acceptance criteria are met
- Complete pre-release requirements (passing CI, security scans, release notes)
- Deploy to staging and run smoke tests
- Execute production deployment with verification
- Follow rollback plan if issues arise
- Announce release to stakeholders and support teams

📄 **Details:** [Release & Deployment Guide](octoacme-release-and-deployment.md)

### 5. Retrospective & Continuous Improvement
**Goal:** Capture learnings and convert them into actionable improvements

- Conduct retrospectives after each sprint, release, or milestone
- Discuss what went well and what could be improved
- Create 2-3 prioritized action items with owners and due dates
- Track improvements in project backlog
- Measure impact and celebrate successes

📄 **Details:** [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)

---

## Structured Workflows

### Project Boards
- Use GitHub Projects with columns: Backlog → Ready → In Progress → In Review → QA → Done
- Link issues to project boards for visibility
- Update status daily during standups

### Templates & Artifacts
- **Project One-pager:** Problem, goal, success metrics, stakeholders, timeline, risks
- **Backlog Items:** Title, description, acceptance criteria, priority, estimate, owner
- **Release Notes:** Release name, date, summary, notable changes, migration steps
- **Risk Register:** ID, description, impact, likelihood, owner, mitigation, status

### Team Rhythm
- **Daily Standups (15 min):** Progress, blockers, dependencies
- **Weekly Delivery Sync:** Show progress, updates, flagged risks
- **Sprint/Milestone Demos:** Demonstrate working features to stakeholders
- **Monthly Stakeholder Updates:** High-level progress and roadmap alignment

### Incident Response
- Trigger incident response for critical production issues
- Notify on-call and follow rollback procedures if needed
- Conduct blameless post-incident retrospective
- Document root cause and action items

### Dashboards & Metrics
- Track velocity and burndown charts
- Monitor success metrics from Project One-pager
- Use dashboards for key signals: errors, latency, usage, test coverage

---

## Key Personas & Roles

OctoAcme projects involve cross-functional collaboration across these key roles:

### Project Manager (PM)
**Coordinates delivery activities, manages schedules, risks, and communications**

- Creates and maintains project plans and timelines
- Manages risks, dependencies, and resource constraints
- Facilitates meetings (kickoff, planning, retrospectives)
- Ensures consistent documentation and status reporting
- Coordinates cross-team and stakeholder communication

### Product Manager (PdM)
**Defines what should be built to deliver customer and business value**

- Defines problem statements and success metrics
- Prioritizes roadmap and backlog
- Collaborates on trade-offs with stakeholders and engineering
- Validates solutions through user research and metrics
- Owns product vision and market fit

### Developers
**Design, build, test, and deliver software components**

- Implement features to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Identify technical risks and propose mitigations

### QA/Testing
**Validate quality and acceptance criteria**

- Develop and execute test plans
- Perform manual testing when needed
- Validate end-to-end flows and critical paths
- Report defects and verify fixes
- Collaborate on acceptance criteria

### Stakeholders
**Provide inputs, approvals, and feedback**

- Define business requirements and constraints
- Review progress and provide feedback
- Approve key decisions and releases
- Champion initiatives across the organization

### Role Interactions
- **PM ↔ PdM:** Weekly alignment on priorities, risks, and roadmap
- **Developers ↔ QA:** Continuous collaboration on testability and quality
- **PM ↔ Stakeholders:** Regular updates and escalation when needed
- **PdM ↔ Stakeholders:** Gather requirements and validate solutions

📄 **Details:** [Roles & Personas](octoacme-roles-and-personas.md)

---

## Communication & Escalation

### Communication Cadence

| Activity | Frequency | Participants | Purpose |
|----------|-----------|--------------|---------|
| Daily Standups | Daily (15 min) | Delivery team | Progress, blockers, dependencies |
| PM + PdM Sync | Weekly | PM, PdM | Alignment on priorities and risks |
| Delivery Sync | Weekly | PM, Dev leads, QA | Progress updates, flagged risks |
| Stakeholder Updates | Monthly | PM, PdM, stakeholders | High-level progress and roadmap |
| Sprint/Milestone Demos | End of sprint/milestone | All team members, stakeholders | Demonstrate working features |
| Retrospectives | After sprint/release | Delivery team | Capture learnings and improvements |

### Weekly Status Template
- **Progress this week:** Key accomplishments and completed items
- **Next steps:** Planned work for upcoming week
- **Risks & blockers:** Issues requiring attention
- **Ask / decisions needed:** Items needing stakeholder input

### Escalation Paths

#### Standard Escalation
1. **Level 1 (Team-level):** Triage in daily standup
2. **Level 2 (PM Escalation):** PM escalates to Product Lead and dependent teams
3. **Level 3 (Sponsor-level):** Escalation for business-impacting issues

#### Security Incidents
- Follow security incident runbook
- Notify Security on-call immediately
- Conduct post-incident review with security team

#### Production Incidents
- Trigger incident response protocol
- Notify on-call and stakeholders
- Execute rollback if necessary
- Document in incident log
- Schedule blameless retrospective

📄 **Details:** [Risk Management & Communication](octoacme-risks-and-communication.md)

---

## Quality Assurance Practices

### Continuous Integration (CI)
- All PRs run automated tests before merge
- Security scanning integrated into CI pipeline
- Linting and code style checks enforced
- Build verification on multiple environments
- Require passing CI before code review completion

### Testing Strategy
- **Unit Tests:** Test individual functions and components
- **Integration Tests:** Verify interactions between components
- **End-to-End Tests:** Validate critical user flows
- **Smoke Tests:** Quick validation after deployments
- **Manual QA:** Feature acceptance testing when needed

### Code Review Standards
- Small PRs (≤ 400 lines when possible)
- Include issue link and acceptance criteria in PR description
- At least one approval required before merging (or team-defined policy)
- Review for security, performance, and maintainability
- Ensure tests cover new code paths

### Quality Metrics
- **Test Coverage:** Track coverage trends over time
- **Defect Rate:** Monitor bugs found in production vs. testing
- **Cycle Time:** Measure time from commit to production
- **Build Success Rate:** Track CI pipeline stability
- **Performance Metrics:** Monitor latency, error rates, resource usage

### Definition of Done (DoD)
Before marking work as complete, ensure:
- Acceptance criteria met and verified
- Code reviewed and approved
- Tests written and passing
- Documentation updated
- Security scans passing
- Deployed to staging and smoke tested

---

## Living Documentation & Institutional Knowledge

### Why Living Documentation Matters

At OctoAcme, we believe that **knowledge should be accessible, up-to-date, and actionable**. Living documentation ensures:

- New team members can onboard quickly
- Processes evolve based on learnings
- Institutional knowledge survives team changes
- Decisions are traceable and reversible
- Best practices are consistently applied

### Using Copilot Spaces

OctoAcme leverages **GitHub Copilot Spaces** to scale institutional knowledge:

- **Contextual Assistance:** Documentation in `.copilot/` directories provides context to Copilot
- **Role-Based Guidance:** Use persona definitions to get role-specific recommendations
- **Process Automation:** Copilot helps generate templates and boilerplate following our standards
- **Knowledge Discovery:** Quickly find relevant processes and examples
- **Consistency:** Ensure all team members follow the same patterns

### Maintaining Documentation

- Keep Project Charter and key artifacts in the project repository
- Add process-specific docs to `.copilot/` for Copilot Spaces context
- Update documentation during retrospectives
- Review and refresh quarterly
- Archive outdated processes with explanatory notes

### Documentation Structure

```
docs/
├── README.md (this file)
├── octoacme-project-management-overview.md
├── octoacme-project-initiation.md
├── octoacme-project-planning.md
├── octoacme-execution-and-tracking.md
├── octoacme-release-and-deployment.md
├── octoacme-retrospective-and-continuous-improvement.md
├── octoacme-risks-and-communication.md
└── octoacme-roles-and-personas.md
```

---

## Core Principles

Our project management approach is guided by these principles:

- **Customer-first:** Prioritize customer value and usability in all decisions
- **Iterative delivery:** Deliver small, testable increments frequently
- **Clear ownership:** Each project has named PM and Product Lead
- **Data-informed decisions:** Measure impact and iterate based on evidence
- **Psychological safety:** Encourage feedback, learning, and experimentation
- **Transparency:** Maintain clear, accessible communication with all stakeholders
- **Continuous improvement:** Learn from every project and refine our processes

---

## Getting Help

- **Questions about processes?** Start with this README and linked documentation
- **Project-specific questions?** Contact the Project Manager listed in the Project One-pager
- **Technical guidance?** Reach out to development leads or use Copilot Spaces
- **Escalations?** Follow the [escalation paths](#escalation-paths) defined above

---

## Related Documentation

- [Project Management Overview](octoacme-project-management-overview.md) - High-level principles and scope
- [Project Initiation](octoacme-project-initiation.md) - Starting new projects
- [Project Planning](octoacme-project-planning.md) - Creating actionable plans
- [Execution & Tracking](octoacme-execution-and-tracking.md) - Day-to-day delivery
- [Release & Deployment](octoacme-release-and-deployment.md) - Shipping to production
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) - Learning and improving
- [Risk Management & Communication](octoacme-risks-and-communication.md) - Managing risks and stakeholder communication
- [Roles & Personas](octoacme-roles-and-personas.md) - Team roles and responsibilities

---

**Last Updated:** December 2025  
**Maintained by:** OctoAcme Project Management Team  
**Feedback:** Submit issues or PRs to improve this documentation
