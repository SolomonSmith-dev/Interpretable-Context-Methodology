# Stage 05 — Promote

## Inputs

| Source | File/Location | Section/Scope | Why |
|--------|---------------|---------------|-----|
| Prior stages | `../01-orient/output/` … `../04-verify/output/` | Latest slug set | Record set |
| Save skill | `~/dotfiles/skills/save/SKILL.md` | Destinations | Routing |

## Process

1. Only after verify PASS (or Solomon waiver).
2. Claude-mem: one-line facts/decisions/corrections only (no instructions-to-act).
3. Vault: durable notes → `025-AI-Notes/` with `ai_generated: true` — never Inbox/020-Notes.
4. Ops: Decision/MAP/PR only if a lock changed — Cursor Task after go.
5. Graphify: `graphify update <repo>` for code repos that changed.
6. Write promote receipt.

## Outputs

| Artifact | Location | Format |
|----------|----------|--------|
| Promote receipt | `output/[slug]-promote.md` | What was written where (ids/paths) |

## Audit

- [ ] No secrets saved
- [ ] Ops items listed if not written here
- [ ] Pipeline slug marked complete
