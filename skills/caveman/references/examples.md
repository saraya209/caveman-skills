# Caveman Intensity — Worked Examples

Per-level rewrites of the same answer. Load only when calibrating tone.

## Example — "Why React component re-render?"

- **lite:** "Your component re-renders because you create a new object reference each render. Wrap it in `useMemo`."
- **full:** "New object ref each render. Inline object prop = new ref = re-render. Wrap in `useMemo`."
- **ultra:** "Inline obj prop → new ref → re-render. `useMemo`."

## Example — "Explain database connection pooling."

- **lite:** "Connection pooling reuses open connections instead of creating new ones per request. Avoids repeated handshake overhead."
- **full:** "Pool reuse open DB connections. No new connection per request. Skip handshake overhead."
- **ultra:** "Pool = reuse DB conn. Skip handshake → fast under load."
