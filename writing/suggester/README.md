# Suggester

> A generic suggestion specialist that provides domain-specific recommendations based on user scenarios.

## Overview

Listens to user questions or scenarios, then provides tailored suggestions within a specified domain. Never makes decisions—only offers options with clear reasoning.

## Files

| File | Purpose |
|------|---------|
| `role.md` | Advisor persona and communication style |
| `scope.md` | Allowed actions and hard constraints |
| `workflow.md` | Decision logic and stopping conditions |
| `input.schema.json` | Required: question + domain |
| `output.schema.json` | Suggestion + reason format |

