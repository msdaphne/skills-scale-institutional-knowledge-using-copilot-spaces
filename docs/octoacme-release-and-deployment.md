# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (see [Security Checklist](octoacme-qa-security-checklists.md#pre-deployment-security-checklist))
- Release notes drafted (see [Release Communication Template](octoacme-communication-templates.md#release-communication-template))
- Rollback / mitigation plan documented
- Smoke tests prepared (see [Pre-Deployment QA Checklist](octoacme-qa-security-checklists.md#pre-deployment-qa-checklist))
- Accessibility requirements verified for UI changes

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Security verification completed (Security Lead sign-off)
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and Customer Support
- [ ] Update documentation (coordinate with Technical Writer)

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify DevOps/Platform Engineer on-call
  - Notify Customer Support Liaison to coordinate customer communications
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items
  - Conduct post-incident retrospective with Security Lead if security-related
  - Use [Incident Communication Template](octoacme-communication-templates.md#incident-communication-template)

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
