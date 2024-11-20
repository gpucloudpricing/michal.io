---
time_modified: 2024-11-03T14:21:40-04:00
time_created: 2024-11-03T13:35:39-04:00
---
#transformers

- [ ] replaces FFN and linear QKV mapping with an attention where keys and values are learned matrices
- [ ] allows scaling up the K and V matrices without a need to retrain
- [ ] ![[Screenshot 2024-11-03 at 1.43.53 PM.png]]![[Screenshot 2024-11-03 at 1.50.21 PM.png]]

![[Screenshot 2024-11-03 at 1.55.00 PM.png]]


- [ ] uses nonparametric layernorm so that only tokens are learned