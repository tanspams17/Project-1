---
description: Run a UI/UX Pro Max design-system search (styles, colors, typography, UX rules) for the given query.
---

Run the ui-skill design-intelligence search for this request: $ARGUMENTS

1. From the repo root, run (try `python3`, fall back to `python` or `py -3` if not found):
   ```bash
   python3 .claude/skills/ui-skill/scripts/search.py "$ARGUMENTS" --design-system
   ```
2. If the project's stack is detectable (package.json, pubspec.yaml, composer.json, etc.), also run:
   ```bash
   python3 .claude/skills/ui-skill/scripts/search.py "$ARGUMENTS" --stack <detected-stack>
   ```
3. Present the recommendations (pattern, style, colors, typography, effects, anti-patterns) directly. If a search returns 0 results, say so explicitly and retry once with broader keywords rather than fabricating output.
