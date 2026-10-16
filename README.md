# Qwen2.5-Coder-1.5B-Instruct — QLoRA Artifacts

Training-artifact repository for parameter-efficient fine-tuning of **Qwen/Qwen2.5-Coder-1.5B-Instruct** for code-repair experimentation.

## Verified configuration from the published adapter

- Base model: `Qwen/Qwen2.5-Coder-1.5B-Instruct`
- PEFT type: LoRA
- LoRA rank (`r`): 16
- LoRA alpha: 16
- LoRA dropout: 0.0
- Task type: causal language modeling
- Target modules include attention projections and MLP projections
- Published checkpoints include at least steps 700 and 800

## Repository contents

`outputs/qwen25-coder-1.5b_qlora/` contains adapter weights, tokenizer/configuration files, trainer state, optimizer/scheduler state, and checkpoint metadata.

## Important note

This repository stores training artifacts rather than a polished inference package. Large optimizer/checkpoint files make the repository heavy; future archival should keep the selected adapter and reproducibility metadata while moving unnecessary intermediate training state to external artifact storage.

## Related evaluation

See [Qwen2.5_Coder1.5B_Instruct_QLORA-RAG_testing](https://github.com/Alif-ziad/Qwen2.5_Coder1.5B_Instruct_QLORA-RAG_testing) for published RAG evaluation outputs.

## Author

MD Alif Ziad Sarkar — CSE, American International University-Bangladesh (AIUB)
