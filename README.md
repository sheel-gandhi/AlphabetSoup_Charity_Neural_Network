# AlphabetSoup_Charity_Neural_Network

Alphabet Soup Charity using Neural Network

## Purpose

Alphabet Soup Charity, a charity organization is about to analyse 34,000 fundings to predict whether it was successful or not. There are multiple features like - APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT on which success of funding is predicted. We shall be using Keras module from TensorFlow to run Neural Network

## Overview

* **Compare the differences between the traditional machine learning classification and regression models and the neural network models.**
* **Describe the perceptron model and its components.**
* **Implement neural network models using TensorFlow.**
* **Explain how different neural network structures change algorithm performance.**
* **Preprocess and construct datasets for neural network models.**
* **Compare the differences between neural network models and deep neural networks.**
* **Implement deep neural network models using TensorFlow.**
* **Save trained TensorFlow models for later use.**

## Results

1. **What variable(s) are considered the target(s) for your model?**
  Our analysis is to predict if a funding is successful. The taget variable in this model is IS_SUCCESSFUL.

2. **What variable(s) are considered to be the features for your model?**
  The variabless considered as features for our model are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT. Running Neural Network on these features will help in predicting our target variable
  
3. **What variable(s) are neither targets nor features, and should be removed from the input data?**
  Variables giving identification information will be included in neither targets nor features. Those variables are EIN and NAME  

### **Compiling, Training, and Evaluating the Model**

1. **How many neurons, layers, and activation functions did you select for your neural network model, and why?**  
  For initial analysis, we have taken 2 layers. The first layer will have 80 neurons with an activation function "relu". For second layer will have 30 neurons with "relu" activation function. The number of layers and neurons has been selected to optimize the model.

2. **Were you able to achieve the target model performance?**
  With the above selection of layers, neurons and activation functions, we were able to acheive the Accuracy: 0.724. The target performance of 0.75 is not achieved from this model   
  
3. **What steps did you take to try and increase model performance?**
  To acheive better results, we tried multiple options with different number of neurons and activation functions to see if we can improve the results from the model. 
  
  **Optimize trial 1** - We tried to drop some of the redundant variables like Status and Special_Consideration as looking at the variable counts, it showed data was skewed towards one value. We also merged Application column by replacing values lower thab 1000 under "Other". Three layers were added for this trial. First layer having 100 neurons witb "relu" activation function, Second layer having 40 neurons with sigmoid activation function and third layer having 15 neurons with sigmoid activation function. However with this model, we acheived accuracy of 0.710
  
  **Optimize trial 2** -  We tried to drop some of the redundant variables like Income_Amt as looking at the column, few funding values are just "0" it showed data was skewed towards one value. Three layers were added for this trial. First layer having 100 neurons witb "relu" activation function, Second layer having 40 neurons with relu activation function and third layer having 20 neurons with relu activation function. Total number of Epoch was changed to 40. However with this model, we acheived accuracy of 0.721
  
  **Optimize trial 3** -  We tried to drop some of the redundant variables like Income_Amt and ASK_AMT as looking at the column, few funding values in Income_Amt column are just "0" it showed skewed data and ASK_AMT column has huge number of unique values. Three layers were added for this trial. First layer having 100 neurons witb "relu" activation function, Second layer having 80 neurons with sigmoid activation function and third layer having 20 neurons with sigmoid activation function. Total number of Epoch was changed to 50. However with this model, we acheived accuracy of 0.720
  
## Summary
The models that we worked on with dropping columns, binning columns, different layers, neurons, activation funcitons and epochs we were able to acheive the accuracy of 0.724 but the target performance was still out of reach. We can work on running neural network model with few neurals in 2 layers both with relu activation function as the initial trial has the highest accuracy among all the trials run. 
