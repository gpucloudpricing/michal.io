---
time_modified: 2024-10-15T09:03:59-04:00
time_created: 2024-09-27T23:34:59-04:00
---

# Indexing and Retrieval

## Full Text Search

### BM25

### TF-IDF



## Vector Search

### Indexes

#### HNSW


#### IVF-Flat

#### LO-PQ


### Chunking

#### Fixed Sized Window

#### Sentence Splitting


#### Late Chunking

Use long context text embedding model, then pool output word embedding with a smaller window. This gives you a a full document contextualized embedding of the smaller section of the document

![Comparative panels display Berlin's Wikipedia article and its chunked text to highlight clarity and readability benefits.](https://jina-ai-gmbh.ghost.io/content/images/2024/08/image-3.png)


![Flowchart comparing naive and late chunking methods in document processing with labeled steps and embeddings.](https://jina-ai-gmbh.ghost.io/content/images/2024/08/Diagram--Blog-images--4-.svg)


- [ ] [Late Chunking in Long-Context Embedding Models](https://jina.ai/news/late-chunking-in-long-context-embedding-models/)
- [ ] [\[2409.04701\] Late Chunking: Contextual Chunk Embeddings Using Long-Context Embedding Models](https://arxiv.org/abs/2409.04701)


#### Contextual Retrieval

Use an LLM to enrich the chunked segment with info from the whole document

![[Pasted image 20241201221242.png]]

- [ ] [Introducing Contextual Retrieval \\ Anthropic](https://www.anthropic.com/news/contextual-retrieval)

## Embedding Models

### Contextual Document Embeddings

###  Matryoshka Embeddings

- [ ] [\[2205.13147\] Matryoshka Representation Learning](https://arxiv.org/abs/2205.13147)


### Gecko - Versatile Text Embeddings Distilled from Large Language Models

[[Gecko - Versatile Text Embeddings Distilled from Large Language Models]]

### Binary Embeddings



## Ranking / Reranking

![[Pasted image 20241201204207.png]]

### Biencoders

### CrossEncoders

### Colbert (Late Interaction)

### SPLADE
- [ ] [\[2109.10086\] SPLADE v2: Sparse Lexical and Expansion Model for Information Retrieval](https://arxiv.org/abs/2109.10086)
- [ ] [SPLADE for Sparse Vector Search Explained | Pinecone](https://www.pinecone.io/learn/splade/)

### DRAGON
- [ ] [\[2302.07452\] How to Train Your DRAGON: Diverse Augmentation Towards Generalizable Dense Retrieval](https://arxiv.org/abs/2302.07452)

## Query Understanding / Rewriting / Expansion


## Index Expansion / Document Augmentation

- [ ] extract keywords, summaries, facts using llm
- [ ] augment with synonyms using llm

## Retrieval Eval

### nDCG

### mAP

### MRR

### Recall@K

### Precision@K



# Function Calling



# Structured Generation


# Prompt Engineering

## In-context learning

Show input output examples for "few shot" learning

## Chain of Thought


## DSPy


## Hacks

### Repeat Prompt

By repeating input twice you allow decoder to do "bidirectional" attention instead of causal

### Move Question to Top

With causal attention it's better to ask then show context so that future tokens are aware of what they should be looking for.

Can also help to have the question and start and end

### Short Output Formats

Speed up generation by asking LLM to as an example output csv data instead of JSON since it's a lot less tokens

### Ask the LLM to rewrite the prompt



# Document Parsing



# Multimodal Rag

## ColPali and ColQwen




# End to End LLMs with Retrieval

[[Retrieval Augmented Models]]

## kNN-LM

## REALM
- [ ] [\[2002.08909\] REALM: Retrieval-Augmented Language Model Pre-Training](https://arxiv.org/abs/2002.08909)
![[Pasted image 20241201210544.png]]

## RETRO 

![[Pasted image 20241201210026.png]]

## RETRO++
- [ ] [\[2304.06762\] Shall We Pretrain Autoregressive Language Models with Retrieval? A Comprehensive Study](https://arxiv.org/abs/2304.06762)



# RAG Evaluation

## LLM as Judge





# Inference Optimizations

## Prefix Caching

## Batch Processing






- [ ] [\[2411.02959\] HtmlRAG: HTML is Better Than Plain Text for Modeling Retrieved Knowledge in RAG Systems](https://arxiv.org/abs/2411.02959)

- [ ] https://www.anthropic.com/news/contextual-retrieval
- [ ] [\[2409.13385\] Contextual Compression in Retrieval-Augmented Generation for Large Language Models: A Survey](https://arxiv.org/abs/2409.13385)
- [ ] [\[2409.14924\] Retrieval Augmented Generation (RAG) and Beyond: A Comprehensive Survey on How to Make your LLMs use External Data More Wisely](https://arxiv.org/abs/2409.14924)
- [ ] [GitHub - NirDiamant/RAG\_Techniques: This repository showcases various advanced techniques for Retrieval-Augmented Generation (RAG) systems. RAG systems combine information retrieval with generative models to provide accurate and contextually rich responses.](https://github.com/NirDiamant/RAG_Techniques)


- [ ] [What Late Chunking Really Is & What It’s Not: Part II](https://jina.ai/news/what-late-chunking-really-is-and-what-its-not-part-ii/)
- [ ] [Stanford CS25: V3 I Retrieval Augmented Language Models - YouTube](https://www.youtube.com/watch?v=mE7IDf2SmJg)



- [ ] [GitHub - athina-ai/rag-cookbooks: This repository contains various advanced techniques for Retrieval-Augmented Generation (RAG) systems.](https://github.com/athina-ai/rag-cookbooks)