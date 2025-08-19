# Deep Learning (Artificial Neural Network): Churn Modelling
## Problem
A certain company wants to predict whether a certain employee will most likely to leave or stay in the company. Using the churn dataset, we will create an algorithm using Artificial Neural Network that can help the company on this issue.

## Project Objective
To create a Deep Learning algorithm (Artificial Neural Network) that gives us the probability whether the a staff in a company will stay or leave depending on some parameters.

## Data used
- <a href = "https://github.com/pagonzales/Artificial_Neural_Network_Project_Churn__Modelling/blob/main/Churn_Modelling_Dataset.csv">Dataset</a>

## Metrics
- Does the employee will most likely to leave or stay in the company?

## Action plan
- Preprocess the data
  - import the necessary dataset and select imporant columns using dataset.iloc command
  - Encode the categorical data
    - use LabelEncoder for the binary part (Male and Female)
    - use OneHotEncoder for encoding geography
  - Split the data into train and test set
  - Feature scale the data using StandardScaler
- Build the Artificial Neural Network (ANN) Algorithm
  - Model the data using the following parameters and hyperparameters
    - We use the "relu" activation function for the layers
    - And "sigmoid" activation function for the output
    - For the model fitting we use 100 epochs with 100 batch size.
- Compile the ANN
  - Use 'adam' as optimizer 'binary_crossentropy' as loss function and 'accuracy' as metrics
  - Train the model with batch size = 32 and epochs = 100
- Finally, Test the model using the test data
  - Create Confusion Matrix

## Project Insights
## Project Insights
- Using the parameters and hyperparameters mentioned above, we found out that:
  - The accuracy of the model using the train and validation dataset is 86.13%
- After running the test dataset we found that the model has an accuracy of 80.36%
## Final conclusion
- Using the parameters and hyperparameters above, we have a test model accuracy of 80.36%. Of course, this can still be improved by altering the parameters and choosing different activation functions and hidden layers. But this model we have presented here predicts that for 10 customers we can predict that 8 of them will buy again.
