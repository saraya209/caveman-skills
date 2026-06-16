# caveman-skills

Seven agent skills for Claude Code: terse communication and plan review.

> **Fork.** Skills come from [JuliusBrussee/skills](https://github.com/JuliusBrussee/skills) (caveman, grill-me, junior-to-senior, context-canary) and [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) (caveman-compress, caveman-commit, caveman-review). This fork drops the skills I don't use, removes the wenyan (classical Chinese) caveman modes, and runs `caveman-compress` inline with no external script or API key. Original work (c) Julius Brussee, MIT.

## Skills

| Skill | What it does |
|---|---|
| **caveman** | Compressed communication mode. Cuts token use (lite/full/ultra) and keeps code, commands, errors, and APIs exact. Stays on until "normal mode". |
| **caveman-compress** | Compresses natural-language memory files (CLAUDE.md, todos) into caveman-speak inline. Backs up the original and leaves code blocks untouched. |
| **caveman-commit** | Conventional-commit messages. Subject 50 chars or fewer; body only when the reason isn't obvious. |
| **caveman-review** | PR review comments, one line each: location, problem, fix. |
| **grill-me** | Stress-tests a plan or decision. Asks your knowledge level and how hard to push, then asks one question at a time with a recommended answer. |
| **junior-to-senior** | Senior-engineer review of agent-written plans, grounded in codebase research and current best practices. |
| **context-canary** | Per-turn signal that shows when context degrades in a long session, with a recovery protocol when it trips. |

## Install

```
/plugin marketplace add saraya209/caveman-skills
/plugin install caveman-skills
```

Skills are namespaced under the plugin (for example, `/caveman-skills:caveman`). Trigger them by intent or by their `/skill` name.

## Develop

```bash
node scripts/list-skills.mjs    # list skills
node scripts/verify-skills.mjs  # validate frontmatter + unique names
```

## Syncing upstream

```bash
git fetch upstream            # JuliusBrussee/skills
git merge upstream/main
```

`caveman`, `grill-me`, `junior-to-senior`, and `context-canary` track upstream. `caveman-compress`, `caveman-commit`, and `caveman-review` were copied from the caveman repo and have diverged (inline rewrite), so re-pull those by hand if you need upstream changes.

## License

MIT. See [LICENSE](LICENSE).
