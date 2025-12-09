# Active Epics

> Per Rule 19: Maximum 10 active epics across all repos
> Per Rule 11: 3-5 epics per project phase

---

## EPIC-001: Portfolio Website Consolidation

**Status:** To Do
**Priority:** High
**Owner:** @Jonathan
**Phase:** 1 - Foundation

### Problem Statement
Currently 4+ website repositories exist with unclear boundaries:
- `AI-Whisperers` (Private, TypeScript)
- `ai-whisperers-portfolio-website` (Private, TypeScript)
- `AI-Whisperers-Website` (Public, TypeScript)
- `AI-Whisperers-website-and-courses` (Private, TypeScript)

### Objective
Consolidate into a single, maintainable portfolio website with clear architecture.

### Success Criteria
- [ ] Single source of truth for company website
- [ ] Deployed and accessible publicly
- [ ] Courses section integrated or clearly separated
- [ ] Old repos archived with redirect documentation

### Related Repositories
- https://github.com/Ai-Whisperers/ai-whisperers-portfolio-website
- https://github.com/Ai-Whisperers/AI-Whisperers-Website
- https://github.com/Ai-Whisperers/AI-Whisperers-website-and-courses
- https://github.com/Ai-Whisperers/AI-Whisperers

---

## EPIC-002: Marketing Pipeline Automation

**Status:** To Do
**Priority:** High
**Owner:** @Kyrian (Strategy), @Ivan (Automation)
**Phase:** 1 - Foundation

### Problem Statement
Multiple marketing-related repos exist but lack integration:
- Strategy docs scattered across repos
- Automation tools not connected to strategy
- LinkedIn content system isolated

### Objective
Create an integrated marketing pipeline from research → content → outreach → tracking.

### Success Criteria
- [ ] Unified marketing workflow documented
- [ ] Company researcher integrated with outreach
- [ ] Campaign generator connected to content system
- [ ] Metrics tracking implemented

### Related Repositories
- https://github.com/Ai-Whisperers/marketing-strategy
- https://github.com/Ai-Whisperers/outreach-automation
- https://github.com/Ai-Whisperers/AI-powered-marketing-campaign-generator
- https://github.com/Ai-Whisperers/Company-resarcher
- https://github.com/Ai-Whisperers/linkedin-content-system
- https://github.com/Ai-Whisperers/social-media-intelligence-marketing

---

## EPIC-003: Client Feedback Intelligence Platform

**Status:** To Do
**Priority:** High
**Owner:** @Ivan (Development), @Kyrian (Client-facing)
**Phase:** 1 - Foundation

### Problem Statement
Feedback and social listening tools are fragmented:
- Comment extraction separate from analysis
- Backend not integrated with frontend
- No unified dashboard for insights

### Objective
Build a cohesive platform for collecting, analyzing, and presenting client feedback.

### Success Criteria
- [ ] Single deployment for feedback collection
- [ ] Automated sentiment analysis
- [ ] Client-facing dashboard
- [ ] API for integrations

### Related Repositories
- https://github.com/Ai-Whisperers/customer-feedback-app
- https://github.com/Ai-Whisperers/feedbackScope-backend
- https://github.com/Ai-Whisperers/Comment-Exctractor
- https://github.com/Ai-Whisperers/scrapped-comments

---

## EPIC-004: Internal Operations Tooling

**Status:** To Do
**Priority:** Medium
**Owner:** @Ivan
**Phase:** 2 - Optimization

### Problem Statement
Internal tools exist but aren't connected:
- Time tracking works but needs better reporting
- Jira parser isolated
- No central ops dashboard

### Objective
Integrate internal tools for unified operations management.

### Success Criteria
- [ ] Automated time reporting with alerts
- [ ] Project metadata parsing integrated
- [ ] Single internal ops view
- [ ] Reduced manual reporting time by 50%

### Related Repositories
- https://github.com/Ai-Whisperers/work-hours-automated-reports
- https://github.com/Ai-Whisperers/jira-meta-parser
- https://github.com/Ai-Whisperers/claude-portable-improving-system
- https://github.com/Ai-Whisperers/team-tasks

---

## EPIC-005: Infrastructure & Deployment Platform

**Status:** To Do
**Priority:** Medium
**Owner:** @Jonathan
**Phase:** 2 - Optimization

