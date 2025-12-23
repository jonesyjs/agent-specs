# Skills

Personal collection of Claude Skills — modular, reusable instruction sets.

## Structure

```
skills/
├── _template/          # Copy this to create new skills
├── category/
│   └── skill-name/
│       ├── SKILL.md    # Core instructions
│       └── ...         # Supporting files
```

## Usage

Skills are auto-loaded by Claude when relevant context is detected, or can be explicitly referenced.

## Categories

- `coding/` — Development workflows, code patterns, testing
- `writing/` — Style guides, templates, documentation
- `workflows/` — Process automation, integrations
- `creative/` — Design, brainstorming, ideation

