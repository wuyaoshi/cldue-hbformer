# HBFormer Session

## Current focus
Establish a resumable session-state workflow for the HBFormer project and preserve the latest experiment state.

## Established facts
- The active research project is `HBFormer`.
- The main remote runtime is the AutoDL 3080 Ti server.
- The HBFormer training run at `/root/HBFormer/outputs/hbformer_base` has completed.
- The best training Dice recorded in the train log is `0.9274`.
- Evaluation with `best_model.pt` has already been run across five test datasets.

## Important paths
- Remote project: `/root/HBFormer`
- Remote outputs: `/root/HBFormer/outputs/hbformer_base`
- Best checkpoint: `/root/HBFormer/outputs/hbformer_base/checkpoints/best_model.pt`
- Latest checkpoint: `/root/HBFormer/outputs/hbformer_base/checkpoints/checkpoint_latest.pt`
- Local mirror: `/home/dawn/文档/HBFormer`
- Session-state repo: `/home/dawn/文档/cldue-hbformer`

## Latest results
- Training status: completed at 200 epochs
- Best Dice in training log: `0.9274`
- Test Avg mDice: `0.8573`
- Test Avg mIoU: `0.7948`
- Dataset Dice:
  - Kvasir: `0.9130`
  - CVC-ClinicDB: `0.9170`
  - CVC-ColonDB: `0.7803`
  - ETIS-LaribPolypDB: `0.8043`
  - CVC-300: `0.8717`

## Open questions
- Whether to keep the current 2-iteration setup as the fixed baseline.
- Whether to add a separate 3-iteration experiment config.
- Why `CVC-ColonDB` is substantially weaker than the stronger datasets.

## Recommended next action
Add a separate 3-iteration experiment config without overwriting the current 2-iteration baseline, then compare metrics and resource cost.
