---
time_modified: 2024-10-23T22:21:43-04:00
time_created: 2023-12-09T00:06:17-05:00
---
- [ ] [Diffusion Meets Flow Matching](https://diffusionflow.github.io/)
- [ ] [Perspectives on diffusion – Sander Dieleman](https://sander.ai/2023/07/20/perspectives.html)
- [ ] [YouTube - Diffusion Models from Scratch](https://youtu.be/B4oHJpEJBAA?si=iTiDR9_q-m4PfO83)
- [ ] [Google Colab](https://colab.research.google.com/drive/1EyqALXFvgKGsTiFDALGEHH5-WnuGjOKU?usp=sharing)
- [ ] [The Illustrated Stable Diffusion – Jay Alammar – Visualizing machine learning one concept at a time.](https://jalammar.github.io/illustrated-stable-diffusion/)
- [ ] [Lesson 9: Deep Learning Foundations to Stable Diffusion, 2022 - YouTube](https://www.youtube.com/watch?v=_7rMfsA24Ls)
- [ ] [Practical Deep Learning for Coders - 9: Stable Diffusion](https://course.fast.ai/Lessons/lesson9.html)
- [ ] [GitHub - CompVis/stable-diffusion](https://github.com/CompVis/stable-diffusion)
- [ ] [GitHub - huggingface/diffusion-models-class: Materials for the Hugging Face Diffusion Models Course](https://github.com/huggingface/diffusion-models-class)
- [ ] [Sana - Efficient High-Resolution Image Synthesis with Linear Diffusion Transformer](https://nvlabs.github.io/Sana/)
- [ ] [\[2410.07815\] Simple ReFlow: Improved Techniques for Fast Flow Models](https://arxiv.org/abs/2410.07815)
- [ ] [\[2410.10733v1\] Deep Compression Autoencoder for Efficient High-Resolution Diffusion Models](https://arxiv.org/abs/2410.10733v1)
- [ ] [\[2411.16318\] One Diffusion to Generate Them All](https://arxiv.org/abs/2411.16318)

- [ ] [CVPR Tutorial Diffusion-based Video Generative Models](https://cvpr.thecvf.com/virtual/2024/tutorial/23730)
- [ ] [23672 - 2nd Workshop on Generative Models for Computer Vision - YouTube](https://youtu.be/GEaSNJOpfsU?si=gc3AEzSy9Owm6Nsr&t=6650)

- [ ] [GitHub - openai/consistency_models: Official repo for consistency models.](https://github.com/openai/consistency_models)



- [ ] [Representation Alignment for Generation: Training Diffusion Transformers Is Easier Than You Think](https://sihyun.me/REPA/)



- [ ] textual inversion
	- [ ] optimize a new token embedding for new concept (an image is worth one word)
- [ ] ControlNet
	- [ ] Copies the model and grafts it onto existing frozen one and tunes it to condition on things like depth or edge maps
- [ ] DreamBooth
	- [ ] find unused tokens to map the concept onto, update (fine tune) the model
	- [ ] auxiliary loss to penalize drift for other concepts
- [ ] LoRA
	- [ ] zipLoRA
	- [ ] C-LoRA

## Unlearning
- [ ] optimize to maximize loss for given concept