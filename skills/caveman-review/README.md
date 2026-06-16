# caveman-review

One-line PR comments: location, problem, fix. Format is `L<line>: <severity> <problem>. <fix>.`, one line per finding. Drops "I noticed that", hedging, and restating the diff. Keeps line numbers, backticked symbols, and concrete fixes. Output only; does not approve, request changes, or run linters.

For full docs and the original, see upstream: [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman). LLM-facing instructions are in [`SKILL.md`](./SKILL.md).

```
/caveman-review
```
