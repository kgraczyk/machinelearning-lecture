## List 1 (5 pt.)

### __Problem 1.1__ (1pt.)
Let a Hopfield network have N nodes. How many weights does a network with symmetric connections have, and how many weights does a network with bidirectional connections have? Answer and justify with a calculation.  

### __Problem 1.2__ (1pt.)
According to Hebb's rule, the weights of the connections in a Hopfield network are updated according to the formula:\
$$w_{ij} = \frac{1}{N}\sum_{\mu=1}^p \xi^\mu_i \xi^\mu_j.$$
     
We can slightly generalize the above rule and assume that\
$$w_{ij} = \eta \sum_{\mu=1}^p \xi^\mu_i \xi^\mu_j, \quad \eta >0
$$\
Does the magnitude of  $\eta$ matter? Why was  $\eta=1/N$ chosen? Provide a short explanation with a calculation.

### __Problem 1.3__ (1pt.)
Show that if a Hopfield network does not have symmetric connections, then the learning update process may not lead to convergent states. Solve the problem by constructing a two-node neural network.

### __Problem 1.3__ (1pt.)
Show that if a Hopfield network is trained synchronously, it may not lead to convergent states. Solve the problem by constructing a two-node neural network.

### __Problem 1.4__ (1pt.)
Show that if the initial pattern $S_i$ has at most half of its bits differing from the pattern $\xi_j$, Hebb's rule will still lead the state $S_i$ to the pattern $xi_j$.

### __Problem 1.5__ (1pt.)
Calculate the first and second moments for the binomial distribution and the variance.
