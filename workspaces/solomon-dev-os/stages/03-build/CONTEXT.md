# Stage 03 — Build

## Inputs

| Source | File/Location | Section/Scope | Why |
|--------|---------------|---------------|-----|
| Prior stage | `../02-brief/output/` | Latest `*-brief.md` | Contract |
| Code graph | `<repo>/graphify-out/graph.json` | via `graphify query` | Architecture |
| Product repo | From brief | As named | Implementation |

## Process

1. Read brief. Do not expand scope.
2. **Codebase questions:** `graphify query "..."` in the target repo first. Only if graph missing or query fails, then limited file reads. Do **not** spawn explore/Task agents for "how does X work".
3. Implement on Hermes by default (D78). Cursor Task only for MAP/DECISIONS/`~/.hermes` or when Hermes cannot.
4. Keep diffs small. No secrets. No Co-Authored-By.
5. Write a build log to output (paths changed, commands, open risks).

## Outputs

| Artifact | Location | Format |
|----------|----------|--------|
| Build log | `output/[slug]-build.md` | Paths, commits/PRs, residual risk |

## Audit

- [ ] Brief Done means addressed or explicitly deferred with reason
- [ ] graphify used before broad search (or noted absent)
- [ ] No MAP/DECISIONS/~/.hermes edits without Solomon go
