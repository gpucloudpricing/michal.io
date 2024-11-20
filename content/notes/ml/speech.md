---
time_modified: 2024-10-27T19:26:42-04:00
time_created: 2023-12-09T00:06:17-05:00
---
## Speech Recognition
#asr 

- [ ] [Open ASR Leaderboard - a Hugging Face Space by hf-audio](https://huggingface.co/spaces/hf-audio/open_asr_leaderboard)

- [ ] https://github.com/openai/whisper
- [ ] https://github.com/ggerganov/whisper.cpp
- [ ] [ylacombe/whisper-large-v3-turbo · Hugging Face](https://huggingface.co/ylacombe/whisper-large-v3-turbo)
- [ ] [nvidia/canary-1b · Hugging Face](https://huggingface.co/nvidia/canary-1b)
- [ ] [Whisper - a mlx-community Collection](https://huggingface.co/collections/mlx-community/whisper-663256f9964fbb1177db93dc)


- [ ] [GitHub - sindresorhus/awesome-whisper: 🔊 Awesome list for Whisper — an open-source AI-powered speech recognition system developed by OpenAI](https://github.com/sindresorhus/awesome-whisper)


### Transducers - RNN-T

Separate source encoder for input sequence and "predictor" model that only predicts next token in output space (LLM), with a "Joiner" module that takes the encoder and predictor outputs and combines them to predict the next output.

- [ ] good for streaming
- [ ] + can pretrain the predictor in self supervised fashion on next token prediction

- [ ] [Sequence-to-sequence learning with Transducers - Loren Lugosch](https://lorenlugosch.github.io/posts/2020/11/transducer/)
- [ ] [In Depth Explaination Of RNN-T based Automatic Speech Recognition Systems (ASR) - YouTube](https://www.youtube.com/playlist?list=PLapTxW9vHtzqMo6gS5zyn5YCNrz2xAm9W)
	- [ ] [sites.cc.gatech.edu/classes/AY2021/cs7643\_spring/assets/L24\_rnnt\_asr\_tutorial\_gt.pdf](https://sites.cc.gatech.edu/classes/AY2021/cs7643_spring/assets/L24_rnnt_asr_tutorial_gt.pdf)

### HuBERT
- [ ] [\[2106.07447\] HuBERT: Self-Supervised Speech Representation Learning by Masked Prediction of Hidden Units](https://arxiv.org/abs/2106.07447)

### CTC


### Decoding

#### Greedy

#### Beam Search

### Conformer

- [ ] [\[2005.08100\] Conformer: Convolution-augmented Transformer for Speech Recognition](https://arxiv.org/abs/2005.08100)




### Whisper


### Mamba 

## TTS - Text to Speech
- [ ] [TTS Arena - a Hugging Face Space by TTS-AGI](https://huggingface.co/spaces/TTS-AGI/TTS-Arena)


### F5-TTS

- [ ] [\[2410.06885\] F5-TTS: A Fairytaler that Fakes Fluent and Faithful Speech with Flow Matching](https://arxiv.org/abs/2410.06885)

![[Pasted image 20241024204525.png]]
## End to End Multimodal Speech to Speech

### Spirit LM

- [ ] [GitHub - facebookresearch/spiritlm: Inference code for the paper "Spirit-LM Interleaved Spoken and Written Language Model".](https://github.com/facebookresearch/spiritlm)
- [ ] [SpiRit-LM, an Interleaved Spoken and Written Language Model | Multimodal Weekly 47 - YouTube](https://youtu.be/oL5YoLNfdJM?si=A-eti-CncqxfXGfC)




## Links

- [ ] [Olewave - YouTube](https://www.youtube.com/@olewave/videos)
- [ ] [WAVLab - YouTube](https://www.youtube.com/@wavlab3016/videos)