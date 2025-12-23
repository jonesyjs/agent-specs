# Agent Specs

Personal collection of Claude Skills — modular, reusable instruction sets for AI agents.

## Skill Anatomy

Each skill follows a two-part structure:

### 1. Context Engineering (Roles & Permissions)

| Component | Purpose |
|-----------|---------|
| **Role Definition** | Who the agent is, expertise, communication style |
| **Task Scope (Allow)** | What the skill is permitted to do |
| **Constraints (Disallow)** | Hard boundaries and restrictions |

### 2. Governance (Workflow Algorithm)

| Component | Purpose |
|-----------|---------|
| **Input Expectations** | Required inputs from user |
| **Output Format** | How results are delivered |
| **Decision Rules** | Logic for choosing between options |
| **Stopping Conditions** | When the task is complete |

## Structure

```
agent-specs/
├── _template/          # Copy this to create new skills
├── coding/             # Development workflows
├── writing/            # Style guides, templates
├── workflows/          # Process automation
└── creative/           # Design, ideation
```

## Usage

```bash
# Create a new skill
cp -r _template coding/my-skill
# Edit the SKILL.md
```

Skills are auto-loaded by Claude when relevant context is detected.
