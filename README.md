# Neural_Network_Charity_Analysis
## Overview of the Analysis

The purpose of the analysis is to determine whether using Alphabet Soup will be effective for binary classifier. We are going to process uisng neural network/deep learning model to create this binary classification model. We will compile, train and evaluare the binary classification model to calculate the model's loss and accuracy.

## Results
1. What variable(s) are considered the target(s) for your model?
The target for our model is IS_SUCCESSFUL, this model determined whether the organization fund was used effectively or not.
2. What variable(s) are considered to be the features for your model? 
APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.
4. What variable(s) are neither targets nor features, and should be removed from the input data?
EIN and NAME were removed from the dataset

Compiling, Training, and Evaluating the Model

1. How many neurons, layers, and activation functions did you select for your neural network model, and why?
There are two hidden layers with 150 and 75 neurons. From this there was 71% accuracy
![image](https://user-images.githubusercontent.com/74630767/117555763-f7aa0b80-b02f-11eb-8605-ded8d06f6350.png)
Adding a third layer resulted in 70% accuracy, not effective in achieving the 75% target model
![image](https://user-images.githubusercontent.com/74630767/117555785-1ad4bb00-b030-11eb-9ad3-f354a97561ff.png)
Tanh was used in place of Relu and it also resulted in 70% accuracy
![image](https://user-images.githubusercontent.com/74630767/117555806-51aad100-b030-11eb-90f5-ab79176dad6e.png)

2. Were you able to achieve the target model performance?
Unfortunately, the closest we got to the 75% accuracy was 71% despite adding the hidden layers and using different activation function. The trials did not show a positive performance in predicting if the charity donations were successful or not.

3. What steps did you take to try and increase model performance?
Initially, the number of neurons were increased to try and increase model performance. A third hidden layer was also added to increase the performance of the neural network model. Both models failed to acheieve the target performance. Lastly, the activation function of the model was changed to try to increase model performance, but the change in function also failed to improve the performance rate.

## Summary
After trials and errors, the deep learning neural network model was unsuccessful in reaching the target model performance rate of 75%. In order to improve performance, I would recommend using the Random Forest Classifier. The Random Forest model combines multiple smaller models into a more accurate model. It would be faster to train due to this model being able to easily work with multiple features.
