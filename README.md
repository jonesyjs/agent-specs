# Agent Specs

Personal collection of Claude Skills — modular, reusable instruction sets for AI agents.

## Structure

```
agent-specs/
├── skills/
│   ├── _shared/         # Reusable components
│   │   ├── output-formats.md
│   │   ├── common-rules.md
│   │   └── tones.md
│   └── skill-name/
│       └── SKILL.md
├── template/
└── README.md
```

## Skill Anatomy

Each `SKILL.md` contains:

| Section | Purpose |
|---------|---------|
| **YAML Frontmatter** | Name, description, tags |
| **Role Definition** | Who the agent is, expertise, communication style |
| **Scope** | Allow / Disallow boundaries |
| **Input Expectations** | Required inputs from user |
| **Output Format** | How results are delivered |
| **Decision Rules** | Logic for choosing between options |
| **Stopping Conditions** | When the task is complete |

## Usage

```bash
# Create a new skill
cp -r template skills/my-skill
# Edit skills/my-skill/SKILL.md
```

## Skills

| Skill | Description |
|-------|-------------|
| [analysis-mode](skills/analysis-mode/) | Diagnostic skill for surfacing interpretive hypotheses about AI outputs |
| [skill-builder](skills/skill-builder/) | Meta-skill for creating fully formatted skills step-by-step or express |
| [suggester](skills/suggester/) | Domain-specific suggestion advisor |
