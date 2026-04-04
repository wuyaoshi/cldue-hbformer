# cldue-hbformer

This repository stores resumable session-state files for the HBFormer research workflow.

It is **not** the source-of-truth code repository. It is used to preserve project state across restarts so a future Claude session can quickly reload context.

## Core files

- `current/SESSION.md` — human-readable current state
- `current/STATE.json` — machine-readable state summary
- `current/NEXT_STEPS.md` — actionable next tasks
- `current/DECISIONS.md` — important project decisions
- `current/ENVIRONMENTS.md` — local/remote environment references

## Resume workflow

After restarting, ask Claude to read:

- `current/SESSION.md`
- `current/STATE.json`
- `current/NEXT_STEPS.md`

and continue the HBFormer work from there.
