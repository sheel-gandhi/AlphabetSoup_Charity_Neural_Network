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

2. **Were you able to achieve the target model performance?**
3. **What steps did you take to try and increase model performance?**
