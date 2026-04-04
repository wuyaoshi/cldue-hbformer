# Schema Notes

## V1 files
- `current/SESSION.md`: human-readable overall state
- `current/STATE.json`: machine-readable snapshot
- `current/NEXT_STEPS.md`: short actionable backlog
- `current/DECISIONS.md`: durable decisions
- `current/ENVIRONMENTS.md`: environment references

## Update rule
Update these files whenever there is a major experiment, decision, or checkpoint worth preserving across restarts.
