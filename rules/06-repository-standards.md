# Repository Standards Rules (51-60)

## Rule 51: Mandatory Descriptions
Every repository MUST have a description. When creating a new repo or discovering one without a description, immediately generate one by:
1. Reading the README.md if it exists
2. Analyzing the repo name and primary language
3. Reviewing directory structure and key files
4. Creating a concise description (max 100 characters) that explains the repo's purpose

**Format:** `[Action verb] + [what it does] + [key technology/context if space allows]`

**Examples:**
- "Auto repair shop management system with Next.js frontend and Express backend"
- "Headless YouTube transcript extraction service with Playwright and RAG support"
- "Customer feedback collection and sentiment analysis application"

## Rule 52: Description Auto-Generation
When a repository lacks a description, auto-generate one using this priority order:
1. **README.md first line or title** - Extract the main heading
2. **Package.json description** - Use if available in Node projects
3. **Setup.py/pyproject.toml** - Use description field for Python projects
4. **Directory analysis** - Infer from folder structure and file types
5. **Repo name parsing** - Convert kebab-case/snake_case to readable description

## Rule 53: README Requirements
Every active repository MUST have a README.md containing at minimum:
- Project title and one-sentence description
- Setup/installation instructions
- Basic usage example
- Link to related repositories (if applicable)

## Rule 54: Naming Conventions
Repository names follow these conventions:
- Use **kebab-case** for all new repositories (e.g., `my-new-project`)
- Avoid underscores in new repos (legacy repos with underscores are acceptable)
- Use descriptive names that indicate purpose
- Prefix client projects with client name or code (e.g., `wpg-amenities`)

## Rule 55: Visibility Classification
Repositories are classified as:
- **Public**: Open source tools, documentation, portfolios
- **Private**: Client projects, internal tools, sensitive data, work-in-progress

## Rule 56: Language Tags
Add primary language/framework topics to repositories:
- `python`, `typescript`, `javascript` for language
- `nextjs`, `express`, `fastapi` for frameworks
- `ai`, `automation`, `dashboard` for domain tags

## Rule 57: Archive Policy
Repositories inactive for 90+ days with no planned future work should be:
1. Reviewed for archival
2. Documented in inventory with reason
3. Archived via GitHub if approved
4. Kept in inventory for historical reference

## Rule 58: Consolidation Triggers
Trigger consolidation review when:
- 3+ repos serve similar purposes
- Repo names suggest overlap (e.g., multiple "website" repos)
- Dependencies between repos are unclear
- Maintenance burden exceeds value

## Rule 59: Client Project Standards
Client project repositories must:
- Include client name in repo name or description
- Be set to private by default
- Have clear handoff documentation
- Include deployment/hosting information

## Rule 60: Repository Creation Checklist
When creating a new repository:
- [ ] Set meaningful description immediately
- [ ] Choose correct visibility (public/private)
- [ ] Add primary language topic
- [ ] Create initial README.md
- [ ] Link to parent epic if applicable
- [ ] Add to repository inventory
