# OctoAcme — Cross-Functional Collaboration

## Purpose
Define how expanded project roles interact, collaborate, and support project success through clear handoffs, communication patterns, and shared accountability.

## Context
As projects scale, cross-functional teams need explicit guidance on how diverse roles work together effectively. This document clarifies role dependencies, decision-making authority, and communication expectations.

---

## Role Interaction Matrix

### Core Dependencies by Phase

#### Initiation Phase
| Role | Responsibility | Key Collaborators | Deliverable |
|------|-----------------|-------------------|-------------|
| **Product Manager** | Define business need and success metrics | Stakeholder/Sponsor, PM | Project One-pager |
| **Stakeholder/Sponsor** | Approve strategic fit and budget | Product Manager, PM | Budget approval & go-ahead |
| **Project Manager** | Establish governance and timeline | Product Manager, Sponsor | High-level plan |

#### Planning Phase
| Role | Responsibility | Key Collaborators | Deliverable |
|------|-----------------|-------------------|-------------|
| **Product Manager** | Prioritize backlog and acceptance criteria | Developers, QA Lead, PdM | Prioritized backlog |
| **Technical Lead** | Define architecture and technology choices | Developers, Security Engineer | Technical design document |
| **Project Manager** | Create detailed timeline and dependencies | Technical Lead, QA Lead, All roles | Project schedule |
| **QA Lead** | Draft test strategy and acceptance criteria | Product Manager, Developers | Test plan |
| **Scrum Master** | Establish team norms and sprint structure | All team members | Sprint setup and cadence |

#### Execution Phase
| Role | Responsibility | Key Collaborators | Deliverable |
|------|-----------------|-------------------|-------------|
| **Developer** | Implement features to acceptance criteria | Technical Lead, QA Lead, Design Lead | Code & PRs |
| **Technical Lead** | Review design decisions, mentor developers | Developers, Architect discussions | Technical guidance & reviews |
| **Design Lead** | Validate UX and design implementation | Developers, Product Manager, Users | Design specs & feedback |
| **QA Lead** | Test implementations and track defects | Developers, Product Manager | Test results & defect reports |
| **Scrum Master** | Remove blockers and facilitate ceremonies | All team members | Meeting facilitation, blocker resolution |
| **Security Engineer** | Review security requirements & findings | Developers, Technical Lead | Security assessments & fixes |
| **Project Manager** | Track progress and manage risks | All roles | Status updates & escalations |

#### Release Phase
| Role | Responsibility | Key Collaborators | Deliverable |
|------|-----------------|-------------------|-------------|
| **Technical Lead** | Plan deployment and rollback strategy | DevOps/Infra, QA Lead | Deployment plan |
| **QA Lead** | Execute smoke tests and sign-off | Product Manager, Developers | Release readiness |
| **Project Manager** | Coordinate release window and communication | Product Manager, all roles | Release announcement |
| **Security Engineer** | Verify security controls in production | Technical Lead, DevOps | Security verification |
| **Product Manager** | Release notes and customer communication | Project Manager, Marketing | Release announcement content |

#### Retrospective Phase
| Role | Responsibility | Key Collaborators | Deliverable |
|------|-----------------|-------------------|-------------|
| **Scrum Master** | Facilitate retrospective and capture learnings | All team members | Retrospective notes |
| **Project Manager** | Track action items and follow-up | All roles | Action item tracking |

---

## Critical Collaboration Patterns

### 1. Acceptance Criteria Definition
**Owner**: Product Manager (with QA Lead & Developers)

**Pattern**:
1. Product Manager drafts acceptance criteria
2. QA Lead validates testability and identifies test scenarios
3. Developers identify implementation complexity and edge cases
4. Collaboratively refine until all parties agree

**Success Metric**: Criteria are testable, implementable, and measurable

### 2. Technical Design & Security Review
**Owner**: Technical Lead (with Security Engineer & Developers)

**Pattern**:
1. Technical Lead proposes architecture for a feature
2. Security Engineer reviews for security risks and compliance
3. Developers provide implementation feedback
4. Design finalized in design review meeting

**Success Metric**: Design addresses scalability, security, and performance concerns

### 3. Design-to-Development Handoff
**Owner**: Design Lead (with Developers & Product Manager)

**Pattern**:
1. Design Lead presents wireframes and prototypes to Product Manager for UX validation
2. Design Lead reviews implementation with Developers during development
3. Developers validate accessibility and responsive design with Design Lead
4. Final sign-off before feature release

