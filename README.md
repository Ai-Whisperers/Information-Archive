# Repository Dashboard Project README

## Overview
This Ignition-based dashboard provides a centralized view of all company repositories, emphasizing to-do lists for actionable tasks across active and inactive projects. Unlike the Company Information project (focused on business details and marketing feeds), this tracks epics, stories, tasks, and subtasks to guide team members on immediate starting points. Built with Ignition views for role-based access and Git integration.

## Project Structure
Organize work hierarchically:
- **Epics**: High-level goals (e.g., "Full Repo Oversight Dashboard").
- **Stories**: User-focused deliverables (e.g., "As a dev, filter inactive repos").
- **Tasks**: Specific actions (e.g., "Build filter UI").
- **Subtasks**: Granular steps (e.g., "Code dropdown component").

Use Ignition Perspective/Vision for views: Epic overview → Story tabs → Task boards with expandable subtasks.

## Team Roles and Assignments
Tasks are assigned by expertise:
- **Kyrian**: Outreach, client investigation, project management (non-coding). E.g., "Repo outreach docs."
- **Ivan**: Internal tools (scrapers, analyzers, generators). E.g., "Repo data automation scripts."
- **Jonathan (CTO)**: Backend, hosting (Pages), tech stack. E.g., "Infrastructure setup."

Tag with @Kyrian, @Ivan, @Jonathan; require acceptance for status updates.

## Rules and Workflow
- **Task Rules**: Include ID, description, priority (High/Medium/Low), assignee, dependencies, deadlines, status (To Do/In Progress/Done/Blocked/Outdated).
- **Cadence**: Weekly epic planning; daily standups; end-of-day Git syncs.
- **Dashboard Features**: Repo list with filters; drill-down boards; role-based views; audit logs.
- **Differentiation**: No company/marketing data—link to repos/Git for context.

## Setup Instructions
1. Clone this Ignition project as base; inherit in repo-specific children.
2. Configure Git bindings for task data pull.
3. Set role permissions in Ignition security.
4. Launch dashboard; populate initial epics.

## Contribution Guidelines
- Create issues/PRs mirroring epic-story-task structure.
- Reference rules in commits.
- Weekly reviews to prioritize inactive projects.

For questions, ping @Jonathan for tech, @Kyrian for process. Start contributing!
