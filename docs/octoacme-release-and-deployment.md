# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (validated by Security Lead)
- Release notes drafted (by Technical Writer)
- Rollback / mitigation plan documented (by Release Manager)
- Smoke tests prepared
- Security review completed for high-risk changes (Security Lead)

## Deployment Checklist
- [ ] Deployment window scheduled by Release Manager (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Security scan results reviewed (Security Lead)
- [ ] Release documentation finalized (Technical Writer)
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support (Release Manager)

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call (Release Manager coordinates)
  - Security Lead assesses if incident has security implications
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items
  - Update documentation with lessons learned (Technical Writer)

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
