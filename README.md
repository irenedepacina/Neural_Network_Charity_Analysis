# Neural_Network_Charity_Analysis

## Overview of the analysis

The purpose of this analysis was to use machine learning and neural networks to create a binary classifer that is capable of predicting whether applicants, from a pool of more than 34,000 organzations, will be successful if funded by investor, Alphabet Soup. The dataset was cleaned, compiled, trained, and evaluate into a model. The model was optimized to the highest possible accuracy.

## Results

Data Preprocessing
- What variable(s) are considered the target(s) for your model?
    - IS_SUCCESSFUL column
- What variable(s) are considered to be the features for your model?
    - All of the columns with the exception of IS_SUCCESSFUL column and the columns there were dropped.
    - APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, STATUS
- What variable(s) are neither targets nor features, and should be removed from the input data?
    - EIN, NAME

Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
    - For my neural network, I used 2 layers, 250 and 100 neurons respecively, and both "relu" activation functions.  
- Were you able to achieve the target model performance?
    - Unfortunately, I was unable to achieve the targer model performance of 75%. Instead, I was able to achieve 72.64%.
- What steps did you take to try and increase model performance?
    - Removed an additional feature; however the accuracy dropped
    - Add more neurons to the hidden layer; the accuracy dropped to 72.61%
    - Add additional hidden layers; however the accuracy dropped to 72.61% - sometimes lower when the code ran again

## Summary
The overall results of the deep learning model is that the model ended up with a slightly increased accuracy after the optimization. The initial neural network had an accuracy of 72.40% and increased to 72.64% at best. The minial increase could be due to the fact that the model is overfitted. Regardless of the additional layers and neurons, the optimization of the model can only extend so far. A recommendation for how a different model could solve this classification problem, is by using Random Forest classifers as they perform faster and more efficient. This recommendation could have prevented any overfitting. 