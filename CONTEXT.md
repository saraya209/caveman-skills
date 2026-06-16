# Context

## Domain

This repository is a curated skill collection for AI coding agents. It publishes `caveman`, `caveman-compress`, `caveman-commit`, `caveman-review`, `grill-me`, `junior-to-senior`, and `context-canary`. Forked from JuliusBrussee/skills + JuliusBrussee/caveman.

## Core Concepts

- **Skill** - installable instruction directory, usually `SKILL.md` plus optional references.
- **Caveman** - communication compression style that removes filler while preserving technical detail. Levels: lite/full/ultra.
- **Caveman Compress** - compress natural-language memory files inline; preserves code blocks exactly, backs up the original.
- **Caveman Commit / Review** - terse conventional-commit messages and one-line PR review comments.
- **Grill Me** - calibrated interview workflow that assesses knowledge and desired pressure before challenging a plan.
- **Junior to Senior** - adversarial senior review that upgrades agent-written plans using codebase + web research.
- **Context Canary** - per-turn first-line signal (name + turn counter + self-check) that dies visibly when context degrades, paired with a checkpoint-and-reset trip protocol.
- **Progressive disclosure** - agents read the smallest useful context first, then load linked references only as needed.

## Repository Shape

- `skills/` contains installable skill directories.
- `scripts/` contains repo maintenance helpers.
- `docs/adr/` records structural decisions.

