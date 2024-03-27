# Deep Learning in Five Steps


## Problems

- Problems were originally wrapped into the lecture notes. So they have a corresponding context.
During the labs, there were organized competitions, like Kaggle, where the best people were awarded extra points. The students had about 20 to 45 minutes to accomplish the task. Then, the solutions were shown and discussed on the whiteboard.
The final grade was based on the final theoretical test and achievements during the labs. In practice, the final grade was a combination of test grades and lab achievements.

### Lecture 1

* __Problem 1 (10 pt.)__

  Adapt above code and plot isolines of the loss as a function of two parameters $b_0$ and $b_1$. In the same figure show the trajectory of the training.

* __Problem 2 (10 pt.)__
  Adapt above code and plot 2d density plot of the loss as a function of two parameters $b_0$ and $b_1$. In the same figure show the trajectory of the training.

* __Problem 3 (10 pt.)__
Adapt above code and consider several values of the learning rate and various starting points. Show the trajectories of training in the parameter space.

* __Problem 4 (5 pt.)__
In one figure plot true vs. predictions and histogram of $r_i$'s

* __Problem 5 (5)__
Compare the model with and without regularization. Strat from the same initial parameters, compare losses and predictions.

* __Problem 6 (15)__
Generate the true data from the function:
$$
y = (\sin(x^1 x^2) +x^1), \quad x^1,x^2 \in [-1,1]
$$  
  * Using the Keras fit the data with 2-layers, 3-layers and 5-layers linear model.
  * Compare the loss functions. Plot predictions vs True. Compare model predictions.

### Lecture 2

* __Problem 7 (10)__

Reconstruct the Figs. 3 and 4 of `https://arxiv.org/abs/2005.00817`

* __Problem 8 (10)__

Consider the true function from __Problem 6__, and generate the data. Then fit the data using a two-hidden layer network with sigmoid activation functions in the hidden layer.

* __Problem 9 (15)__

  * Generate the true data from the function (with Gaussian noise, variance=0.3):
  $y=(\sin(x1x2)+x1),x1,x2∈[−1,1] $
  * Using the Keras fit the data with 3-layers model. Check four different choices for activation functions.
  * Compare the loss functions.
  * Plot predictions vs True.
  * Compare model predictions.

* __Problem 10 (10)__

  * For which type of feature the best predictions have been obtained?
  * Choose the worst five features and train the model only for them.
  * Train separate model for rest of features.
  * Chech the performance of the two models on the test dataset and compare them with the vanilla model.

* __Problem 11 (10)__

  * Train the model with MAE loss.
  * Compare the obtained model with the vanila one, namely compare the predictions for test dataset, and MAE values for test dataset.
 
<font color = 'red'>**COMPETITION** </font>

<font color = 'red'> During classes, tray to learn the model so that you get the lowest in the group loss for test dataset.
  * The winner takes 25 points
  * The second place 15 points
  * The third place  10 points
</font>

Tips: play with activation functions, initializations, regularizations, batch size, optimization algorithms etc.

### Lecture 3

* __Problem 12 (10)__

  * Find how many times the network overshots in MNIST problem.

  * Print six the most spectacular examples.


* __Problem 13 (15) + Competetion 1__

* Consider fashion mnist data (https://keras.io/api/datasets/fashion_mnist).

* Performe the analysis, using dense neural network.

  * Split the training data set into training and validation, in propotions 80 to 20
  * Plot the training losses and metrics
  * Plot the six best (pictures of obejcts) predictions and six worst predictions (pictures of obejcts with labels and net predictions)
  * Compute the score for the test dataset. The best three persons get extra points for the best results.

* __Probelm 14 (8)__
  * From the previous problem, make four figures (choose the worst four cases for network predictions). Each figure should contain the input picture with network prediction and plots of probabilities predicted for each possible class.  

* **Competition 2**

  * Consider the Reuters dataset.

  * https://keras.io/api/datasets/reuters/

  * Consider the training dataset, split, as you wish, into the training and validation datasets
  * Construct the fully connected layer, use all the structures that you have learned so far.
  * Save the best model according to the validation data set.

  * Only the best model you saved use to compute the score for the test data set.

    * **1st place: 30**
    * **2nd place: 25**
    * **3nd place: 20**
    * **4th place: 15**
   
*  **Problem 15 (25)**

  The dataset with cats and dogs contains unlaballed samples.
  * Choose four of them randomly (write a script that does it)
  * Take the models DC and DC and make predictions for the four chosen pictures.
  * Plot four figures with both model predictions.

### Lectures 4-5

* **Competition 3**
  Consider dogs vs cats data, as they are given at the lecture. Design the network which can have no more than 4 convolutional layers. Train the model. The model with the highest accuracy on test data set wins.

   * **1st place: 30**
   * **2nd place: 25**
   * **3nd place: 20**
   * **4th place: 15**
   * **5th place: 10**
   * **6nd place:  5**




* **Competition 4**
  Write the procedure that randomly takes 20 figures from an unlabelled set of pictures (see problem above). Print them together with a prediction of your network. Count the number of successful predictions.

   * **1st place: 30**
   * **2nd place: 25**
   * **3nd place: 20**
   * **4th place: 15**
   * **5th place: 10**
   * **6nd place:  5**
