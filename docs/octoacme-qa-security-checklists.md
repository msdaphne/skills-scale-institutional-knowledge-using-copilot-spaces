# OctoAcme — QA & Security Review Checklists

## Purpose
Comprehensive checklists to ensure quality and security standards are met throughout the development lifecycle, from planning through deployment.

---

## Feature Planning QA Checklist

**When:** During feature planning and backlog grooming
**Owner:** Product Manager, QA Lead

- [ ] Acceptance criteria are clear, testable, and measurable
- [ ] Definition of Done includes quality requirements
- [ ] Test strategy defined (unit, integration, E2E, manual)
- [ ] Test data requirements identified
- [ ] Test environment needs documented
- [ ] Performance requirements specified (if applicable)
- [ ] Accessibility requirements defined
- [ ] Security requirements identified
- [ ] Edge cases and error scenarios documented
- [ ] Backwards compatibility considerations noted
- [ ] Rollback scenarios considered

---

## Development QA Checklist

**When:** During active development
**Owner:** Developers

### Code Quality
- [ ] Code follows team style guide and conventions
- [ ] Code is modular, readable, and maintainable
- [ ] Appropriate error handling implemented
- [ ] Edge cases handled properly
- [ ] No hardcoded credentials or sensitive data
- [ ] Logging implemented for debugging and monitoring
- [ ] Performance optimization applied where needed
- [ ] Code comments added for complex logic

### Testing
- [ ] Unit tests written for new functionality
- [ ] Test coverage meets team standards (e.g., 80%+)
- [ ] Integration tests added for component interactions
- [ ] Existing tests still pass
- [ ] Tests are meaningful and test actual functionality
- [ ] Test names clearly describe what they test
- [ ] Mock/stub dependencies appropriately
- [ ] Tests run quickly (under X seconds)

### Documentation
- [ ] Code documentation (docstrings, comments) updated
- [ ] README updated if setup/usage changed
- [ ] API documentation updated
- [ ] Configuration changes documented
- [ ] Migration scripts documented (if applicable)

---

## Pull Request QA Checklist

**When:** Before and during code review
**Owner:** Developer (PR Author), Reviewers

### PR Preparation (Author)
- [ ] PR title and description are clear and descriptive
- [ ] Issue/ticket linked in PR description
- [ ] Acceptance criteria referenced or included
- [ ] Breaking changes clearly called out
- [ ] Screenshots/recordings included for UI changes
- [ ] Deployment notes added if needed
- [ ] All CI checks passing
- [ ] Self-review completed
- [ ] Conflicts resolved with target branch

### Code Review (Reviewer)
- [ ] Code logic is correct and solves the stated problem
- [ ] Code is maintainable and follows best practices
- [ ] Security vulnerabilities addressed (see Security Checklist)
- [ ] Tests adequately cover the changes
- [ ] Documentation is clear and complete
- [ ] Performance implications considered
- [ ] Error handling is appropriate
- [ ] No unnecessary code changes (stay focused on the issue)
- [ ] Naming conventions followed
- [ ] Dependencies are necessary and up-to-date

### Approval Criteria
- [ ] At least one approval from qualified reviewer
- [ ] All CI/CD checks passing
- [ ] No unresolved comments or concerns
- [ ] Security review completed (if required)
- [ ] QA team notified if manual testing required

---

## Pre-Deployment QA Checklist

**When:** Before deploying to staging or production
**Owner:** QA Team, DevOps Engineer

### Test Execution
- [ ] All automated tests passing in CI/CD
- [ ] Smoke tests executed successfully
- [ ] Integration tests verified
- [ ] E2E tests completed for critical paths
- [ ] Performance tests executed (if applicable)
- [ ] Load tests completed (for high-traffic features)
- [ ] Security scans passing
- [ ] Accessibility tests completed

### Environment Readiness
- [ ] Deployment window scheduled (if required)
- [ ] Staging environment mirrors production
- [ ] Database migrations tested in staging
- [ ] Configuration changes validated
- [ ] Feature flags configured correctly
- [ ] Monitoring and alerts configured
- [ ] Rollback plan documented and tested

### Documentation & Communication
- [ ] Release notes drafted and reviewed
- [ ] Deployment runbook updated
- [ ] Stakeholders notified of deployment
- [ ] Customer Support briefed on changes
- [ ] Known issues documented
- [ ] Support documentation updated

---

## Post-Deployment QA Checklist

**When:** Immediately after deployment
**Owner:** DevOps Engineer, QA Team

