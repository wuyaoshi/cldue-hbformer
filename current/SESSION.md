# HBFormer Session

## Current focus
Use HBFormer as Chapter 4 of the master's thesis and preserve the latest comparative experiment state across restarts.

## Established facts
- The active research project is `HBFormer`.
- The primary earlier runtime was the AutoDL 3080 Ti server.
- A cloned AutoDL machine was also used to run the final 3-iteration test.
- The HBFormer 2-iteration run at `/root/HBFormer/outputs/hbformer_base` completed and was fully evaluated.
- The HBFormer 3-iteration run at `/root/HBFormer/outputs/hbformer_3iter` completed and was fully evaluated.
- The thesis-writing instruction is to write Chapter 4 using the model name **HBFormer** without appending the phrase `3-iteration`, even though the adopted chapter data comes from the 3-iteration experiment.

## Important paths
- Local HBFormer mirror: `/home/dawn/文档/HBFormer`
- Session-state repo: `/home/dawn/文档/cldue-hbformer`
- Thesis source docx: `/home/dawn/文档/非全日制硕士学位论文.docx`
- BoundFormer comparison log: `/home/dawn/文档/BoundFormer/outputs/boundformer_small_b4/test.log`
- HBFormer 3-iteration config: `/home/dawn/文档/HBFormer/configs/experiments/hbformer_3iter.yaml`

## Latest results
### HBFormer (2-iteration baseline)
- Best training Dice: `0.9274`
- Test Avg mDice: `0.8573`
- Test Avg mIoU: `0.7948`
- Dataset Dice:
  - Kvasir: `0.9130`
  - CVC-ClinicDB: `0.9170`
  - CVC-ColonDB: `0.7803`
  - ETIS-LaribPolypDB: `0.8043`
  - CVC-300: `0.8717`

### HBFormer (3-iteration experiment, to be written simply as HBFormer in Chapter 4)
- Best training Dice: `0.9220`
- Test Avg mDice: `0.8623`
- Test Avg mIoU: `0.7967`
- Dataset Dice:
  - Kvasir: `0.9173`
  - CVC-ClinicDB: `0.9206`
  - CVC-ColonDB: `0.7960`
  - ETIS-LaribPolypDB: `0.7876`
  - CVC-300: `0.8899`

### BoundFormer comparison result currently referenced
- Test Avg mDice: `0.8667`
- Test Avg mIoU: `0.8051`
- Dataset Dice:
  - Kvasir: `0.9297`
  - CVC-ClinicDB: `0.9141`
  - CVC-ColonDB: `0.7865`
  - ETIS-LaribPolypDB: `0.8019`
  - CVC-300: `0.9013`

## Open questions
- Whether the Chapter 4 comparison should explicitly mention that the adopted HBFormer numbers come from the 3-iteration setting, while the displayed model name remains just `HBFormer`.
- How to explain that HBFormer improves over the 2-iteration baseline on test average but still does not exceed the current BoundFormer small_b4 comparison result.
- Whether a fair same-backbone BoundFormer baseline should be added later for a stricter comparison.

## Recommended next action
Write a new standalone Chapter 4 draft file that presents HBFormer as the chapter model name, uses the 3-iteration test results as the adopted HBFormer quantitative results, and does not modify the original thesis docx yet.
