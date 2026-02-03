# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (validated by **Security Lead**)
- QA sign-off completed (**QA/Test Engineer**)
- Release notes drafted (**Product Manager** and **Project Manager**)
- Rollback / mitigation plan documented (**SRE/DevOps**)
- Smoke tests prepared and validated in staging (**QA/Test Engineer** and **SRE/DevOps**)
- Infrastructure capacity confirmed (**SRE/DevOps**)

## Deployment Checklist
- [ ] Deployment window scheduled (if needed) — **Project Manager**
- [ ] Backup or snapshot (if applicable) — **SRE/DevOps**
- [ ] Deploy to staging and run smoke tests — **SRE/DevOps** and **QA/Test Engineer**
- [ ] Final security scan review — **Security Lead**
- [ ] Deploy to production (automated pipeline preferred) — **SRE/DevOps**
- [ ] Run post-deploy verifications — **SRE/DevOps** and **QA/Test Engineer**
- [ ] Monitor error rates and performance metrics — **SRE/DevOps**
- [ ] Announce release to stakeholders and support — **Project Manager** and **Product Manager**

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - **SRE/DevOps** triggers incident response and notifies on-call
  - **Project Manager** coordinates stakeholder communication
  - **SRE/DevOps** rollback to last known-good release if necessary
  - **Developer** and **SRE/DevOps** triage root cause
  - **Security Lead** assesses if incident has security implications
  - **Project Manager** captures action items and schedules postmortem
  - **Product Manager** communicates customer impact and remediation timeline

### Roles in Incident Response
- **SRE/DevOps**: Lead technical response, execute rollback, coordinate recovery
- **Developer**: Debug issues, implement fixes, support root cause analysis
- **QA/Test Engineer**: Validate fixes and regression test before redeployment
- **Security Lead**: Assess security impact, coordinate security response if needed
- **Project Manager**: Manage communications, document timeline, track action items
- **Product Manager**: Assess customer impact, prioritize remediation work

---

*Related to Issue #5: Role-specific release and deployment responsibilities - https://github.com/masam23/skills-scale-institutional-knowledge-using-copilot-spaces/issues/5*

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
