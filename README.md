# Neural_Network_Charity_Analysis
## Overview
This repository contains data from over 34,000 organizations that have received funding from Alphabet Soup, with information describing the status and uses of this funding. This data is used to create a neural network model using Tensorflow and keras for the purpose of accurate classification. The performance of this model will be discussed and then optimized. 

## Results

### - **Data Processing**
- What variable(s) are considered the target(s) for your model?
The target variable in this data-set is the "Is_Successful" column. 

- What variable(s) are considered to be the features for your model?
The featurs of the model include [these columns.](https://github.com/K-Sharma95/Neural_Network_Charity_Analysis/blob/main/Resources/features.png)
 
- What variable(s) are neither targets nor features, and should be removed from the input data?
The columns "EIN" and "NAME" are not necessary and were removed. 



### - **Compiling, Training and Evaluating the Model**
As observed in [AlphabetSoupCharity.ipynb](https://github.com/K-Sharma95/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity.ipynb) the original characteristics of the model are two hidden layers, with 80 and 30 neurons respectively. The two layers are activated using the relu function, and the sigmoid function is used on the output layer. These inputs achieved an accuracy score of 72.64%, short of the goal of 75% accuracy. 
![](https://github.com/K-Sharma95/Neural_Network_Charity_Analysis/blob/main/Resources/accuracy_score_1.png)

### - **Optimization Techniques**
Three steps/techniques were implemented in order to optimize this model, located in [AlphabetSoupCharity_Optimization.ipynb](https://github.com/K-Sharma95/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity_Optimzation.ipynb). Firstly I added a third hidden layer, and added more neurons to each layer. Secondly, I changed the activation function of the outer layer from "sigmoid" to "tanh". And finally, I added 50 more epochs. Surprisingly, this resulted in a less accurate model suggesting the changed I made were not relevant for the data. I expected the "tanh" function was not the appropriate activation, so I ran the code without changing the activation function from "sigmoid", and still resulted in a less accurate model. Therefore I was not able to achieve the target performance. 



### - Summary
Given the fact that I did not achieve my target accuracy, more consideration needs to be done for this model. The dataset provided is vast and I need to reconsider its characteristics, and the features being used. With a better understanding of my values I can accurately build my neuron layers to match and sleect the most appropriate activation function. I also believe that perhaps I should run the model using all of the features, and then test out removing some more data and see if that results in a more accurate model. 
