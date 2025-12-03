# OctoAcme — Communication & Collaboration Templates

## Purpose
Standardized templates to ensure clear, consistent communication across all team members and stakeholders, improving transparency and alignment.

---

## Weekly Status Update Template

**For:** Project Managers, Team Leads
**Audience:** Stakeholders, Team Members
**Frequency:** Weekly

### Progress This Week
- [List key accomplishments]
- [Features completed]
- [Milestones reached]

### Next Steps (Upcoming Week)
- [Planned work items]
- [Key deliverables]
- [Important meetings or decisions]

### Risks & Blockers
| Risk/Blocker | Impact | Owner | Status | Mitigation |
|--------------|--------|-------|--------|------------|
| [Description] | High/Med/Low | [Name] | [Status] | [Plan] |

### Asks / Decisions Needed
- [Item requiring stakeholder input]
- [Decision points]
- [Resource needs]

### Metrics Update
- [Success metric 1]: [Current value] (Target: [Target value])
- [Success metric 2]: [Current value] (Target: [Target value])

---

## Sprint Planning Summary Template

**For:** Project Managers, Scrum Masters
**Audience:** Team Members, Stakeholders
**Frequency:** Start of each sprint

### Sprint Goal
[Clear, concise statement of what this sprint aims to achieve]

### Sprint Duration
Start Date: [Date]
End Date: [Date]

### Team Capacity
- Total story points/hours available: [Number]
- Planned vacation/out-of-office: [List]
- Adjusted capacity: [Number]

### Committed Work Items
| Item | Type | Assignee | Priority | Estimate | Acceptance Criteria Link |
|------|------|----------|----------|----------|--------------------------|
| [Title] | Feature/Bug/Task | [Name] | High/Med/Low | [Points/Hours] | [Link] |

### Dependencies
- [Dependency description] - Owner: [Name] - Due: [Date]

### Risks Identified
- [Risk description] - Mitigation: [Plan]

---

## Daily Standup Template

**For:** All Team Members
**Audience:** Team Members
**Frequency:** Daily (15 minutes)
**Format:** Asynchronous (written) or Synchronous (meeting)

### What I completed yesterday/since last update
- [Task 1]
- [Task 2]

### What I'm working on today
- [Task 1]
- [Task 2]

### Blockers or help needed
- [Blocker description] - Need help from: [Name/Role]
- None

---

## Design Review Request Template

**For:** UX/UI Designers
**Audience:** Product Managers, Developers, Stakeholders

### Design Context
**Feature/Problem:** [Brief description]
**User Story:** [Link to user story or description]
**Design Goal:** [What this design aims to achieve]

### Design Artifacts
- Wireframes: [Link]
- Mockups: [Link]
- Prototype: [Link]
- Design specs: [Link]

### User Research Insights
- [Key finding 1]
- [Key finding 2]
- [Link to full research]

### Design Decisions & Rationale
- **Decision:** [Description]
  - **Rationale:** [Why this approach]
  - **Alternatives considered:** [Other options]

### Accessibility Considerations
- [How design meets accessibility standards]
- [WCAG compliance notes]

### Technical Constraints
- [Known limitations]
- [Integration considerations]

### Feedback Requested
- [ ] Overall design direction
- [ ] Specific interaction pattern
- [ ] Visual design details
- [ ] Accessibility review
- [ ] Technical feasibility

### Review Deadline
[Date] - Needed by this date to support development timeline

---

## Technical Design Document Template

**For:** Developers, DevOps Engineers
**Audience:** Team Members, Technical Stakeholders

### Problem Statement
[What problem does this solve? Why now?]

### Goals & Non-Goals
**Goals:**
- [Goal 1]
- [Goal 2]

**Non-Goals:**
- [What this does NOT address]

### Proposed Solution
[High-level description of the approach]

### Design Details
- **Architecture:** [Diagrams, components]
- **API Design:** [Endpoints, contracts]
- **Data Model:** [Schema, relationships]
- **Infrastructure:** [Services, resources]

### Security Considerations
- [Authentication/authorization]
- [Data protection]
- [Vulnerability mitigation]

### Performance & Scalability
- [Expected load]
- [Scaling strategy]
- [Performance benchmarks]

### Testing Strategy
- Unit tests: [Approach]
- Integration tests: [Approach]
- E2E tests: [Approach]

### Rollout Plan
- Phase 1: [Description, timeline]
- Phase 2: [Description, timeline]

### Monitoring & Alerts
- [Metrics to track]
- [Alert conditions]

### Rollback Strategy
[How to revert if issues arise]

### Open Questions
- [Question 1] - Owner: [Name]
- [Question 2] - Owner: [Name]

### Decision Log
| Date | Decision | Rationale | Owner |
|------|----------|-----------|-------|
| [Date] | [Decision] | [Why] | [Name] |

---

## Code Review Checklist Template

**For:** Developers
**Audience:** Code Reviewers

### Before Requesting Review
- [ ] Code follows team style guide and conventions
- [ ] All tests pass locally
- [ ] New tests added for new functionality
- [ ] Documentation updated (code comments, README, API docs)
- [ ] Security considerations addressed
- [ ] PR description includes context and acceptance criteria
- [ ] Issue/ticket linked in PR
- [ ] Self-review completed

### Reviewer Checklist
- [ ] Code is clear and maintainable
- [ ] Logic is correct and handles edge cases
- [ ] Tests adequately cover changes
- [ ] No obvious security vulnerabilities
- [ ] Performance implications considered
- [ ] Breaking changes documented
- [ ] Error handling is appropriate
- [ ] Documentation is clear and accurate

---

## Security Review Request Template

**For:** Security Leads, Developers
**Audience:** Security Team, Stakeholders

