# caveman-compress

Compress project memory files (`CLAUDE.md`, todos, preferences) into caveman format so each session load fewer tokens. Original saved as `FILE.original.md`; code blocks, URLs, and paths stay exact.

This fork run compression inline (no script, API key, or subprocess). For full docs, benchmarks, and the original version, see upstream: [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman).

```
/caveman-compress CLAUDE.md
```
