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
**Status:** Done ✅
**Effort:** 4 hours
**Dependencies:** TASK-001
**Completed:** 2025-12-09

Add meaningful descriptions to the 28 repositories currently missing them.

**Acceptance Criteria:**
- [x] All repos have descriptions
- [x] Descriptions are actionable and clear
- [x] Updated via GitHub CLI

All 28 repositories now have descriptions. See Rule 51-60 for auto-generation standards.

---

### TASK-003: Audit Website Repositories
**Priority:** High
**Assignee:** @Jonathan
**Status:** Done ✅
**Effort:** 3 hours
**Dependencies:** None
**Completed:** 2025-12-09

Review all 4+ website repos to determine consolidation strategy.

**Acceptance Criteria:**
- [x] Each website repo reviewed for content
- [x] Differences documented
- [x] Recommendation for consolidation written
- [x] Migration plan drafted

**Findings Summary:**

| Repo | Created | Last Push | Status | Purpose |
|------|---------|-----------|--------|---------|
| AI-Whisperers | Aug 12 | Nov 12 | Semi-Active | Org main repo + internal tools |
| AI-Whisperers-Website | Aug 14 | Sep 16 | Dormant | Original website (Next.js 15, AI SDK) |
| AI-Whisperers-website-and-courses | Sep 4 | Oct 14 | Dormant | Combined site + courses |
| ai-whisperers-portfolio-website | Oct 1 | Dec 1 | **Active** | Current portfolio website |

**Recommendation:**
1. **KEEP**: `ai-whisperers-portfolio-website` as PRIMARY website
2. **ARCHIVE**: `AI-Whisperers-website-and-courses` (superseded)
3. **MIGRATE**: Useful features from `AI-Whisperers-Website` (AI SDK, multilingual)
4. **RENAME**: `AI-Whisperers` to `internal-tools` for clarity
5. **CLEANUP**: Remove personal notes from AI-Whisperers-Website/CLAUDE.md

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

### TASK-006: Polish Dormant Repositories
**Priority:** Medium
**Assignee:** @Kyrian
**Status:** To Do
**Effort:** 2 hours
**Dependencies:** TASK-001

Review dormant repositories and create improvement plans (no archiving - all repos have value).

**Repos to Review:**
- demo-repository - identify use case
- Call-Recorder - document features, plan updates
- WPG-Amenities - waiting for client pictures
- Lawfirm-website - **Dropped** (client declined price)

**Acceptance Criteria:**
- [ ] Each dormant repo reviewed
- [ ] Improvement plan documented per repo
- [ ] Priority for reactivation assigned
- [ ] Status updated in inventory

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

### TASK-011: Consolidate Website Repositories
**Priority:** High
**Assignee:** @Jonathan
**Status:** To Do
**Effort:** 6 hours
**Dependencies:** TASK-003

Execute the website consolidation plan from TASK-003 findings.

**Action Items:**
1. Archive `AI-Whisperers-website-and-courses`
2. Migrate AI SDK + multilingual features from `AI-Whisperers-Website` to `ai-whisperers-portfolio-website`
3. Rename `AI-Whisperers` repo to `internal-tools`
4. Clean up CLAUDE.md (remove personal notes)
5. Update all cross-references and documentation

**Subtasks:**
- [ ] Create migration branch in portfolio website
- [ ] Copy AI SDK integration code (@ai-sdk/anthropic, @ai-sdk/openai)
- [ ] Port multilingual implementation (MULTILINGUAL_IMPLEMENTATION.md)
- [ ] Archive AI-Whisperers-website-and-courses via GitHub
- [ ] Rename AI-Whisperers repo
- [ ] Delete/replace CLAUDE.md with proper AI instructions
- [ ] Update inventory and epic docs

**Acceptance Criteria:**
- [ ] Single active website repository
- [ ] AI features preserved
- [ ] Archived repos marked appropriately
- [ ] Documentation updated

---

### TASK-012: Create Website Architecture Document
**Priority:** Medium
**Assignee:** @Kyrian
**Status:** To Do
**Effort:** 2 hours
**Dependencies:** TASK-011

Document the consolidated website architecture for future development.

**Note:** Website will merge portfolio + courses into one unified site with logical navigation structure.

**Acceptance Criteria:**
- [ ] Tech stack documented (Next.js, React, Tailwind, etc.)
- [ ] Feature inventory (AI chat, multilingual, courses section)
- [ ] Deployment process documented
- [ ] Development setup guide

---

## Phase 2 Tasks - Gap Analysis Actions

### TASK-013: Define Stories for Phase 1 Epics
**Priority:** High
**Assignee:** @Kyrian
**Status:** To Do
**Effort:** 4 hours
**Dependencies:** None
**Epic:** EPIC-001, EPIC-002, EPIC-003

Break down Phase 1 epics (Website, Marketing, Feedback) into user stories.

**Acceptance Criteria:**
- [ ] 5-8 stories per epic defined
- [ ] Each story follows "As a... I want... so that..." format (Rule 12)
- [ ] Acceptance criteria for each story (Rule 20)
- [ ] Stories added to planning/stories/ folder

---

### TASK-014: Create Project Roadmap
**Priority:** Medium
**Assignee:** @Kyrian
**Status:** To Do
**Effort:** 2 hours
**Dependencies:** TASK-013

Create visual roadmap with quarterly milestones and epic timelines.

