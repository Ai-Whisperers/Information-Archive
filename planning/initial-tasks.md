# Initial Task Backlog

> Per Rule 1: Every task has a unique ID
> Per Rule 2: Descriptions start with a verb
> Per Rule 8: Deadlines not exceeding one week

---

## Phase 1 Tasks - Foundation

### TASK-001: Document Repository Inventory
**Priority:** High
**Assignee:** @Kyrian
**Status:** Done
**Effort:** 2 hours
**Dependencies:** None

Create comprehensive inventory of all 50 repositories with status, language, and ownership.

**Acceptance Criteria:**
- [x] All repos listed with metadata
- [x] Status categorization (Active/Recent/Semi-Active/Dormant)
- [x] Missing descriptions identified

---

### TASK-002: Add Descriptions to Undocumented Repos
**Priority:** High
**Assignee:** @Jonathan
**Status:** To Do
**Effort:** 4 hours
**Dependencies:** TASK-001

Add meaningful descriptions to the 28 repositories currently missing them.

**Acceptance Criteria:**
- [ ] All repos have descriptions
- [ ] Descriptions are actionable and clear
- [ ] Updated via GitHub API or UI

**Repos Needing Descriptions:**
1. LangAi
2. customer-feedback-app
3. Taller_Ocampos
4. Company-resarcher
5. yt-transcript-headless
6. Courses-Content
7. outreach-automation
8. AI-powered-marketing-campaign-generator
9. feedbackScope-backend
10. scrapped-comments
11. cluster-template
12. Lawfirm-website
13. legal
14. agentic-schemas
15. templates-standard
16. AI-Whisperers
17. linkedin-content-system
18. excel-parsing-service
19. storage-service
20. Negociation-Personal
21. transcriptions
22. n8nResearch
23. branding-tester
24. aws-docker-mcp
25. courseResource
26. AI-Whisperers-website-and-courses
27. jira-meta-parser
28. chatbot-rag-rbac

---

### TASK-003: Audit Website Repositories
**Priority:** High
**Assignee:** @Jonathan
**Status:** To Do
**Effort:** 3 hours
**Dependencies:** None

Review all 4+ website repos to determine consolidation strategy.

**Acceptance Criteria:**
- [ ] Each website repo reviewed for content
- [ ] Differences documented
- [ ] Recommendation for consolidation written
- [ ] Migration plan drafted

**Subtasks:**
- [ ] Clone and review AI-Whisperers
- [ ] Clone and review ai-whisperers-portfolio-website
- [ ] Clone and review AI-Whisperers-Website
- [ ] Clone and review AI-Whisperers-website-and-courses
- [ ] Document findings
- [ ] Propose single architecture

---

### TASK-004: Define Stories for EPIC-002 Marketing Pipeline
**Priority:** High
**Assignee:** @Kyrian
**Status:** To Do
**Effort:** 2 hours
**Dependencies:** TASK-001

Break down Marketing Pipeline epic into user stories with acceptance criteria.

**Acceptance Criteria:**
- [ ] 5-8 user stories defined (per Rule 13)
- [ ] Each story has acceptance criteria (per Rule 20)
- [ ] Stories linked to specific repos
- [ ] Initial task breakdown for top story

---

### TASK-005: Set Up Ignition Project Structure
**Priority:** Medium
**Assignee:** @Jonathan
**Status:** To Do
**Effort:** 4 hours
**Dependencies:** None

Initialize Ignition project with dashboard views for repository tracking.

**Acceptance Criteria:**
- [ ] Ignition project created
- [ ] Basic navigation structure
- [ ] Role-based access configured
- [ ] Git binding for task data

---

### TASK-006: Archive Dormant Repositories
**Priority:** Medium
**Assignee:** @Jonathan
**Status:** To Do
**Effort:** 1 hour
**Dependencies:** TASK-001

Review and archive truly dormant repositories that have no future use.