- [ ] Smoke tests run in production environment
- [ ] Critical user flows verified manually
- [ ] Monitoring dashboards show healthy metrics
- [ ] No error rate spikes in logs
- [ ] Performance metrics within acceptable range
- [ ] Database migrations completed successfully
- [ ] Feature flags activated as planned
- [ ] Rollback tested (if safe to do so)
- [ ] Stakeholders notified of successful deployment
- [ ] Customer Support has access to updated documentation

---

## Security Planning Checklist

**When:** During feature planning and design
**Owner:** Security Lead, Product Manager

- [ ] Security requirements identified and documented
- [ ] Data classification determined (public, internal, confidential, restricted)
- [ ] Authentication and authorization requirements defined
- [ ] Data encryption requirements specified (in transit, at rest)
- [ ] Compliance requirements identified (GDPR, HIPAA, SOC 2, etc.)
- [ ] Third-party integrations reviewed for security
- [ ] API security requirements defined
- [ ] Threat modeling completed for complex features
- [ ] Security testing strategy defined
- [ ] Privacy impact assessment completed (if handling PII)

---

## Development Security Checklist

**When:** During active development
**Owner:** Developers, Security Lead

### Secure Coding Practices
- [ ] Input validation implemented for all user inputs
- [ ] Output encoding applied to prevent injection attacks
- [ ] Authentication and authorization properly implemented
- [ ] Sensitive data encrypted in transit (HTTPS/TLS)
- [ ] Sensitive data encrypted at rest (where applicable)
- [ ] No secrets, API keys, or passwords in code
- [ ] Secure random number generation used for security purposes
- [ ] SQL injection prevention (parameterized queries)
- [ ] XSS prevention (input sanitization, CSP headers)
- [ ] CSRF protection implemented
- [ ] Session management follows best practices
- [ ] Rate limiting applied to prevent abuse

### Dependencies & Libraries
- [ ] All dependencies are from trusted sources
- [ ] Dependencies are up-to-date with security patches
- [ ] Vulnerability scanning run on dependencies
- [ ] Unused dependencies removed
- [ ] License compatibility verified
- [ ] Dependency pinning configured

### Access Control
- [ ] Principle of least privilege applied
- [ ] Role-based access control (RBAC) implemented correctly
- [ ] Admin functions properly protected
- [ ] Sensitive operations require additional authentication
- [ ] Access logs capture security-relevant events

---

## Code Review Security Checklist

**When:** During code review
**Owner:** Security Lead, Reviewers

- [ ] No hardcoded credentials, API keys, or secrets
- [ ] User input properly validated and sanitized
- [ ] Authentication and authorization logic correct
- [ ] Sensitive data handled securely
- [ ] No SQL injection vulnerabilities
- [ ] No XSS vulnerabilities
- [ ] No CSRF vulnerabilities
- [ ] No path traversal vulnerabilities
- [ ] No insecure deserialization
- [ ] Proper error handling (no sensitive info in errors)
- [ ] Logging doesn't include sensitive data
- [ ] Cryptographic functions used correctly
- [ ] Random number generation is cryptographically secure
- [ ] Session management is secure
- [ ] Rate limiting and throttling in place
- [ ] Security headers configured (CSP, HSTS, etc.)

---

## Pre-Deployment Security Checklist

**When:** Before deploying to production
**Owner:** Security Lead, DevOps Engineer

### Security Scanning
- [ ] Static Application Security Testing (SAST) completed
- [ ] Dynamic Application Security Testing (DAST) completed
- [ ] Dependency vulnerability scanning completed
- [ ] Container image scanning completed (if applicable)
- [ ] Infrastructure as Code (IaC) security scanning completed
- [ ] Secrets scanning completed (no secrets in code)
- [ ] All critical and high vulnerabilities remediated
- [ ] Medium vulnerabilities assessed and accepted/remediated

### Configuration & Infrastructure
- [ ] Security groups/firewall rules reviewed and minimized
- [ ] Unnecessary ports and services disabled
- [ ] TLS/SSL certificates valid and properly configured
- [ ] Security headers configured (HSTS, CSP, X-Frame-Options, etc.)
- [ ] CORS policy properly restrictive
- [ ] Database access properly restricted
- [ ] Secrets management solution configured (not in env vars)
- [ ] Logging and monitoring capture security events
- [ ] Backup and disaster recovery tested

### Compliance & Documentation
- [ ] Compliance requirements verified (GDPR, HIPAA, etc.)
- [ ] Privacy policy updated (if handling new data types)
- [ ] Data retention policies implemented
- [ ] Security documentation updated
- [ ] Incident response procedures documented
- [ ] Security training completed by team (if new risks)

