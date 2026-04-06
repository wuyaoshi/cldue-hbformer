# Decisions

- This repository is for **session-state persistence**, not for storing the HBFormer source code.
- The initial implementation is **V1 basic mode**: durable status files only, no hooks yet.
- The remote runtime to treat as primary execution environment was first the AutoDL 3080 Ti server, and a cloned AutoDL machine was later used for additional testing.
- For iterative-refinement experiments, prefer creating a new config over overwriting the current 2-iteration baseline.
- For thesis Chapter 4 drafting, the adopted chapter model name should be written simply as **HBFormer**.
- For thesis Chapter 4 drafting, the adopted quantitative results should come from the HBFormer 3-iteration experiment, but the text should not append the phrase `3-iteration` to the displayed model name.
