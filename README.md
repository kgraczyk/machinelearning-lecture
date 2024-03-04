# Machine Learning Lecture


## Lista 1

* **Problem 0.1**
  - Generate the tensor t of dimension $100$ filled by random numbers from the range [-1,1].
  - Using the the tensor from the above obtain the tensor of the form [[number],[number],[number],...], so of the shape (100,1)
  - from tensor t obtain the tensor of the shape (25,4) and (4,25)


* __Problem 1.1 (10 pt.)__
  Consider `fitter(x_train,y_train)` (Lecture 2, Sec. 2.1.1) and data below and plot isolines of the loss as a function of two parameters $b_0$ and $b_1$. In the same figure show the trajectory of the training.

  ``` Python

  # true values of the parameters of the linear model
  b0true=0.7
  b1true=2.3
  # width of the normal distribution of noise
  sigma=0.15
  # total number of points
  Ntot =120

  # Data Generation
  x = np.random.rand(Ntot, 1)
  y = b0true + b1true * x + sigma * np.random.randn(Ntot, 1)

  # Shuffles the indices
  idx = np.arange(Ntot)
  np.random.shuffle(idx)

  # Uses first 80 random indices for train
  train_idx = idx[:80]
  # Uses the remaining indices for validation
  val_idx = idx[80:]

  # Generates train and validation sets
  x_train, y_train = x[train_idx], y[train_idx]
  x_val, y_val = x[val_idx], y[val_idx]

  ```

* __Problem 1.2 (10 pt.)__
  Adapt code from previous problem and plot 2d density plot of the loss as a function of two parameters $b_0$ and $b_1$. In the same figure show the trajectory of the training.

* __Problem 1.3 (10 pt.)__
Adapt training code and consider several values of the learning rate and various starting points. Show the trajectories of training in the parameter space.

* __Problem 1.4 (5 pt.)__
In one figure plot true vs. predictions and histogram of r_i's

* __Problem 1.5 (10 pt.)__ Consider Boston housing data. Choose one of the linear models in scikit-learn and make analysis. Compare the resutls with the linear model discussed during the lecture.
