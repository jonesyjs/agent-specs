# Agent Specs

Personal collection of Claude Skills — modular, reusable instruction sets for AI agents.

## Skill Structure

Each skill is a folder containing:

```
skill-name/
├── README.md           # Summary
├── role.md             # Role definition
├── scope.md            # Allow / Disallow
├── workflow.md         # Decision logic + Stopping conditions
├── input.schema.json   # Input expectations
└── output.schema.json  # Output format
```

## Anatomy

| File | Purpose |
|------|---------|
| `role.md` | Who the agent is, expertise, communication style |
| `scope.md` | What's allowed and what's forbidden |
| `workflow.md` | Decision rules, missing input handling, stopping conditions |
| `input.schema.json` | JSON schema for expected inputs |
| `output.schema.json` | JSON schema for output format |
| `README.md` | High-level summary of the skill |

## Repository Structure

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
# Edit the files in coding/my-skill/
```
