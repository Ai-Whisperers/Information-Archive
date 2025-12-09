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
**Assignee:** @Jonathan
**Status:** To Do
**Effort:** 2 hours
**Dependencies:** TASK-011

Document the consolidated website architecture for future development.

**Acceptance Criteria:**
- [ ] Tech stack documented (Next.js, React, Tailwind, etc.)
- [ ] Feature inventory (AI chat, multilingual, etc.)
- [ ] Deployment process documented
- [ ] Development setup guide

---

## Task Summary

| ID | Task | Priority | Assignee | Status | Effort |
|----|------|----------|----------|--------|--------|
| TASK-001 | Document Repository Inventory | High | @Kyrian | Done ✅ | 2h |
| TASK-002 | Add Repo Descriptions | High | @Jonathan | Done ✅ | 4h |
| TASK-003 | Audit Website Repos | High | @Jonathan | Done ✅ | 3h |
| TASK-004 | Define Marketing Stories | High | @Kyrian | To Do | 2h |
| TASK-005 | Set Up Ignition Project | Medium | @Jonathan | To Do | 4h |
| TASK-006 | Archive Dormant Repos | Medium | @Jonathan | To Do | 1h |
| TASK-007 | Create README Templates | Medium | @Ivan | To Do | 2h |
| TASK-008 | Map Marketing Dependencies | High | @Ivan | To Do | 3h |
| TASK-009 | Review Comment-Extractor | High | @Ivan | To Do | 2h |
| TASK-010 | Document Infrastructure | Medium | @Jonathan | To Do | 3h |
| TASK-011 | Consolidate Website Repos | High | @Jonathan | To Do | 6h |
| TASK-012 | Website Architecture Doc | Medium | @Jonathan | To Do | 2h |

### Workload Distribution

| Assignee | Tasks | Total Effort | Completed |
|----------|-------|--------------|-----------|
| @Kyrian | 2 | 4 hours | 1 (2h) |
| @Jonathan | 7 | 23 hours | 2 (7h) |
| @Ivan | 3 | 7 hours | 0 |

> Note: @Jonathan has highest load. TASK-011 (website consolidation) is highest priority next step.
