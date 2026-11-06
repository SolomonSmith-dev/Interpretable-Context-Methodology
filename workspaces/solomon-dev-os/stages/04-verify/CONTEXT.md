# Stage 04 — Verify

## Inputs

| Source | File/Location | Section/Scope | Why |
|--------|---------------|---------------|-----|
| Prior stage | `../03-build/output/` | Latest `*-build.md` | What changed |
| Brief | `../02-brief/output/` | Done means | Acceptance |
| Evals | `~/Projects/personal-tech-ops/evals/run.sh` | Relevant tasks | P0 gates |

## Process

1. Run the brief's Done checks and any named evals (`evals/run.sh` when ops touched).
2. Reviewer ≠ implementer when the brief requires it (Hermes reviewer profile or separate Cursor review).
3. Checkpoint on fail: Solomon chooses fix / ship with waiver / abort.
4. Write verify report.

## Outputs

| Artifact | Location | Format |
|----------|----------|--------|
| Verify report | `output/[slug]-verify.md` | PASS/FAIL per check + evidence |

## Checkpoints

- On any FAIL: stop for Solomon.

## Audit

- [ ] Every Done means line has evidence or FAIL
- [ ] No "looks good" without command/output proof
