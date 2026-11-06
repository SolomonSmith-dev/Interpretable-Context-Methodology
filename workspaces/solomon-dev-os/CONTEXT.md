# Solomon Dev OS — task routing

Sequential ship pipeline. Human edits any stage `output/` before the next stage.

## Task Routing

| Task Type | Go To | Description |
|-----------|-------|-------------|
| Orient on live state | `stages/01-orient/CONTEXT.md` | MAP where, NOW, Decisions, Hub/Kanban |
| Write a buildable brief | `stages/02-brief/CONTEXT.md` | Single-stage contract: goal, bans, done means |
| Implement | `stages/03-build/CONTEXT.md` | Hermes-first product code; graphify before explore agents |
| Verify | `stages/04-verify/CONTEXT.md` | Evals, map-check, smoke; implementer ≠ reviewer |
| Promote / record | `stages/05-promote/CONTEXT.md` | Claude-mem facts, vault note if durable, Decision/MAP if locked |

## Shared Resources

| Resource | Location | Contains |
|----------|----------|----------|
| Factory pointers | `_config/FACTORY.md` | Paths into personal-tech-ops, dotfiles, Hermes |
| North Star | `_config/NORTH_STAR.md` | D74–D84 summary (one page) |
| Playbooks | `~/dotfiles/skills/` | Procedural SoR (D82) — do not fork into this workspace |