---

## Production Security Monitoring Checklist

**When:** Ongoing after deployment
**Owner:** Security Lead, DevOps Engineer

### Monitoring & Alerting
- [ ] Security event logging enabled and monitored
- [ ] Failed authentication attempts monitored
- [ ] Unusual access patterns detected
- [ ] Rate limiting violations logged
- [ ] Security alerts configured and tested
- [ ] Intrusion detection system (IDS) active
- [ ] Web application firewall (WAF) logs reviewed

### Vulnerability Management
- [ ] Automated vulnerability scanning scheduled
- [ ] Security advisories monitored for dependencies
- [ ] Patch management process followed
- [ ] Penetration testing scheduled (annually or as required)
- [ ] Bug bounty program active (if applicable)
- [ ] Vulnerability disclosure process documented

### Incident Response
- [ ] Security incident response plan documented
- [ ] Incident response team identified and trained
- [ ] Security contact information published
- [ ] Incident log maintained
- [ ] Post-incident reviews conducted

---

## Accessibility QA Checklist

**When:** During development and before release
**Owner:** UX/UI Designer, Developers, QA Team

### WCAG 2.1 Level AA Compliance
- [ ] Perceivable: Content can be perceived by all users
  - [ ] Text alternatives for non-text content (alt text)
  - [ ] Captions and transcripts for audio/video
  - [ ] Content is adaptable (semantic HTML)
  - [ ] Sufficient color contrast (4.5:1 for normal text)
  - [ ] Text can be resized up to 200% without loss of functionality
- [ ] Operable: Users can navigate and operate the interface
  - [ ] All functionality available via keyboard
  - [ ] No keyboard traps
  - [ ] Adequate time limits or ability to extend them
  - [ ] No content that flashes more than 3 times per second
  - [ ] Skip navigation links provided
  - [ ] Descriptive page titles and link text
- [ ] Understandable: Content and operation are understandable
  - [ ] Language of page specified
  - [ ] Navigation is consistent
  - [ ] Form inputs have labels
  - [ ] Error messages are clear and helpful
  - [ ] Context changes are predictable
- [ ] Robust: Content works with assistive technologies
  - [ ] Valid HTML markup
  - [ ] ARIA labels used appropriately
  - [ ] Tested with screen readers (NVDA, JAWS, VoiceOver)

### Testing Tools
- [ ] Automated accessibility testing tool run (axe, Lighthouse, WAVE)
- [ ] Manual keyboard navigation tested
- [ ] Screen reader testing completed
- [ ] Color contrast verified
- [ ] Responsive design tested at different zoom levels

---

## Performance QA Checklist

**When:** Before release of performance-sensitive features
**Owner:** Developers, QA Team, DevOps Engineer

### Performance Testing
- [ ] Page load time meets targets (e.g., < 3 seconds)
- [ ] Time to interactive (TTI) measured and optimized
- [ ] API response times within SLA (e.g., p95 < 500ms)
- [ ] Database query performance optimized
- [ ] Load testing completed for expected traffic
- [ ] Stress testing completed to identify breaking points
- [ ] Resource usage monitored (CPU, memory, disk)

### Optimization
- [ ] Images optimized and properly sized
- [ ] CSS and JavaScript minified
- [ ] Caching strategy implemented
- [ ] CDN configured for static assets
- [ ] Database indexes optimized
- [ ] N+1 query problems resolved
- [ ] Lazy loading implemented where appropriate
- [ ] Bundle size monitored and kept reasonable

---

## Documentation Quality Checklist

**When:** Before publishing or updating documentation
**Owner:** Technical Writer

- [ ] Documentation is accurate and up-to-date
- [ ] Language is clear and concise
- [ ] Examples are working and relevant
- [ ] Screenshots are current and helpful
- [ ] Step-by-step instructions are complete
- [ ] Prerequisites clearly stated
- [ ] Troubleshooting section included
- [ ] Links are valid and not broken
- [ ] Consistent terminology used throughout
- [ ] Grammar and spelling checked
- [ ] Accessibility guidelines followed (alt text, headings, etc.)
- [ ] Feedback mechanism available for users

---

## Continuous Improvement

After each release or milestone:
- [ ] Review checklist effectiveness
- [ ] Identify gaps or missing items
- [ ] Update checklists based on lessons learned
- [ ] Share improvements with team
- [ ] Track metrics on defects found vs. missed

## Related Documentation
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- [Communication Templates](octoacme-communication-templates.md)
- [Roles & Personas](octoacme-roles-and-personas.md)