### Change Summary
[Brief description of the change]

### Security Impact Analysis
**Data Handling:**
- [ ] New data storage introduced
- [ ] Sensitive data processed
- [ ] Data classification: [Public/Internal/Confidential/Restricted]

**Authentication & Authorization:**
- [ ] New authentication mechanism
- [ ] Authorization changes
- [ ] Privilege escalation possible

**External Interfaces:**
- [ ] New API endpoints
- [ ] Third-party integrations
- [ ] Network exposure changes

**Known Vulnerabilities:**
- [List any identified vulnerabilities and mitigation plans]

### Threat Model
- **Assets:** [What needs protection]
- **Threats:** [Potential attack vectors]
- **Mitigations:** [Security controls in place]

### Compliance Requirements
- [ ] GDPR considerations
- [ ] SOC 2 requirements
- [ ] Industry-specific regulations: [List]

### Security Testing Completed
- [ ] Static analysis (SAST)
- [ ] Dependency scanning
- [ ] Dynamic testing (DAST)
- [ ] Penetration testing (if applicable)

### Remediation Plan
| Vulnerability | Severity | Remediation | Owner | Due Date | Status |
|---------------|----------|-------------|-------|----------|--------|
| [Description] | Critical/High/Med/Low | [Plan] | [Name] | [Date] | [Status] |

---

## Incident Communication Template

**For:** DevOps Engineers, Project Managers, Security Leads
**Audience:** Stakeholders, Affected Users

### Initial Notification

**Subject:** [Service] Incident - [Brief Description]

**Status:** Investigating / Identified / Monitoring / Resolved

**Impact:** [Description of user/business impact]

**Affected Services/Features:** [List]

**Start Time:** [Timestamp]

**Current Actions:**
- [Action 1]
- [Action 2]

**Next Update:** [Expected time]

---

### Update Notification

**Subject:** [Service] Incident Update - [Brief Description]

**Status:** Investigating / Identified / Monitoring / Resolved

**Update:** [What has changed since last update]

**Current Actions:**
- [Action 1]
- [Action 2]

**Next Update:** [Expected time]

---

### Resolution Notification

**Subject:** [Service] Incident Resolved - [Brief Description]

**Status:** Resolved

**Resolution:** [What fixed the issue]

**Impact Duration:** [Start time] to [End time] ([Duration])

**Root Cause:** [Brief explanation]

**Next Steps:**
- [ ] Post-incident review scheduled for [Date]
- [ ] Monitoring for recurrence
- [ ] Action items to prevent future occurrences

**Apology & Appreciation:** [If applicable]

---

## Customer Feedback Summary Template

**For:** Customer Support Liaisons, Product Managers
**Audience:** Product Team, Stakeholders
**Frequency:** Weekly or as needed

### Feedback Period
[Start Date] to [End Date]

### Summary Metrics
- Total tickets: [Number]
- Average resolution time: [Duration]
- Customer satisfaction: [Score/Percentage]
- Escalations: [Number]

### Top Issues
| Issue | Frequency | Severity | Status |
|-------|-----------|----------|--------|
| [Description] | [Count] | High/Med/Low | [Status] |

### Feature Requests
| Request | Frequency | Business Value | Requester Segment |
|---------|-----------|----------------|-------------------|
| [Description] | [Count] | High/Med/Low | [Segment] |

### Positive Feedback
- [Highlight 1]
- [Highlight 2]

### Recommended Actions
- [Action 1] - Owner: [Name] - Priority: [High/Med/Low]
- [Action 2] - Owner: [Name] - Priority: [High/Med/Low]

### Trending Topics
- [Topic 1]: [Trend direction and context]
- [Topic 2]: [Trend direction and context]

---

## Retrospective Meeting Template

**For:** All Team Members
**Audience:** Team Members
**Frequency:** After sprint, release, or milestone

### Retrospective Details
**Date:** [Date]
**Facilitator:** [Name]
**Participants:** [Names]
**Sprint/Project:** [Name]

### What Went Well
- [Positive item 1]
- [Positive item 2]
- [Positive item 3]

### What Could Be Improved
- [Improvement area 1]
- [Improvement area 2]
- [Improvement area 3]

### Action Items from Previous Retrospective
| Action | Owner | Status | Notes |
|--------|-------|--------|-------|
| [Action] | [Name] | Done/In Progress/Blocked | [Notes] |

### New Action Items
| Action | Owner | Due Date | Success Criteria | Priority |
|--------|-------|----------|------------------|----------|
| [Action] | [Name] | [Date] | [How we'll know it's done] | High/Med/Low |

### Appreciations
- [Appreciation 1]
- [Appreciation 2]

---

## Release Communication Template

**For:** Product Managers, Technical Writers
**Audience:** All Stakeholders, End Users

### Release Announcement

**Release:** [Version/Name]
**Date:** [Release Date]
**Type:** Major / Minor / Patch

### What's New
- **[Feature 1]:** [Description and benefit]
- **[Feature 2]:** [Description and benefit]

### Improvements
- [Improvement 1]
- [Improvement 2]

### Bug Fixes
- [Fix 1]
- [Fix 2]

### Breaking Changes
- [Change 1] - Migration guide: [Link]

### Deprecations
- [Deprecated feature] - End of support: [Date] - Alternative: [Recommendation]

### Documentation
- [Link to updated docs]
- [Link to migration guide]
- [Link to API changes]

### Getting Help
- [Support channel]
- [FAQ link]
- [Contact information]

---

## Related Documentation
- [Communication Cadence](octoacme-risks-and-communication.md)
- [Project Management Overview](octoacme-project-management-overview.md)
- [Roles & Personas](octoacme-roles-and-personas.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
