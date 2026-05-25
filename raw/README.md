# CCC Raw Input

Write notes here in plain markdown. When you're ready to update the dashboard, paste the relevant raw file into a Claude session and say "update wiki/career.json from this" or "update wiki/interview.json from this". Claude will rewrite the JSON and the dashboard will pick up the changes on next load.

## Files

| File | Updates | Dashboard section |
|------|---------|-------------------|
| `career.md` | `wiki/career.json` | Career tab (timeline, skills, quals, milestones, projects) |
| `interview-prep.md` | `wiki/interview.json` | Interview Engine (Q bank, workplace Q bank) |

## Workflow

1. Edit a file in `raw/`
2. Paste it into Claude: "update wiki/career.json from raw/career.md"
3. Claude rewrites the JSON
4. Commit and push: `git add . && git commit -m "update" && git push`
5. Reload the dashboard — data is live

## Direct JSON editing

You can also edit `wiki/*.json` directly if you know what you want to change. The format is self-explanatory — just follow the existing structure.

## Colours for experience timeline

| Company tier | Hex |
|---|---|
| Current / target role | `#58a6ff` (blue) |
| Previous / secondary | `#d29922` (amber) |
| Early career | `#3fb950` (green) |
| Other | `#a5a0ff` (purple) |