**Candidates for Review:**
- demo-repository (GitHub demo, likely archivable)
- Call-Recorder (no activity since Sept)
- WPG-Amenities (client project - check status)

**Acceptance Criteria:**
- [ ] Each dormant repo reviewed
- [ ] Decision documented (archive/activate/keep)
- [ ] Archived repos marked in GitHub
- [ ] Reason logged in inventory

---

### TASK-007: Create README Templates
**Priority:** Medium
**Assignee:** @Ivan
**Status:** To Do
**Effort:** 2 hours
**Dependencies:** None

Create standardized README templates for different project types.

**Templates Needed:**
- [ ] Python tool/service template
- [ ] TypeScript web app template
- [ ] Documentation repo template
- [ ] Client project template

**Acceptance Criteria:**
- [ ] Templates created in templates-standard repo
- [ ] Each template includes sections for: Overview, Setup, Usage, Contributing
- [ ] Badge placeholders included

---

### TASK-008: Map Marketing Tool Dependencies
**Priority:** High
**Assignee:** @Ivan
**Status:** To Do
**Effort:** 3 hours
**Dependencies:** None

Document how marketing automation tools connect and identify gaps.

**Tools to Map:**
- Company-resarcher → ?
- outreach-automation → ?
- AI-powered-marketing-campaign-generator → ?
- linkedin-content-system → ?

**Acceptance Criteria:**
- [ ] Data flow diagram created
- [ ] API dependencies documented
- [ ] Integration gaps identified
- [ ] Recommendations for connections

---

### TASK-009: Review Comment-Extractor for Feedback Platform
**Priority:** High
**Assignee:** @Ivan
**Status:** To Do
**Effort:** 2 hours
**Dependencies:** None

Assess Comment-Exctractor capabilities and integration with customer-feedback-app.

**Acceptance Criteria:**
- [ ] Current features documented
- [ ] API endpoints listed
- [ ] Integration points with feedback app identified
- [ ] Enhancement recommendations

---

### TASK-010: Document Infrastructure Stack
**Priority:** Medium
**Assignee:** @Jonathan
**Status:** To Do
**Effort:** 3 hours
**Dependencies:** None

Create comprehensive infrastructure documentation from scattered configs.

**Sources:**
- clustering-for-ai-whisperers-hosting-and-deploys
- self-hosting-ai-whisperers
- aws-docker-mcp

**Acceptance Criteria:**
- [ ] Current architecture diagram
- [ ] Service inventory
- [ ] Deployment procedures documented
- [ ] Cost breakdown (if available)

---

## Task Summary

| ID | Task | Priority | Assignee | Status | Effort |
|----|------|----------|----------|--------|--------|
| TASK-001 | Document Repository Inventory | High | @Kyrian | Done | 2h |
| TASK-002 | Add Repo Descriptions | High | @Jonathan | To Do | 4h |
| TASK-003 | Audit Website Repos | High | @Jonathan | To Do | 3h |
| TASK-004 | Define Marketing Stories | High | @Kyrian | To Do | 2h |
| TASK-005 | Set Up Ignition Project | Medium | @Jonathan | To Do | 4h |
| TASK-006 | Archive Dormant Repos | Medium | @Jonathan | To Do | 1h |
| TASK-007 | Create README Templates | Medium | @Ivan | To Do | 2h |
| TASK-008 | Map Marketing Dependencies | High | @Ivan | To Do | 3h |
| TASK-009 | Review Comment-Extractor | High | @Ivan | To Do | 2h |
| TASK-010 | Document Infrastructure | Medium | @Jonathan | To Do | 3h |

### Workload Distribution

| Assignee | Tasks | Total Effort |
|----------|-------|--------------|
| @Kyrian | 2 | 4 hours |
| @Jonathan | 5 | 15 hours |
| @Ivan | 3 | 7 hours |

> Note: @Jonathan has highest initial load for infrastructure setup. Consider redistributing after Phase 1.
