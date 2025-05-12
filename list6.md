## List 6


### **Problem 6.1 (1 pt.)** 
  Consider California housing data
   - split data into train and test datasets using the scikit-learn split method
   - perform the analysis using neural network inplemented in [scikit-learn](https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPRegressor.html#sklearn.neural_network.MLPRegressor)
   - consider neural network with one hidden layer but with 5, 10 and 50 hidden units
   - check the accuracy of the networks predictions on training and test datasets
   - prepare the presentation about data, their properties, and results of the analysis

### **Problem 6.2 (1 pt.)**

  Repeat the problem 4.2 but use the neural network model from scikit-learn. Find the optimal number of neurons. How to choose the the optimal networks architecture?
  Play with activation functions, optimisation algorithm, batch size, learning rate etc.

### **Problem 6.3 (1 pt.)**

  Having a function f(x), compute its first, second, and third-order derivatives. Plot them in one picture. Let $x$ ranges from $[0,10]$. Compare obtained results with the true values.  Consider:
  * a) $f(x)=x^2\sin(x)+\sqrt{x}$

  * b) $f(x)=\frac{ln(x)}{x}+(\sqrt{x}+1)^2$

  * c) $f(x) = \sqrt{x} \exp(-x^2)$

*Note* Computations perform using Autograd PyTorch package.

### **Problem 6.4 (1 pt.)**
  Consider the `class RBF4(torch.nn.Module)`  from lecture 7. Correct this code and obtain the class of Gaussian RBF with fixed widths. Then, fit the data from the lecture and discuss several user-defined widths.

### **Problem 6.5 (1 pt.)**
  Consider the class `Network(nn.Module)` design to fit radial basis functions. Then, consider the three RBFs (Gaussian) with a number of centers 10, 40, and 200, respectively. Then, consider the boundary data, make the analysis, and plot all boundary areas in one figure (play with transparency and color).

### **Problem 6.6 (1 pt.)**
  Repeat the analysis of the Iris data with RGB (Gaussians) using the class `Network(nn.Module)` design to fit radial basis functions.

### **Problem 6.7 (1 pt.)**
  Write your own neural network class with four most popular activation functions, and user defined number of layers and units.
