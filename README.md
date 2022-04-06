# Fashion Image Recognition with Convolutional Neural Network
## Overview
* Created a Convolutional Neural Network (CNN) to classify images from the Fashion MNIST dataset.
* Built a Random Forest Classifier model to compare the CNN results with.
* Optimized the Random Forest model with RandomizedSearchCV to reach the best model.

![](fashion_mnist.png)

<img src="https://github.com/andreasbergstrm/Fashion-Image-Recognition-with-CNN/blob/main/fashion_mnist.png" width="200" height="400" />

## Code and Resources Used

**Programming Language:** Python  
**Packages:** tensorflow, keras, matplotlib, scikit-learn  
**Dataset Source:** Fashion MNIST dataset imported from keras

## Model Building

When I imported the fashion_mnist data set I split the data directly into training and test splits. Then I reshaped the data to be appropriate for the CNN and normalized the data for more efficient training. Then I created the CNN with categorical_crossentropy as the loss function, the adam optimzier and accuracy as the evaluation metric. After fitting the data for 10 epochs I plotted the training history to show the train/test model accuracy and loss.  

![](CNN_history.png)

To compare the CNN results I also created a Random Forest classifier model. I used RandomizedSearchCV to tune the hyperparameters and reach the best model.

## Model Performance

The Convolutional Neural Net outperformed the Random Forest by about four percent accuracy. 
* **Convolutional Neural Network:** Accuracy = 91% 
* **Random Forest:** Accuracy = 87%
