---
time_modified: 2024-10-04T00:37:41-04:00
time_created: 2024-10-04T00:22:47-04:00
---
- [ ] [\[2410.02749\] Training Language Models on Synthetic Edit Sequences Improves Code Synthesis](https://arxiv.org/abs//2410.02749)
- [ ] [x.com](https://x.com/jnsgehring/status/1842002155030380920)
- [ ] [\[2410.02089\] RLEF: Grounding Code LLMs in Execution Feedback with Reinforcement Learning](https://arxiv.org/abs/2410.02089)



- [ ] [NeurIPS Competition HAC: The Hacker-Cup AI Competition](https://neurips.cc/virtual/2024/competition/84789)

## Code Embedding Models

- [ ] [voyage-code-3: more accurate code retrieval with lower dimensional, quantized embeddings – Voyage AI](https://blog.voyageai.com/2024/12/04/voyage-code-3/)


## Synthetic Tasks
- [ ] remove function body, implement it, validate output against original function
- [ ] corrupt function, have LLM find and fix mistakes (AST based)
- [ ] translate code into other languages
- [ ] commit => describe issue => implement commit
- [ ] make up tasks => write tests => implement code
- [ ] fill in the middle tasks
- [ ] learn to optimize, best of N implementation to write faster version of existing functions
- [ ] existing code => tests => new code
- [ ] parser guided generation (reject paths that can't parse)
	- [ ] [GitHub - tree-sitter/tree-sitter: An incremental parsing system for programming tools](https://github.com/tree-sitter/tree-sitter)
	- [ ] [GitHub - lark-parser/lark: Lark is a parsing toolkit for Python, built with a focus on ergonomics, performance and modularity.](https://github.com/lark-parser/lark)
	- [ ] [GitHub - amazon-science/incremental-parsing: Incremental Python parser for constrained generation of code by LLMs.](https://github.com/amazon-science/incremental-parsing)
- [ ] structured generation (grammar based) [[Structured Generation with LLMs]]