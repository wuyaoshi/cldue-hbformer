# Decisions

- This repository is for **session-state persistence**, not for storing the HBFormer source code.
- The initial implementation is **V1 basic mode**: durable status files only, no hooks yet.
- The remote runtime to treat as primary execution environment is the AutoDL 3080 Ti server.
- For iterative-refinement experiments, prefer creating a new config over overwriting the current 2-iteration baseline.
