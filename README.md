# Artifical-Neural-Network-Model for Diagnosis prediction
An artificial neural network (ANN) model built from scratch that trains multi-layer a perceptron network to predict cancer diagnoses from the Mix cancer dataset

## How to run
This project was created using Jupiter Notebook which is accessible through Anaconda Navigator, although this file can be run without Jupiter Notebook, in any IDE that supports Python e.g. VisualStudio Code. 

## How it works
This model of an Artificial Neural Network contains 3 layers: an input layer, a hidden layer and an outut layer. It is able to predict the classification of elements in a given dataset as either having or not having cancer based on 500 observations with 30 input variables and 1 output variable (Diagnosis).

Using a provided dataset called 'MixCancer.csv', the data from this is imported, split using sklearn's train_test_split library fucntion with a test size of 0.5.

Then the weights and biases of both layers are assigned random values. These will be updated later on as our model learns.

Note: The hidden layer of this model contains 5 perceptrons that use ReLu activation fucntion and the output layer contains only one perceptron that uses Sigmoid activation function.

The model is trained using the dataset during the 'feed forward' and 'backpropagation' sections and finally the new weights and biases are updated. This is repeated for x epochs (forward and backward passes of each perceptron) and repeated further by using mini-batch gradient descent which ultimately means that the weights and biases will be updated more times throughout the model.

Error/Loss and accuracy of the model is calculated and plotted for both the training and testing stages. The final error/loss and accuracy are printed at the very end. 

Note that the initial model is not fully optimised, and can only achieve about 76.0% accuracy and an error/loss of 0.178. The improved model has an accuracy of 97.6% and an error/loss of only 0.0205.



