---
time_modified: 2024-10-27T19:26:51-04:00
time_created: 2024-10-24T09:27:36-04:00
---


$$\text{logsumexp}(x_1, x_2, \dots, x_n) = \log \left( \sum_{i=1}^{n} e^{x_i} \right)$$


shifted with the logsumexp trick for stability

$$\text{logsumexp}(x_1, x_2, \dots, x_n) = \max_i x_i + \log \left( \sum_{i=1}^{n} e^{x_i - \max_j x_j} \right)$$

proof:

$$


\log \left( \sum_{i=1}^{n} e^{x_i} \right)

$$

$$
\log \left( \sum_{i=1}^{n} e^{x_i} \right) = \log \left( \sum_{i=1}^{n} e^{x_i - M} \cdot e^M \right)
$$


$$
= \log \left( e^M \sum_{i=1}^{n} e^{x_i - M} \right)
$$


$$
= \log(e^M) + \log \left( \sum_{i=1}^{n} e^{x_i - M} \right)
$$


$$
= M + \log \left( \sum_{i=1}^{n} e^{x_i - M} \right)
$$

$$
\log \left( \sum_{i=1}^{n} e^{x_i} \right) = \max_i x_i + \log \left( \sum_{i=1}^{n} e^{x_i - \max_j x_j} \right)
$$

