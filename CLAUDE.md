# Simian Strong

Single-file React PWA for logging strength workouts, deployed as a static site
on Netlify. Use the `simian-strong` agent (`.claude/agents/simian-strong.md`)
for work on this project — it documents the file layout, architecture and
working rules.

Quick facts:
- All app code is in `index.html` (compiled `React.createElement` style, no build step).
- Don't read `index.html` whole; grep for `^function ` and read ranges.
- Bump the cache version in `sw.js` on every shipped change.
- Verify syntax with `node --check` on the extracted last `<script>` block.
