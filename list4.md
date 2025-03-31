## List 4

### **Problem 4.1 (1 pt.)**
Consider the [wine dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_wine.html#sklearn.datasets.load_wine):
- Split the data into training and test sets using scikit-learn’s split method.
- Analyze the data (for example, plot relationships between features using a 2D “triangle” plot).
- Create a 3D plot of the samples, distinguishing the three classes. Try various combinations of features.
- Use PCA, then plot the data in 3D again.
- Use the K-means algorithm for clustering the data.
- Check the accuracy of the model predictions on both the training and test sets.
- Prepare a presentation about the data, its properties, and the results of your analysis.

### **Problem 4.2 (1 pt.)**
Consider the [diabetes dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_diabetes.html#sklearn.datasets.load_diabetes):
- Split the data into training and test sets using scikit-learn’s split method.
- Analyze the data (for example, plot relationships between features using a 2D “triangle” plot).
- Perform a linear regression analysis.
- Check the accuracy of the model predictions on both the training and test sets.
- Prepare a presentation about the data, its properties, and the results of your analysis.

### **Problem 4.3 (1 pt.)**
Perform the same analysis as in **Problem 2.1**, but for the [digits dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_digits.html#sklearn.datasets.load_digits):
- Perform PCA, then do linear regression.

### **Problem 4.4 (1 pt.)**
Perform the same analysis as in **Problem 2.1**, but for the [breast cancer dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html#sklearn.datasets.load_breast_cancer).

### **Problem 4.5 (5 pt.)**
Consider the scattering [data](). The last column indicates the process type. Examine the dataset and determine if any types should be removed due to insufficient information. If necessary, perform data preprocessing. Then check the correlations.

Use PCA, K-means, or another clustering algorithm from scikit-learn to distinguish between the different process IDs. Finally, treat types 0 and 3 as the same and attempt to distinguish among the remaining types.  