### Problem Statement
Infrastructure scattered across multiple configs:
- K8s configs in one repo
- Self-hosting docs in another
- AWS configs separate
- No unified deployment workflow

### Objective
Create standardized deployment pipeline for all projects.

### Success Criteria
- [ ] Single deployment config repository
- [ ] Automated CI/CD for all active projects
- [ ] Self-hosting documentation complete
- [ ] Cost tracking implemented

### Related Repositories
- https://github.com/Ai-Whisperers/clustering-for-ai-whisperers-hosting-and-deploys
- https://github.com/Ai-Whisperers/self-hosting-ai-whisperers
- https://github.com/Ai-Whisperers/aws-docker-mcp
- https://github.com/Ai-Whisperers/storage-service

---

## EPIC-006: Data Processing Pipeline

**Status:** To Do
**Priority:** Medium
**Owner:** @Ivan
**Phase:** 2 - Optimization

### Problem Statement
Multiple overlapping data processing tools:
- Analysis engine duplicates normalizer functions
- Excel parsing separate from general parsing
- No unified data ingestion

### Objective
Consolidate data processing into modular, reusable pipeline.

### Success Criteria
- [ ] Single entry point for data ingestion
- [ ] Modular parsers (Excel, CSV, JSON, Parquet)
- [ ] Automated schema detection
- [ ] Output to standardized formats

### Related Repositories
- https://github.com/Ai-Whisperers/analysis-engine
- https://github.com/Ai-Whisperers/normalizer-service
- https://github.com/Ai-Whisperers/excel-parsing-service
- https://github.com/Ai-Whisperers/agentic-schemas

---

## EPIC-007: AI/ML Product Suite

**Status:** To Do
**Priority:** Low
**Owner:** @Jonathan (Architecture), @Ivan (Implementation)
**Phase:** 3 - Innovation

### Problem Statement
Several AI projects in various states:
- LangAi active but unclear scope
- Ternary engine experimental
- RAG chatbot incomplete
- Meeting agent prototype

### Objective
Define and prioritize AI product roadmap.

### Success Criteria
- [ ] Clear product definition for each AI project
- [ ] Prioritized development roadmap
- [ ] At least one production-ready AI feature
- [ ] Documentation for AI capabilities

### Related Repositories
- https://github.com/Ai-Whisperers/LangAi
- https://github.com/Ai-Whisperers/ternary-engine
- https://github.com/Ai-Whisperers/chatbot-rag-rbac
- https://github.com/Ai-Whisperers/meeting-ai-agent
- https://github.com/Ai-Whisperers/audio-to-text

---

## EPIC-008: Education & Courses Platform

**Status:** To Do
**Priority:** Low
**Owner:** @Kyrian (Content), @Jonathan (Platform)
**Phase:** 3 - Innovation

### Problem Statement
Course content scattered:
- Multiple course repos
- Content separate from delivery platform
- No clear curriculum structure

### Objective
Unified courses platform with structured content.

### Success Criteria
- [ ] Single courses content repository
- [ ] Learning management integration
- [ ] Course catalog documented
- [ ] At least 3 complete courses

### Related Repositories
- https://github.com/Ai-Whisperers/Courses-Content
- https://github.com/Ai-Whisperers/Summer-courses
- https://github.com/Ai-Whisperers/courseResource

---

## Epic Summary

| Epic | Priority | Owner | Phase | Status |
|------|----------|-------|-------|--------|
| EPIC-001: Website Consolidation | High | @Jonathan | 1 | To Do |
| EPIC-002: Marketing Pipeline | High | @Kyrian/@Ivan | 1 | To Do |
| EPIC-003: Feedback Platform | High | @Ivan/@Kyrian | 1 | To Do |
| EPIC-004: Internal Ops | Medium | @Ivan | 2 | To Do |
| EPIC-005: Infrastructure | Medium | @Jonathan | 2 | To Do |
| EPIC-006: Data Processing | Medium | @Ivan | 2 | To Do |
| EPIC-007: AI/ML Suite | Low | @Jonathan/@Ivan | 3 | To Do |
| EPIC-008: Courses Platform | Low | @Kyrian/@Jonathan | 3 | To Do |

**Active Epics: 8** (within 10 limit per Rule 19)
