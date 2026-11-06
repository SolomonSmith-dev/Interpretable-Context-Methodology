# Stage 01 — Orient

## Inputs

| Source | File/Location | Section/Scope | Why |
|--------|---------------|---------------|-----|
| Factory | `../../_config/FACTORY.md` | Full | Path SoR |
| North Star | `../../_config/NORTH_STAR.md` | Full | Locked decisions |
| Live state | `~/Projects/personal-tech-ops/NOW.md` | Top + Active | What is live |
| MAP | run `map-check where <name>` or read MAP.md | Named ids only | Location truth |
| Kanban | `hermes kanban boards list` + current board stats | Counts + blocked | Work truth |

## Process

1. Load Layer 0–2 only until you know the task slug.
2. Resolve where the work lives via MAP / map-check — never invent paths.
3. Note blockers on Hermes Kanban (especially `solomon` / needs_input).
4. Write a short orientation brief to output.

## Outputs

| Artifact | Location | Format |
|----------|----------|--------|
| Orientation | `output/[slug]-orient.md` | Markdown: goal guess, paths, blockers, next stage |

## Audit

- [ ] Every path cited exists or is marked unresolved
- [ ] No secrets
- [ ] Explicit "ready for 02-brief" or "stop — need Solomon"