**Acceptance Criteria:**
- [ ] Mermaid Gantt chart created
- [ ] All 8 epics mapped to timeline
- [ ] Dependencies visualized
- [ ] Added to planning/roadmap.md

---

### TASK-015: Set Up GitHub Actions
**Priority:** Medium
**Assignee:** @Jonathan
**Status:** To Do
**Effort:** 3 hours
**Dependencies:** None

Add CI/CD workflows for documentation quality.

**Workflows Needed:**
- [ ] Markdown linting
- [ ] Link checking
- [ ] Auto table of contents generation

**Acceptance Criteria:**
- [ ] .github/workflows/ created
- [ ] At least 2 workflows functional
- [ ] Badge added to README

---

### TASK-016: Create Repository Health Dashboard
**Priority:** Medium
**Assignee:** @Ivan
**Status:** To Do
**Effort:** 2 hours
**Dependencies:** None

Document current health status per Rule 70 indicators.

**Acceptance Criteria:**
- [ ] Health status per repo documented
- [ ] Added to inventory/health-status.md
- [ ] Critical repos flagged
- [ ] Update process documented

---

### TASK-017: Create Risk Register
**Priority:** Low
**Assignee:** @Kyrian
**Status:** To Do
**Effort:** 2 hours
**Dependencies:** TASK-013

Document risks and mitigation strategies for Phase 1 epics.

**Acceptance Criteria:**
- [ ] Risk identification per epic
- [ ] Impact assessment (High/Medium/Low)
- [ ] Mitigation strategies documented
- [ ] Added to planning/risk-register.md

---

## Task Summary

| ID | Task | Priority | Assignee | Status | Effort |
|----|------|----------|----------|--------|--------|
| TASK-001 | Document Repository Inventory | High | @Kyrian | Done ✅ | 2h |
| TASK-002 | Add Repo Descriptions | High | @Jonathan | Done ✅ | 4h |
| TASK-003 | Audit Website Repos | High | @Jonathan | Done ✅ | 3h |
| TASK-004 | Define Marketing Stories | High | @Kyrian | To Do | 2h |
| TASK-005 | Set Up Ignition Project | Medium | @Jonathan | To Do | 4h |
| TASK-006 | Polish Dormant Repos | Medium | @Kyrian | To Do | 2h |
| TASK-007 | Create README Templates | Medium | @Ivan | To Do | 2h |
| TASK-008 | Map Marketing Dependencies | High | @Ivan | To Do | 3h |
| TASK-009 | Review Comment-Extractor | High | @Ivan | To Do | 2h |
| TASK-010 | Document Infrastructure | Medium | @Jonathan | To Do | 3h |
| TASK-011 | Consolidate Website Repos | High | @Jonathan | To Do | 6h |
| TASK-012 | Website Architecture Doc | Medium | @Kyrian | To Do | 2h |
| TASK-013 | Define Stories for Phase 1 Epics | High | @Kyrian | To Do | 4h |
| TASK-014 | Create Project Roadmap | Medium | @Kyrian | To Do | 2h |
| TASK-015 | Set Up GitHub Actions | Medium | @Jonathan | To Do | 3h |
| TASK-016 | Create Repository Health Dashboard | Medium | @Ivan | To Do | 2h |
| TASK-017 | Create Risk Register | Low | @Kyrian | To Do | 2h |

### Workload Distribution

| Assignee | Tasks | Total Effort | Completed |
|----------|-------|--------------|-----------|
| @Kyrian | 7 | 16 hours | 1 (2h) |
| @Jonathan | 6 | 22 hours | 2 (7h) |
| @Ivan | 4 | 9 hours | 0 |

---

## Priority Matrix (Based on Activity Analysis)

Per Rule 67, tasks are scored: `(Client×3) + (Blocker×2) + (Activity×1)`

| Task | Client | Blocker | Activity | Score | **Rank** |
|------|--------|---------|----------|-------|----------|
| Comment Analyzer (current) | 0 | 2 | 1 | **3** | 1 |
| TASK-011 Website Consolidation | 0 | 2 | 1 | **3** | 1 |
| TASK-008 Map Marketing Deps | 0 | 2 | 1 | **3** | 1 |
| Taller_Ocampos (product research) | 0 | 0 | 1 | **1** | 4 |
| TASK-004 Marketing Stories | 0 | 0 | 1 | **1** | 4 |
| TASK-010 Infrastructure Doc | 0 | 0 | 0.5 | **0.5** | 6 |

### Current Active Projects by Owner

**@Jonathan** (5 projects - within 50% limit per Rule 63):
1. 🟢 Comment-Analyzer - **Currently working on**
2. 🟢 yt-transcript-headless - Product, active
3. 🟡 agentic-schemas - Internal, recent
4. 🟠 Taller_Ocampos - Product research pending
5. 🟠 WPG-Amenities - Client, waiting for pictures

**@Kyrian** (2 projects):
1. 🟢 marketing-strategy - Business dev, active
2. 🟢 Courses-Content - Revenue, active

**@Ivan** (1 visible + private):
1. 🟡 team-tasks - Internal, recent
2. (Private repos not visible)

### Recommended Immediate Priorities

1. **@Jonathan**: Complete Comment-Analyzer, then TASK-011 Website Consolidation
2. **@Kyrian**: TASK-004 Define Marketing Stories (enables pipeline)
3. **@Ivan**: TASK-008 Map Marketing Dependencies (enables automation)

See [team-activity-analysis.md](team-activity-analysis.md) for full analysis.