**Success Metric**: Delivered feature matches design intent and passes UX validation

### 4. Test Planning & Quality Gate
**Owner**: QA Lead (with Product Manager & Developers)

**Pattern**:
1. QA Lead creates test plan aligned with acceptance criteria (in Planning phase)
2. During execution, QA Lead communicates test results and defect prioritization
3. Developers address defects in priority order
4. QA Lead validates fixes and marks feature as ready for release

**Success Metric**: Feature passes all acceptance criteria and quality gates before release

### 5. Risk & Dependency Escalation
**Owner**: Project Manager (with all roles)

**Pattern**:
1. Team identifies risks or blockers in daily standup or sprint planning
2. Project Manager triages and escalates to appropriate level:
   - **Level 1** (Team): Scrum Master helps resolve
   - **Level 2** (Cross-team): PM escalates to Product Lead
   - **Level 3** (Business): PM escalates to Sponsor
3. Project Manager tracks resolution status and communicates updates
4. Scrum Master removes team-level blockers proactively

**Success Metric**: Blockers resolved within agreed SLA; no surprises at stakeholder reviews

### 6. Release Coordination
**Owner**: Project Manager (with Technical Lead, QA Lead, Product Manager)

**Pattern**:
1. Product Manager confirms scope and release date
2. Technical Lead provides deployment plan and rollback strategy
3. QA Lead executes smoke tests and provides sign-off
4. Project Manager coordinates release window and communication
5. Security Engineer verifies production controls post-deployment

**Success Metric**: Release deployed on schedule with zero unplanned rollbacks

---

## Communication Cadence by Role

### Daily
- **Developers**: Standup with team, code reviews with peers and Technical Lead
- **Scrum Master**: Facilitate standup, identify blockers
- **QA Lead**: Test status updates, defect triage
- **Project Manager**: Ad-hoc escalations as needed

### Weekly
- **Product Manager & Project Manager**: Alignment on priorities and risks
- **Technical Lead**: Design review or tech talk with team
- **Stakeholder/Sponsor**: Status via PM (milestone-based or on-demand)
- **Design Lead**: Check-in with developers on implementation fidelity

### Sprint/Iteration Boundary
- **All roles**: Sprint planning (what we'll build)
- **All roles**: Sprint review (what we built and delivered)
- **All roles**: Retrospective (what we learned and how to improve)

### Monthly/Milestone
- **Stakeholder/Sponsor**: Executive update on progress, risks, and business impact
- **Project Manager**: Full project health review across all dimensions

---

## Decision Authority Matrix

| Decision Type | Owner | Consultants | Approval Required |
|---|---|---|---|
| Acceptance Criteria | Product Manager | QA, Developers | Product Lead |
| Technical Design | Technical Lead | Developers, Security | Architecture review |
| Test Scope & Strategy | QA Lead | Product Manager, Developers | Product Manager approval |
| Release Date | Project Manager + Product Manager | Technical Lead, Sponsor | Sponsor sign-off |
| Security Requirements | Security Engineer | Technical Lead, Product Manager | Security Lead |
| Design & UX | Design Lead | Product Manager, Developers | Product Manager validation |
| Sprint Scope | Scrum Master + Product Manager | Developers | PM/PdM alignment |
| Escalation Path | Project Manager | Relevant stakeholders | Sponsor (if L3) |

---

## Collaboration Health Indicators

- ✅ Acceptance criteria are clear, testable, and agreed by all parties before development starts
- ✅ Design decisions are documented and reviewed by Technical Lead and Security Engineer
- ✅ QA is involved in planning and design phases, not just execution
- ✅ Blockers are surfaced within 24 hours of identification
- ✅ Risk register is reviewed and updated weekly
- ✅ Cross-functional handoffs occur with explicit "ready" checkpoints
- ✅ Retrospectives capture action items and drive visible improvements
- ✅ Communication is transparent, timely, and uses consistent channels

---

## Onboarding Checklist for New Team Members

- [ ] Meet each role on the project and understand their responsibilities
- [ ] Review this collaboration guide and ask questions about role dependencies
- [ ] Observe a sprint planning, standup, and retrospective
- [ ] Understand the escalation path for your role
- [ ] Know who to contact for each type of decision or blocker
- [ ] Have 1-on-1 with your functional lead (PdM, PM, Tech Lead, etc.)
