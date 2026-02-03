# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - **Security Lead** reviews security-sensitive changes
  - Require at least one approval before merging (or team-defined policy)
  - **Developer** addresses review feedback and ensures CI passes
  - Upon merge, notify **QA/Test Engineer** for validation

## Quality & Testing

### Testing Responsibilities by Role
- **Developers**: Write unit and integration tests; ensure tests pass before PR submission
- **QA/Test Engineers**: Create test plans, execute regression testing, perform exploratory testing, and sign off on feature acceptance
- **Security Lead**: Configure and monitor security scanning tools; review scan results and triage vulnerabilities
- **SRE/DevOps**: Maintain test environments and CI/CD pipelines; ensure deployment smoke tests run successfully

### Testing Process
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI (SAST, DAST, dependency checks)
- Manual QA for feature acceptance when needed

### QA-to-Deployment Handoff Checklist
- [ ] All acceptance criteria validated by **QA/Test Engineer**
- [ ] Regression tests executed and passing
- [ ] Security scans reviewed and approved by **Security Lead**
- [ ] Test results documented and shared with **Project Manager**
- [ ] Deployment readiness confirmed with **SRE/DevOps**
- [ ] Known issues and edge cases documented in release notes
- [ ] Rollback procedure validated in staging environment

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation

### Escalation Path by Role
- **Developers**: Escalate technical blockers to tech lead or architect; dependency issues to **Project Manager**
- **QA/Test Engineers**: Escalate quality concerns or insufficient acceptance criteria to **Product Manager**
- **SRE/DevOps**: Escalate infrastructure or operational risks to **Project Manager** and affected stakeholders
- **Security Lead**: Escalate critical security vulnerabilities immediately to **Project Manager** and leadership

### Escalation Levels
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Security scanning integrated into CI pipeline (**Security Lead**)
- [ ] Test environments provisioned and accessible (**SRE/DevOps**)
- [ ] QA test plan documented and approved (**QA/Test Engineer**)
- [ ] Design specifications finalized (**UX/UI Designer**)
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] Cross-role handoff processes understood by all team members

---

*Related to Issue #5: Expanded role definitions and handoff processes - https://github.com/masam23/skills-scale-institutional-knowledge-using-copilot-spaces/issues/5*
