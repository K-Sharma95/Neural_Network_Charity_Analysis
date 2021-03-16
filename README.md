# Neural_Network_Charity_Analysis
## Overview
This repository contains data from over 34,000 organizations that have received funding from Alphabet Soup, with information describing the status and uses of this funding. This data is used to create a neural network model using Tensorflow and keras for the purpose of accurate classification. The performance of this model will be discussed and then optimized. 

## Results

### - **Data Processing**
What variable(s) are considered the target(s) for your model?
What variable(s) are considered to be the features for your model?
What variable(s) are neither targets nor features, and should be removed from the input data?



### - **Compiling, Training and Evaluating the Model**
As observed in [AlphabetSoupCharity.ipynb](https://github.com/K-Sharma95/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity.ipynb) the original characteristics of the model are two hidden layers, with 80 and 30 neurons respectively. The two layers are activated using the relu function, and the sigmoid function is used on the output layer. These inputs achieved an accuracy score of 72.64%, short of the goal of 75% accuracy. 
![](https://github.com/K-Sharma95/Neural_Network_Charity_Analysis/blob/main/Resources/accuracy_score_1.png)

### - **Optimization Techniques**
Three steps/techniques were implemented in order to optimize this model, located in [AlphabetSoupCharity_Optimization.ipynb](https://github.com/K-Sharma95/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity_Optimzation.ipynb). Firstly I added a third hidden layer, and added more neurons to each layer. Secondly, I changed the activation function of the outer layer from "sigmoid" to "tanh". And finally, I added 50 more epochs. Surprisingly, this resulted in a less accurate model suggesting the changed I made were not relevant for the data. I expected the "tanh" function was not the appropriate activation, so I ran the code without changing the activation function from "sigmoid", and still resulted in a less accurate model. Therefore I was not able to achieve the target performance. 



What variable(s) are considered the target(s) for your model?
What variable(s) are considered to be the features for your model?
What variable(s) are neither targets nor features, and should be removed from the input data?
Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take to try and increase model performance?

Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
