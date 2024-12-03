---
time_modified: 2024-10-13T01:44:12-04:00
time_created: 2024-10-03T23:15:33-04:00
---

1. pretraining
	1. filtered for quality
	2. include instruction tuning data
	3. synthetic data
	4. weighted sampling from different sources / categories
2. long context training
3. annealing with high quality data
4. supervised finetuning
5. RLHF / DPO


- [ ] [Common LLM Settings - Google Sheets](https://docs.google.com/spreadsheets/d/14vbBbuRMEHoqeuMHkTfw3uiZVmyXNuoSp8s-aHvfvZk/edit?gid=0#gid=0)

- [ ] [torchtune: Easy and Accessible Finetuning in Native PyTorch - Evan Smothers, Meta - YouTube](https://www.youtube.com/watch?v=43X9E25-Qg0)

![[Pasted image 20241003232836.png]]

# Optimizations

### Quantized Optimizers

### Fused Ops

- [ ] [GitHub - unslothai/unsloth: Finetune Llama 3.2, Mistral, Phi & Gemma LLMs 2-5x faster with 80% less memory](https://github.com/unslothai/unsloth/tree/main)
- [ ] [GitHub - linkedin/Liger-Kernel: Efficient Triton Kernels for LLM Training](https://github.com/linkedin/Liger-Kernel)

### Compile

### FlexAttention

Block causal mask  to pack samples
![[Pasted image 20241003232628.png]]


### Distributed

# Pretraining


# Finetuning


# Post Training / Alignment

[[Alignment and Post Training]]

