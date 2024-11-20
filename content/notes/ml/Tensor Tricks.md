---
time_modified: 2024-10-17T14:37:51-04:00
time_created: 2024-10-17T12:24:12-04:00
---
#pytorch 

## Broadcasting

```python



```



## Selecting Samples

```python

batch[[1]]  # => (1, ...)
batch[1]  # => (...)
```


## New Axis == None

```python
batch = torch.randn((8, 3, 12))

batch[None]  # (1, 8, 3, 12)

batch[..., None]  # (8, 3, 12, 1)

batch[:, None]  # (8, 1, 3, 13)
```