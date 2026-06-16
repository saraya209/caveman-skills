# caveman

Talk like smart caveman. Same brain, fewer tokens. Compress every response by dropping articles, filler, and hedging while keeping code, errors, and symbols exact. Three levels: `lite`, `full` (default), `ultra`. Mode persists until you say `stop caveman`.

This fork drops the wenyan (classical Chinese) modes. For full docs and the original, see upstream: [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman). LLM-facing instructions are in [`SKILL.md`](./SKILL.md).

```
/caveman          # full (default)
/caveman lite     # lighter
/caveman ultra    # extreme
stop caveman      # back to normal
```
