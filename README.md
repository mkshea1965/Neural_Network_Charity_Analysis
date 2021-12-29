# Neural_Network_Charity_Analysis
## Overview of the Analysis
The purpose of this analysis was to create a binary classifier using machine learning and neural networks to predict whether or not applicants will be funded by a chaity, Alphabet Soup. Through this analysis, 34,000 sub-recipients of Alphabet Soup's previous funding were analyzed to predict either "yes" or "no" for future funding recipients.
## Results
### Data Preprocessing
What variable(s) are considered the target(s) for your model? "IS_SUCCESSFUL" column
What variable(s) are considered to be the features for your model? All other columns besides "IS_SUCCESSFUL" (APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special consideration for application
ASK_AMT—Funding amount requested).
What variable(s) are neither targets nor features, and should be removed from the input data? "EIN" and "NAME" since they have no effect on whether or not the recipient was successful in receiving funding - they are merely descriptors.
### Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why? Initiall, I used 2 layers, with 80 and 30 neurons each, respectively. FOr the first and second layer, ReLU was used, then Sigmoid was used for the output layer. I chose 80 neurons in the first hidden layer for faster processing time and 30 since it was less than half the first hidden layer and followed a pattern seen in the example codes of the module.
Were you able to achieve the target model performance? No.
What steps did you take to try and increase model performance? I tried optimizing the model by increasing the amount of individual neurons, increasing the amount of hidden layers, and changing the output activation function to "tanh".
## Summary
In summary, increasing the amount of individual neurons slightly decreased accuracy:
![Opt_Attempt1](https://user-images.githubusercontent.com/88520929/147705153-33b7446d-e991-4cee-b1a3-31bba2a0402f.PNG)
Increasing the amount of hidden layers s;ightly increased accuracy of the model:
![Opt_Attempt2](https://user-images.githubusercontent.com/88520929/147705168-6db4d5da-e6fe-46ed-bb81-24c1d31bcf27.PNG)
Changing the output activation function increased the accuracy of the model as well:
![Opt_Attempt3](https://user-images.githubusercontent.com/88520929/147705179-244b1309-98c1-4ab9-8646-ca670a3e30e7.PNG)
I would recommend increasing the amount of hidden layers, decreasing the amount of individual neurons, and changing the output activation function to tanh to increase performance. Further experimentation with these variables can hopefully get the data to above 75% accuracy
