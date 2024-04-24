# Machine Learning Lecture


## List 1

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


## List 2

* __Problem 2.1 (20 pt.)__
 Consider wine data [here](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_wine.html#sklearn.datasets.load_wine)
   - split data into train and test datasets using scikit-learn split method
   - analyze data (plot relations between features 2D triangle plot)
   - plot3D of the samples, distinguish between three classes, consider various combinations of features
   - use PCA and then plot3D once again
   - use the K-means algorithm for clustering the data
   - check the accuracy of the model predictions on training and test datasets
   - prepare the presentation about data, their properties, and the results of the analysis

 * __Problem 2.2 (20 pt.)__
 Consider diabetes data [here](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_diabetes.html#sklearn.datasets.load_diabetes)
   - split data into train and test datasets using scikit-learn split method
   - analyze data (plot relations between features 2D triangle plot)
   - perform linear regression analysis
   - check the accuracy of the model predictions on training and test datasets
   - prepare the presentation about data, their properties, and results of the analysis

* __Problem 2.3 (20 pt.)__
Make the dame analysis as in Problem 2.1 but for digits data [here](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_digits.html#sklearn.datasets.load_digits)
   - make PCA, and then linear regression

* __Problem 2.4 (20 pt.)__
Make the dame analysis as in Problem 2.1 but for breast cancer [here](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html#sklearn.datasets.load_breast_cancer)


## List 3

* __Problem 3.1 (30 pt.)__ 
  Implement the K-Means algorithm but consider the distance defined by |x-y|^3.

* __Problem 3.2 (35 pt.)__ 
  - Implement the Perceptron algorithm.
  - Using the sklearn package for generation data, obtain two classes of data that are linearly separable.
  - Apply the Perceptron algorithm, and make a simulation showing the iteration steps.

* __Problem 3.3 (15 pt)__
  - Generate 20 pseudo-data points assuming that the true function reads $x/2 + 0.5 x^2 sin(6 x^2) $, and add the Gaussian noise (consider three scales of the noise).
  - Fit the polynomials of degrees 3, 10, and 20 using PolynomialFeatures from sklearn and numpy.polyfit 

## List 4

* __Problem 4.1 (20 pt.)__ 
  Consider California housing data
   - split data into train and test datasets using the scikit-learn split method
   - perform the analysis assuming that the input features are related via polynomial, use polynomial features, play with the highest degree of polynomial  
   - check the accuracy of the model predictions on training and test datasets
   - prepare the presentation about data, their properties, and results of the analysis

* __Problem 4.2 (15 pt)__
  - Generate 100 pseudo-data points assuming that the true function reads $x/2 + 0.5 x^2 sin(6 x^2) $, and add the Gaussian noise (consider three scales of the noise).
  - Fit the polynomials of degrees 3, 10, and 20 using PolynomialFeatures from sklearn but apply Bayesian Ridge
  - Plot predictions with uncertainties
  - How do uncertainties depend on the degree of the polynomial? 

* __Problem 4.3 (25 pt)__
  Repeat the analysis of 4.2 for $x^2/2 + 0.5 x^3 cos(6 x^2) $ for 20 data with x in [0, 3] and 20 data with x in [7,10] for the Gaussian noise with std 0.1, 1, and 10 respectively. 
  Compare the predictions.
  How does uncertainty depend on the noise?
  What about generalization? Play with regularization parameters.
  

## List 5

* __Problem 5.1 (20 pt.)__ 
  Consider California housing data
   - split data into train and test datasets using the scikit-learn split method
   - perform the analysis using neural network inplemented in [scikit-learn](https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPRegressor.html#sklearn.neural_network.MLPRegressor)
   - consider neural network with one hidden layer but with 5, 10 and 50 hidden units
   - check the accuracy of the networks predictions on training and test datasets
   - prepare the presentation about data, their properties, and results of the analysis

* __Problem 5.2 (20 pt.)__

  Repeat the problem 4.2 but use the neural network model from scikit-learn. Find the optimal number of neurons. How to choose the the optimal networks architecture?
  Play with activation functions, optimisation algorithm, batch size, learning rate etc.

* __Problem 5.3 (20 pt.)__

  Having a function f(x), compute its first, second, and third-order derivatives. Plot them in one picture. Let $x$ ranges from $[0,10]$. Compare obtained results with the true values.  Consider:
  * a) $f(x)=x^2\sin(x)+\sqrt{x}$

  * b) $f(x)=\frac{ln(x)}{x}+(\sqrt{x}+1)^2$

  * c) $f(x) = \sqrt{x} \exp(-x^2)$

*Note* Computations perform using Autograd PyTorch package.

## List 6

* __Problem 6.1 (15 pt.)__
  Consider the `class RBF4(torch.nn.Module)`  from lecture 7. Correct this code and obtain the class of Gaussian RBF with fixed widths. Then, fit the data from the lecture and discuss several user-defined widths.

* __Problem 6.2 (20 pt.)__
  Consider the class `Network(nn.Module)` design to fit radial basis functions. Then, consider the three RBFs (Gaussian) with a number of centers 10, 40, and 200, respectively. Then, consider the boundary data, make the analysis, and plot all boundary areas in one figure (play with transparency and color).

* __Problem 6.3 (20 pt.)__
  Repeat the analysis of the Iris data with RGB (Gaussians) using the class `Network(nn.Module)` design to fit radial basis functions.

* __Problem 6.4 (40 pt.)__
  Write your own neural network class with four most popular activation functions, and user defined number of layers and units.

## List 7.

* __Problem 7.1 (30 pt)__
  Read the review [arxiv:1609.04747](https://arxiv.org/abs/1609.04747). Then choose one of the algorithms from section 4 and implement. It should optimize of the function of the form `loss(*params)`.
* __Problem 7.2 (5 pt)__
  Read the paper [arxiv:2005.00817](https://arxiv.org/abs/2005.00817), and reproduce the figures 3 and 4.


  
