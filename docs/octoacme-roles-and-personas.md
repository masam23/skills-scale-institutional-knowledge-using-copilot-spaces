# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

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

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

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

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## UX/UI Designers

### Role Summary
UX/UI Designers create intuitive, accessible user experiences and deliver design specifications for implementation. They balance user needs with technical constraints to ensure products are both functional and delightful.

### Responsibilities
- Conduct user research and usability testing
- Create wireframes, mockups, and interactive prototypes
- Define design systems and maintain UI consistency
- Collaborate with Product Managers on feature requirements and user stories
- Work with Developers to ensure designs are implemented as intended
- Validate design implementations and provide feedback during QA

### Goals
- Deliver user-centered designs that meet accessibility standards
- Reduce design-to-implementation friction
- Maintain consistent brand and UX patterns across products
- Improve user satisfaction and task completion rates

### Typical Communication
- Design critiques and stakeholder reviews
- Handoff sessions with Developers (design specs, assets, interaction patterns)
- User research findings and recommendations shared with Product Managers
- Feedback during PR reviews and QA cycles

### Interaction Points with Other Personas
- **Product Managers**: Collaborate on feature requirements, success metrics, and user priorities
- **Developers**: Provide design specifications, review implementations, discuss feasibility
- **QA/Test Engineers**: Define expected UI behavior and validate user flows
- **Project Managers**: Communicate design timeline, dependencies, and risks

---

## QA/Test Engineers

### Role Summary
QA/Test Engineers ensure product quality by designing test strategies, executing comprehensive testing, and validating that features meet acceptance criteria. They act as the final quality gate before release.

### Responsibilities
- Create test plans and test cases based on acceptance criteria
- Execute manual and automated regression tests
- Perform exploratory testing to identify edge cases
- Report and track defects, working with Developers on fixes
- Coordinate release sign-off and validation
- Maintain test documentation and test data
- Support incident investigation and root cause analysis

### Goals
- Prevent defects from reaching production
- Reduce regression risks and improve test coverage
- Shorten feedback cycles between testing and development
- Ensure features meet functional and non-functional requirements

### Typical Communication
- Test plan reviews with Product Managers and Developers
- Daily bug triage and defect status updates
- Release readiness reports for Project Managers
- Test results and quality metrics shared in sprint reviews

### Interaction Points with Other Personas
- **Developers**: Clarify acceptance criteria, report bugs, validate fixes
- **Product Managers**: Validate features against requirements, identify gaps
- **SRE/DevOps**: Coordinate deployment validation and smoke tests
- **Project Managers**: Report on quality status and release readiness
- **UX/UI Designers**: Validate user flows and UI implementations

---

## Site Reliability Engineers (SRE)/DevOps

### Role Summary
Site Reliability Engineers maintain operational excellence by managing infrastructure, deployment pipelines, monitoring, and incident response. They ensure systems are reliable, scalable, and observable.

### Responsibilities
- Design and maintain CI/CD pipelines and deployment automation
- Monitor system health, performance, and availability
- Respond to incidents and coordinate resolution efforts
- Implement and maintain infrastructure as code
- Configure logging, alerting, and observability tools
- Perform capacity planning and scaling activities
- Conduct postmortem reviews and implement preventive measures

### Goals
- Maximize system uptime and reliability
- Reduce deployment cycle time and risk
- Improve mean time to detection (MTTD) and recovery (MTTR)
- Automate operational tasks and eliminate toil

### Typical Communication
- Incident response channels and postmortem reports
- Deployment coordination and release notifications
- Infrastructure health dashboards and SLO reports
- Operational risk assessments shared with Project Managers

### Interaction Points with Other Personas
- **Developers**: Collaborate on deployment strategies, debug production issues
- **QA/Test Engineers**: Support test environment setup and deployment validation
- **Project Managers**: Report infrastructure constraints and operational risks
- **Security Lead**: Implement security controls and respond to security incidents

---

## Security Lead

### Role Summary
Security Leads ensure secure software delivery by assessing risks, implementing security controls, and reviewing code and infrastructure for vulnerabilities. They promote security best practices across the team.

### Responsibilities
- Conduct security reviews of code, design, and architecture
- Perform threat modeling and risk assessments
- Implement and maintain security scanning tools (SAST, DAST, SCA)
- Review and approve security-sensitive changes
- Respond to security incidents and vulnerabilities
- Provide security training and guidance to the team
- Ensure compliance with security policies and standards

### Goals
- Prevent security vulnerabilities from reaching production
- Reduce security incident response time
- Foster a security-aware development culture
- Maintain compliance with security standards and regulations

### Typical Communication
- Security review findings and remediation guidance
- Threat model documentation and risk assessments
- Security incident reports and postmortems
- Security metrics and compliance status reports

### Interaction Points with Other Personas
- **Developers**: Review code for security issues, provide secure coding guidance
- **Project Managers**: Communicate security risks and timeline impacts
- **SRE/DevOps**: Collaborate on secure infrastructure and deployment practices
- **Product Managers**: Advise on security implications of feature decisions
- **QA/Test Engineers**: Define security test cases and validation criteria

---

## Cross-Persona Collaboration Examples

### Feature Development Flow
1. **Product Manager** defines feature requirements and success criteria
2. **UX/UI Designer** creates design specifications and prototypes
3. **Developer** implements feature following design specs
4. **Security Lead** reviews code for security vulnerabilities
5. **QA/Test Engineer** validates feature against acceptance criteria
6. **SRE/DevOps** deploys to staging and production environments
7. **Project Manager** coordinates timeline and tracks progress

### Incident Response Flow
1. **SRE/DevOps** detects and declares incident
2. **Developer** investigates root cause and implements fix
3. **QA/Test Engineer** validates fix in staging environment
4. **Security Lead** assesses security implications (if applicable)
5. **Project Manager** coordinates communication to stakeholders
6. **Product Manager** evaluates customer impact and prioritizes follow-up work

### Release Handoff Flow
1. **Developer** completes implementation and code review
2. **QA/Test Engineer** executes test plan and signs off on quality
3. **Security Lead** confirms security scans pass and reviews risk
4. **SRE/DevOps** prepares deployment and rollback procedures
5. **Project Manager** confirms release readiness with all stakeholders
6. **Product Manager** reviews release notes and customer communication

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Cross-persona collaboration examples demonstrate typical handoffs and interaction patterns in modern software delivery.
- Referenced in Issue #5: https://github.com/masam23/skills-scale-institutional-knowledge-using-copilot-spaces/issues/5

