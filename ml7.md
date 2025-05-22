## List 7


### **Problem 7.1 (2 pt.)** 

- Consider the MNIST dataset.
- Design a neural network with no more than 6 fully connected layers, and no more than 20 units per layer.
- You may use dropout, batch normalization, and experiment with various weight initialization strategies.
- Train the most successful model you can under these constraints.
- Compute the model's accuracy on digit classification.
- Identify the misclassified samples.
- For 10 misclassified samples, examine the output probabilities predicted by the network. Plot a histogram of these probabilities for - - each of the 10 misclassified samples.

### **Problem 7.2 (2 pt.)** 

- Repeat Problem 7.1, but this time use the Fashion-MNIST dataset.
- Split the original training set into a new training and validation set using an 80:20 ratio.
- The best model is defined as the one achieving the lowest error on the validation set.
- You may use convolutional layers, pooling, and other advanced techniques.

### **Problem 7.3. (2 pt.)**

- Consider the Reuters dataset.
- https://keras.io/api/datasets/reuters/
- Consider the training dataset, split, as you wish, into the training and validation datasets
- Construct the fully connected layer, use all the structures that you have learned so far.
- Save the best model according to the validation data set.
