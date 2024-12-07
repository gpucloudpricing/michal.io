#vlm



## PaliGemma 2

### TLDR
1. Take pretrained SigLip Model and Gemma LLM, add linear projection from SigLip tokens to Gemma
2. Train whole thing end to end on 224x224 resolution (1 Billion Examples)
3. Tune at larger resolutions (50 mil at 448, then 10 mil at 896)
	1. sample tasks that require larger resolution like OCR
2. Tune for downstream tasks

- [ ] [\[2412.03555\] PaliGemma 2: A Family of Versatile VLMs for Transfer](https://arxiv.org/abs/2412.03555)
- [ ] [Welcome PaliGemma 2 – New vision language models by Google](https://huggingface.co/blog/paligemma2)

![[Pasted image 20241205131908.png]]

![[Pasted image 20241205132830.png]]

![[Pasted image 20241205132839.png]]


![](https://x.com/AndreasPSteiner/status/1864729070526681510)