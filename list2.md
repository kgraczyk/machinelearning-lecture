## List 2 (6 pt.)

### __Problem 2.1__ (1 pt.)
Compute the integral\
$$\int_0^\infty d x \exp( - a x^2)$$

### __Problem 2.2__ (1 pt.)

Let $P(x)$ and $Q(x)$ be probability distributions defined over the same domain. The relative entropy between $Q$ and $P$ is defined as:
	 	
$$D_{KL} (Q\mid \mid P) = \sum_x Q(x) \ln \frac{Q(x)}{P(x)} $$

Show that relative entropy is always positive.

### __Problem 2.3__ (1 pt.)
Let us introduce the free energy:\
$$\tilde{F}(w)= \sum_x Q(x;w)\ln\frac{Q(x,w)}{\exp(-\beta H(x,w))}$$

Show that the energy $\tilde{F}$ upper bounds the free energy $F$.

Note that $P(x,w) = \exp(-\beta H(x,w))/Z$, $Q$ is the probability defined on the same domain as $P$

### __Problem 2.4__ (1 pt.)
Given the function

$$
G(\mathbf{w})=-\frac{1}{2} \sum_{i}^N \sum_{\mu =1}^p\left\{ (1+\xi_i^\mu) \ln\left[ \frac{1}{2}(1+S_i^\mu)\right]+(1 - \xi_i^\mu) \ln\left[ \frac{1}{2}(1-S_i^\mu) \right]
\right\},
$$

  
where $\xi_i^\mu$ is the pattern to be memorized, and $S_i^\mu = \tanh(h_i^\mu/2)$ is the network response,
$h_i^{\mu} = \sum_{j} w_{ij} \xi_i^\mu$.

Compute the derivative\
$$\frac{\partial G(\mathbf{w})}{\partial w_{k m}} =? $$

### __Problem 2.5__ (**2 pt.**)
Consider the Hopfield network. Consider two new patterns and check the network's ability to memorize with synchronous and asynchronous updating.

Additional patterns (Python):
```python
p5=np.array([[1,-1,1,-1,1],[-1,1,-1,1,-1],[1,-1,1,-1,1],[-1,1,-1,1,-1],[1,-1,1,-1,1]])

p6=np.array([[1,-1,-1,-1,1],[-1,1,1,1,1],[1,-1,-1,-1,1],[1,1,1,1,-1],[1,-1,-1,-1,1]])```



