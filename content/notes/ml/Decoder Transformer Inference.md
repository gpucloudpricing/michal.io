---
time_modified: 2024-10-28T10:45:24-04:00
time_created: 2024-09-25T21:08:25-04:00
---
#inference #llm 


- [ ] [Transformer Inference Arithmetic | kipply's blog](https://kipp.ly/transformer-inference-arithmetic/)

![[Pasted image 20241003215519.png]]



Prefill vs generation, compute bound vs memory bound



## KV Cache

![[Pasted image 20241214102559.png]]

![[Pasted image 20241028094703.png]]

### Grouped Query Attention

Less Keys and Values, to reduce Key Value Cache

### Paged Attention
- [ ] [Fast LLM Serving with vLLM and PagedAttention - YouTube](https://www.youtube.com/watch?v=5ZlavKF_98U)

Avoid padding out samples with fixed size blocks, use proper paging, split up samples across smaller pages

### Sliding Window Attention => Rolling Buffer KV Cache
- [ ] [Exploring the Latency/Throughput & Cost Space for LLM Inference // Timothée Lacroix // CTO Mistral - YouTube](https://www.youtube.com/watch?v=mYRqvB1_gRk)
- [ ] [SKVQ: Sliding-window Key and Value Cache Quantization for Large Language Models - YouTube](https://www.youtube.com/watch?v=K8iqzH5pKkQ)

### Cross Layer KV Cache Sharing

- [ ] [\[2405.12981\] Reducing Transformer Key-Value Cache Size with Cross-Layer Attention](https://arxiv.org/abs/2405.12981)
![[Pasted image 20241003225937.png]]
[\[2405.05254\] You Only Cache Once: Decoder-Decoder Architectures for Language Models](https://arxiv.org/abs/2405.05254)


### StreamingLLM

See [[Long Context Transformers]]


### Prompt / Prefix Caching

Cache KV cache for common prefixes


### Low Precision and Compression

Use bf16, float8, int8 or smaller dtypes like int4 to save memory


![[Pasted image 20241028094817.png]]


- [ ] [GitHub - NVIDIA/kvpress: LLM KV cache compression made easy](https://github.com/NVIDIA/kvpress)

### Other
- [ ] [\[2410.03960\] SwiftKV: Fast Prefill-Optimized Inference with Knowledge-Preserving Model Transformation](https://arxiv.org/abs/2410.03960)

## Speculative Decoding


- [ ] [Dynamic Speculative Decoding](https://huggingface.co/blog/dynamic_speculation_lookahead)
- [ ] [How Speculative Decoding Boosts vLLM Performance by up to 2.8x | vLLM Blog](https://blog.vllm.ai/2024/10/17/spec-decode.html)


## Chunked Prefill (for batched inference)

Split up the prefill compute into chunks to reduce the units of work so that large prefills do not interfere with other request doing generation in the same batch

![[Pasted image 20241003220522.png]]

- [ ] [\[2403.02310\] Taming Throughput-Latency Tradeoff in LLM Inference with Sarathi-Serve](https://arxiv.org/abs/2403.02310)


## Disaggregated Prefill and Decoding

Do prefill on larger GPU then decode on smaller cheaper GPUs

- [ ] [\[2401.09670\] DistServe: Disaggregating Prefill and Decoding for Goodput-optimized Large Language Model Serving](https://arxiv.org/abs/2401.09670)
- [ ] [DistServe: disaggregating prefill and decoding for goodput-optimized LLM inference - YouTube](https://www.youtube.com/watch?v=Bh-jlh5vlF0)


## Prefix Caching


## Continuous Batching / Inflight Batching

- [ ] [Accelerating LLM Inference with vLLM - YouTube](https://www.youtube.com/watch?v=qBFENFjKE-M)

![[Pasted image 20241003220433.png]]



## Flash Attention


## Mixture of Experts
Reduce compute, skipping experts


See [[Mixture of Experts]]

## Quantization




## Structured Decoding / Generation


## LLM Routing
Predict best (speed / cost / expert) model for given request and route based on that

## Metrics

### Time to First Token

### Inter Token Latency


---
## Links
- [ ] [Understanding the LLM Inference Workload - Mark Moyou, NVIDIA - YouTube](https://www.youtube.com/watch?v=z2M8gKGYws4)
- [ ] [Mastering LLM Techniques: Inference Optimization | NVIDIA Technical Blog](https://developer.nvidia.com/blog/mastering-llm-techniques-inference-optimization/)
- [ ] [Optimizing AI Inference at Character.AI](https://research.character.ai/optimizing-inference/)
- [ ] [\[2402.16363\] LLM Inference Unveiled: Survey and Roofline Model Insights](https://arxiv.org/abs/2402.16363)
- [ ] [\[2407.12391\] LLM Inference Serving: Survey of Recent Advances and Opportunities](https://arxiv.org/abs/2407.12391)