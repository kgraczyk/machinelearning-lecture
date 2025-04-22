## List 5

### **Problem 5.1 (1 pt.)**
  Implement the K-Means algorithm but consider the distance defined by |x-y|^3.

### **Problem 5.2 (1 pt.)** 
  - Implement the Perceptron algorithm.
  - Using the sklearn package for generation data, obtain two classes of data that are linearly separable.
  - Apply the Perceptron algorithm, and make a simulation showing the iteration steps.

### **Problem 5.3 (1 pt.)**
  - Generate 20 pseudo-data points assuming that the true function reads $x/2 + 0.5 x^2 sin(6 x^2) $, and add the Gaussian noise (consider three scales of the noise).
  - Fit the polynomials of degrees 3, 10, and 20 using PolynomialFeatures from sklearn and numpy.polyfit 

### **Problem 5.4 (1 pt.)** 
  Consider California housing data
   - split data into train and test datasets using the scikit-learn split method
   - perform the analysis assuming that the input features are related via polynomial, use polynomial features, play with the highest degree of polynomial  
   - check the accuracy of the model predictions on training and test datasets
   - prepare the presentation about data (mardown), their properties, and results of the analysis

### **Problem 5.5 (1 pt.)**
  - Generate 100 pseudo-data points assuming that the true function reads $x/2 + 0.5 x^2 sin(6 x^2) $, and add the Gaussian noise (consider three scales of the noise).
  - Fit the polynomials of degrees 3, 10, and 20 using PolynomialFeatures from sklearn but apply Bayesian Ridge
  - Plot predictions with uncertainties
  - How do uncertainties depend on the degree of the polynomial? 

### **Problem 5.6 (1 pt.)**
  Repeat the analysis of 4.2 for $x^2/2 + 0.5 x^3 cos(6 x^2) $ for 20 data with x in [0, 3] and 20 data with x in [7,10] for the Gaussian noise with std 0.1, 1, and 10 respectively. 
  Compare the predictions.
  How does uncertainty depend on the noise?
  What about generalization? Play with regularization parameters.
