# Solomon Dev OS (ICM workspace)

Interpretable Context Methodology workspace for Solomon's Dual Develop stack. One agent reads the right files at each stage. Do **not** spawn Task/explore agents for codebase questions when `graphify-out/` exists — use `graphify query` first.

Upstream: https://github.com/RinDig/Interpretable-Context-Methodology  
Paper: https://arxiv.org/abs/2603.16021

## Folder Map

```
solomon-dev-os/
├── CLAUDE.md
├── CONTEXT.md
├── setup/questionnaire.md
├── _config/                 # factory: pointers into personal-tech-ops
├── shared/
├── skills/                  # pointers only — SoR is ~/dotfiles/skills
└── stages/
    ├── 01-orient/
    ├── 02-brief/
    ├── 03-build/
    ├── 04-verify/
    └── 05-promote/
```

## Triggers

| Keyword | Action |
|---------|--------|
| `setup` | Run `setup/questionnaire.md` once — configure factory prefs |
| `status` | Scan `stages/*/output/` — COMPLETE if files besides `.gitkeep`, else PENDING |
| `next` | Run the first PENDING stage CONTEXT.md |

## Hard bans (Solomon)

- No second kanban store. Hermes Kanban is card SoR (D83).
- MAP / DECISIONS / `~/.hermes` edits only via Cursor Task after Solomon says go (D78).
- No secrets in stage outputs. Names/paths only.
- Team L / `team-l-loop` is killed — do not reinstall.
