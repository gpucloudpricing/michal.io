#multimodal #vlm

## TLDR
1. Labeling data sucks, we have paired image - text data that we can learn from in a "self" supervised fashion
2. Contrastive models are good for retrieval but:
	1. require huge batches to train
	2. collapse to bag of word model and don't have "semantic" understanding of images
3. Autoregressive Vision Language models learn richer representations of text and offer a lot of other advantages that come with next token prediction:
	1. in context learning
	2. prompting
3. LLaVA style architecture is standard (MLP to align pretrained vision encoder outputs with pretrained LLM inputs)
# Contrastive Vision Language Models

Train separate backbones for image and text, align them with a contrastive objective ala standard two tower approach

## CLIP

- [ ] https://github.com/mlfoundations/open_clip
- [ ] [GitHub - baaivision/EVA: EVA Series: Vision Foundation Model Fanatics from BAAI](https://github.com/baaivision/EVA)
- [ ] https://github.com/OpenAI/CLIP
- [ ] https://github.com/LAION-AI/CLIP_benchmark
- [ ] https://github.com/rom1504/clip-retrieval
- [ ] https://github.com/rom1504/laion-prepro
- [ ] [GitHub - yzhuoning/Awesome-CLIP: Awesome list for research on CLIP (Contrastive Language-Image Pre-Training).](https://github.com/yzhuoning/Awesome-CLIP)
- [ ] [e-CLIP: Large-Scale Vision-Language Representation Learning in E-commerce](http://arxiv.org/abs/2207.00208)
- [ ] [GitHub - facebookresearch/SLIP: Code release for SLIP Self-supervision meets Language-Image Pre-training](https://github.com/facebookresearch/SLIP)
- [ ] [GitHub - facebookresearch/flip: Official Open Source code for "Scaling Language-Image Pre-training via Masking"](https://github.com/facebookresearch/flip)
- [ ] [GitHub - facebookresearch/diht: Filtering, Distillation, and Hard Negatives for Vision-Language Pre-Training](https://github.com/facebookresearch/diht)
- [ ] [GitHub - OliverRensu/DeepMIM](https://github.com/OliverRensu/DeepMIM)
- [ ] [[2311.17049] MobileCLIP: Fast Image-Text Models through Multi-Modal Reinforced Training](https://arxiv.org/abs/2311.17049)
- [ ] [GitHub - bytedance/fc-clip: [NeurIPS 2023] This repo contains the code for our paper Convolutions Die Hard: Open-Vocabulary Segmentation with Single Frozen Convolutional CLIP](https://github.com/bytedance/fc-clip)
- [ ] [[2307.16634] CDUL: CLIP-Driven Unsupervised Learning for Multi-Label Image Classification](https://arxiv.org/abs/2307.16634)
- [ ] [[2309.05551] OpenFashionCLIP: Vision-and-Language Contrastive Learning with Open-Source Fashion Data](https://arxiv.org/abs/2309.05551)
- [ ] [\[2410.18857\] Probabilistic Language-Image Pre-Training](https://arxiv.org/abs/2410.18857)
- [ ] [\[2410.05270\] Fine-Tuning CLIP's Last Visual Projector: A Few-Shot Cornucopia](https://arxiv.org/abs/2410.05270)
![[Screenshot 2024-12-09 at 9.22.30 AM.png]]
## SigLIP


## Extensions
### FLAIR

![[Pasted image 20241207102401.png]]
![[Pasted image 20241207102313.png]]


# Autoregressive Vision Language Models

- [ ] [[2306.07915v3] Image Captioners Are Scalable Vision Learners Too](https://arxiv.org/abs/2306.07915v3)
- [ ] [[2311.03079] CogVLM: Visual Expert for Pretrained Language Models](https://arxiv.org/abs/2311.03079)
- [ ] [GitHub - OpenBMB/MiniCPM-V: MiniCPM-V 2.6: A GPT-4V Level MLLM for Single Image, Multi Image and Video on Your Phone](https://github.com/OpenBMB/MiniCPM-V/)
- [ ] [GitHub - FreedomIntelligence/LongLLaVA: LongLLaVA: Scaling Multi-modal LLMs to 1000 Images Efficiently via Hybrid Architecture](https://github.com/FreedomIntelligence/LongLLaVA)
- [ ] [[Stanford CS25: V4 I From Large Language Models to Large Multimodal Models - YouTube](https://www.youtube.com/watch?v=cYfKQ6YG9Qo)](https://www.youtube.com/watch?v=cYfKQ6YG9Qo)
- [ ] [Recent Advances on Multimodal Models Pre-training - YouTube](https://www.youtube.com/watch?v=g_RvHaIoZ2w)
- [ ] [GitHub - OpenGVLab/InternVL: \[CVPR 2024 Oral\] InternVL Family: A Pioneering Open-Source Alternative to GPT-4o. 接近GPT-4o表现的开源多模态对话模型](https://github.com/OpenGVLab/InternVL)

## CapPa

![[Pasted image 20241207095717.png]]

- [ ] [\[2306.07915v5\] Image Captioners Are Scalable Vision Learners Too](https://arxiv.org/abs/2306.07915v5)
- [ ] [Weights & Biases - # CapPa: Training vision models as captioners](https://wandb.ai/craiyon/cappa-jax/reports/CapPa-Training-vision-models-as-captioners--Vmlldzo4NDUyNDUz)

## LLaVA



### LLaVA-OneVision

![[Pasted image 20241207101105.png]]
- [ ] [\[2408.03326\] LLaVA-OneVision: Easy Visual Task Transfer](https://arxiv.org/abs/2408.03326)



- [ ] [\[2412.00876\] Dynamic-LLaVA: Efficient Multimodal Large Language Models via Dynamic Vision-language Context Sparsification](https://arxiv.org/abs/2412.00876)
## Flamingo

## Qwen2 VL

## Pixtral

## InternVL

### InternVL 2.5
![[Screenshot 2024-12-07 at 10.14.08 AM.png]]

- [ ] [InternVL/InternVL2\_5\_report.pdf at main · OpenGVLab/InternVL · GitHub](https://github.com/OpenGVLab/InternVL/blob/main/InternVL2_5_report.pdf)
## MiniCPM

## Molmo

![[Pasted image 20241207101640.png]]

![[Pasted image 20241207101651.png]]

![[Pasted image 20241207101739.png]]

## LLAMA 3.2 Vision

## Chameleon
![[Pasted image 20241207095931.png]]
- [ ] [\[2405.09818\] Chameleon: Mixed-Modal Early-Fusion Foundation Models](https://arxiv.org/abs/2405.09818)


## AIMv2 (Multimodal Autoregressive Pre-training of Large Vision Encoders)

- [ ] [GitHub - apple/ml-aim: This repository provides the code and model checkpoints for AIMv1 and AIMv2 research projects.](https://github.com/apple/ml-aim/tree/main)
- [ ] [\[2401.08541\] Scalable Pre-training of Large Autoregressive Image Models](https://arxiv.org/abs/2401.08541)

![[Pasted image 20241207100322.png]]


## Mixture-of-Transformer

![[Pasted image 20241207101225.png]]
![[Screenshot 2024-12-07 at 10.12.55 AM.png]]
## NVLM


## PaliGemma

## CogVLM

## Aria 

- [ ] [GitHub - rhymes-ai/Aria: Codebase for Aria - an Open Multimodal Native MoE](https://github.com/rhymes-ai/Aria)


## Florence-VL
- [ ] [\[2412.04424\] Florence-VL: Enhancing Vision-Language Models with Generative Vision Encoder and Depth-Breadth Fusion](https://arxiv.org/abs/2412.04424)
![[Pasted image 20241207225534.png]]

![[Pasted image 20241207225604.png]]

## SmolVLM

## Moondream


# Other Approaches

## Aligning Vision and LLMs
- [ ] [\[2412.04616\] Assessing and Learning Alignment of Unimodal Vision and Language Models](https://arxiv.org/abs/2412.04616)

## Multi Task / Combined Objectives

### VladVA

- [ ] [\[2412.04378\] Discriminative Fine-tuning of LVLMs](https://arxiv.org/abs/2412.04378)

![[Pasted image 20241207112708.png]]



## Generative VLMs

- [ ] [\[2412.03069\] TokenFlow: Unified Image Tokenizer for Multimodal Understanding and Generation](https://arxiv.org/abs/2412.03069)
- [ ] [\[2412.04332\] Liquid: Language Models are Scalable Multi-modal Generators](https://arxiv.org/abs/2412.04332)


- [ ] [[notes/ml/Generative Models|Generative Models]]
# Patterns

## Data Curation / Data Augmentation

### Filter for Quality

CLIP score to filter out web data that has captions that don't align with the image
### Expand Captions

Use existing VLMs to generate more detailed captions

## Modality Alignment

### MLP projection from Vision Backbone to LLM

## Image Encoding

### Multiple Resolutions, Scales and Aspect Ratios

### End of Row Encoding

### Positional Encodings

## Token Compression / Dropping
- [ ] [\[2412.04467\] VisionZip: Longer is Better but Not Necessary in Vision Language Models](https://arxiv.org/abs/2412.04467)

## Early vs Late Fusion


# Datasets

- [ ] https://github.com/rom1504/laion-prepro
- [ ] [GitHub - allenai/mmc4: MultimodalC4 is a multimodal extension of c4 that interleaves millions of images with text.](https://github.com/allenai/mmc4)
- [ ] [nyu-visionx/Cambrian-10M · Datasets at Hugging Face](https://huggingface.co/datasets/nyu-visionx/Cambrian-10M)
- [ ] [allenai/pixmo-cap-qa · Datasets at Hugging Face](https://huggingface.co/datasets/allenai/pixmo-cap-qa)



# Leaderboard / Benchmarks

- [ ] [GitHub - cambrian-mllm/cambrian: Cambrian-1 is a family of multimodal LLMs with a vision-centric design.](https://github.com/cambrian-mllm/cambrian)

# Links

- [ ] [GitHub - microsoft/BridgeTower: Open source code for AAAI 2023 Paper "BridgeTower: Building Bridges Between Encoders in Vision-Language Representation Learning"](https://github.com/microsoft/BridgeTower)
- [ ] [GitHub - microsoft/react](https://github.com/microsoft/react)
- [ ] https://github.com/salesforce/lavis
- [ ] https://github.com/uta-smile/TCL
- [ ] https://github.com/YehLi/xmodaler
- [ ] https://github.com/sangminwoo/awesome-vision-and-language
- [ ] [Masked Vision and Language Modeling for Multi-modal Representation Learning (2022-08-03)](https://arxiv.org/abs/2208.02131)
- [ ] [GitHub - facebookresearch/CiT: Code for the paper titled "CiT Curation in Training for Effective Vision-Language Data".](https://github.com/facebookresearch/CiT/tree/main)
- [ ] [GitHub - guilk/VLC: Research code for "Training Vision-Language Transformers from Captions Alone"](https://github.com/guilk/VLC)
- [ ] [GitHub - OliverRensu/TinyMIM](https://github.com/OliverRensu/TinyMIM)
- [ ] [GitHub - RERV/UniAdapter](https://github.com/RERV/UniAdapter)
- [ ] [\[2406.16860\] Cambrian-1: A Fully Open, Vision-Centric Exploration of Multimodal LLMs](https://arxiv.org/abs/2406.16860)