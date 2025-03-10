# Machine Learning Lecture 2025

---

## List 1 (5 pt.)

* __Problem 1.1__ (1pt.)

  Let a Hopfield network have N nodes. How many weights does a network with symmetric connections have, and how many weights does a network with bidirectional connections have? Answer and justify with a calculation.  

* __Problem 1.2__ (1pt.)
  According to Hebb's rule, the weights of the connections in a Hopfield network are updated according to the formula:\
  $$w_{ij} = \frac{1}{N}\sum_{\mu=1}^p \xi^\mu_i \xi^\mu_j.$$
     
  We can slightly generalize the above rule and assume that\
  $$w_{ij} = \eta \sum_{\mu=1}^p \xi^\mu_i \xi^\mu_j, \quad \eta >0
  $$\
  Does the magnitude of  $\eta$ matter? Why was  $\eta=1/N$ chosen? Provide a short explanation with a calculation.

* __Problem 1.3__ (1pt.)
  Show that if a Hopfield network does not have symmetric connections, then the learning update process may not lead to convergent states. Solve the problem by constructing a two-node neural network.

* __Problem 1.3__ (1pt.)
  Show that if a Hopfield network is trained synchronously, it may not lead to convergent states. Solve the problem by constructing a two-node neural network.

* __Problem 1.4__ (1pt.)
  Show that if the initial pattern $S_i$ has at most half of its bits differing from the pattern $\xi_j$, Hebb's rule will still lead the state $S_i$ to the pattern $xi_j$.

* __Problem 1.5__ (1pt.)
  Calculate the first and second moments for the binomial distribution and the variance.

---

## List 2 (6 pt.)

* __Problem 2.1__ (1 pt.)
  Compute the integral\
  $$\int_0^\infty d x \exp( - a x^2)$$

* __Problem 2.2__ (1 pt.)

  Let $P(x)$ and $Q(x)$ be probability distributions defined over the same domain. The relative entropy between $Q$ and $P$ is defined as:
	 	
  $$D_{KL} (Q\mid \mid P) = \sum_x Q(x) \ln \frac{Q(x)}{P(x)} $$

  Show that relative entropy is always positive.

* __Problem 2.3__ (1 pt.)
  Let us introduce the free energy:\
  $$\tilde{F}(w)= \sum_x Q(x;w)\ln\frac{Q(x,w)}{\exp(-\beta H(x,w))}$$

  Show that the energy $\tilde{F}$ upper bounds the free energy $F$.

  Note that $P(x,w) = \exp(-\beta H(x,w))/Z$, $Q$ is the probability defined on the same domain as $P$

* __Problem 2.4__ (1 pt.)
  Given the function\
  $$G(\mathbf{w}) = - \frac{1}{2} \sum_{i}^N \sum_{ \mu =1}^p  \left\{ (1 + \xi_i^\mu) \ln\left[ \frac{1}{2}(1+S_i^\mu) \right] +(1 - \xi_i^\mu) \ln\left[ \frac{1}{2}(1-S_i^\mu)\right] \right\},$$
  where $\xi_i^\mu$ is the pattern to be memorized, and $S_i^\mu = \tanh(h_i^\mu/2)$ is the network response,
  $h_i^{\mu} = \sum_{j} w_{ij} \xi_i^\mu$.

  Compute the derivative\
  $$\frac{\partial G(\mathbf{w})}{\partial w_{k m}} =? $$

* __Problem 2.5__ (**2 pt.**)
  Consider the Hopfield network. Consider two new patterns and check the network's ability to memorize with synchronous and asynchronous updating.

  Additional patterns (Python):
  ```python
  p5=np.array([[1,-1,1,-1,1],[-1,1,-1,1,-1],[1,-1,1,-1,1],[-1,1,-1,1,-1],[1,-1,1,-1,1]])

  p6=np.array([[1,-1,-1,-1,1],[-1,1,1,1,1],[1,-1,-1,-1,1],[1,1,1,1,-1],[1,-1,-1,-1,1]])```



