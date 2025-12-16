# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — facilitated by Scrum Master, focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone (with UX Designer presenting design updates)
- Sprint retrospectives facilitated by Scrum Master

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
- Security scanning in CI (monitored by Security Lead)
- Manual QA for feature acceptance when needed
- Usability testing coordinated by UX Designer for user-facing features
- Documentation review by Technical Writer before release

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo (by Technical Writer)
- [ ] CI configured for tests, lint, and security scanning (Security Lead)
- [ ] Regular demos scheduled (Scrum Master)
- [ ] Risk register updated weekly (Project Manager with Security Lead input)
- [ ] Design reviews scheduled for user-facing changes (UX Designer)
- [ ] Release coordination established (Release Manager)
