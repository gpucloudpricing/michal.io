---
time_modified: 2024-11-05T09:19:20-05:00
time_created: 2024-11-03T14:20:48-04:00
---


## Review of Architectures

- [ ] Network in Network 
	- [ ] 1x1 convs
- [ ] Resnet 
	- [ ] Residual Block 
	- [ ] Bottleneck Block
- [ ] SE Net
	- [ ] channel wise attention (global)
- [ ] MobileNetV2
	- [ ] inverted residual
	- [ ] depthwise convolutions
- [ ] 3x3 convs
	- [ ] winograd conv
- [ ] EfficientNet
	- [ ] poor comp efficiency on GPUs
- [ ] reducing activation size to reduce latency (due to memory movement and large intermediates)
- [ ] wider models have more compute per activation
- [ ] depth first execution of kernels to avoid large intermediate activations
	- [ ] can't be used for global ops like SE attention
- [ ] ConvNeXT
- [ ] ResNeXt
- [ ] 


## Contributions

- [ ] GPU kernels for fused FusedMBConv and MBConv blocks, exploiting temporal locality and reduce workspace size to avoid spilling to dram![[Screenshot 2024-11-03 at 2.56.55 PM.png]]![[Screenshot 2024-11-03 at 3.00.21 PM.png]]

![[Pasted image 20241103150830.png]]


instead use a fused kernel that computes in depth first fashion, getting rid of large intermediates



## ConvFirst Block
![[Screenshot 2024-11-03 at 3.16.22 PM.png]]



![[Pasted image 20241103152035.png]]![[Screenshot 2024-11-03 at 3.20.42 PM.png]]