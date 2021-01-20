# Neural Network Model Analysis

# Overview:

Bek’s is ready to put her skills of Neural Networks and deep learning models to work to help foundation predict where to make investments. With the knowledge of neural networks and machine learning, will be creating a binary classifier, that can predict whether applicants will be successful if funded by Alphabet Soup.  From Alphabet Soup’s business team, received a csv contain more than 34,000 organizations that have received funding from Alphabet Soup over the years. The csv contains columns EIN and NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, IS_SUCCESSFUL.


# Results:

## Data Processing

•	The target variable that used in AlphabetSoupCharity.ipynb and AlphabetSoupCharit_optimization.ipynb 1,2 and 3rd copy is “IS_SUCCESSFUL”.

•	The deliverable 2, used APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, IS_SUCCESSFUL as feature variables and drop EIN and NAME columns.

•	The deliverable 3, optimized copy 1 used APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, ASK_AMT, IS_SUCCESSFUL and dropped "EIN", "NAME", "SPECIAL_CONSIDERATIONS" columns. Also define Income_amt is greater than 0 and drop all the empty values.

•	In deliverable 3 optimized copy 2 drop "EIN", "NAME", "SPECIAL_CONSIDERATIONS", "CLASSIFICATION", also drop the null values in the application Data Frame.

•	In deliverable 3 optimized copy 3, dropped "EIN", "NAME","AFFILIATION", "USE_CASE", "SPECIAL" and null values.

## Compiling, Training and Evaluating the model

•	In deliverable 2, had two hidden layers: layer 1 had 80 neurons, layer 2 had 30 neurons, “relu” was used as activation function and for output layer used “sigmoid” as activation function. Relu activation function was used because it simplifies the positive nonlinear input data for classification. 

•	In deliverable 3 optimized copy 1, had two hidden layers with 300 and 100 neurons, “relu” as input and “sigmoid” as output activation function. Relu is ideal for positive nonlinear input data for classification and Sigmoid function is ideal for binary classification. Unfortunately, model did not perform up to 75%. Revised the columns need to remove, defined Income_amt is greater than 0, increasing neurons amount in hidden layers.

•	Deliverable 3 optimized copy 2, used 3 hidden layers with 200, 100 and 50 neurons. For first 2 layers used “relu” as input activation function and “tanh” was for third layer. Relu is ideal for positive nonlinear classification, Tanh function can expand the range between -1 to 1 for classification or regressions. Output activation function was “sigmoid”. Unfortunately, our model was not successful, there was more data loss than accuracy. Increase more layers and neurons and multiple activation functions did not made model work up to 75%.

•	Deliverable 3 optimized copy 3, chose to use 5 hidden layers, 1000,800,600,400,200 neurons. Tanh as input activation function and sigmoid as output. Tanh can classify the input data between range of -1 to 1. Unfortunately, our model accuracy did not go up to 75% or higher. Loss 0.72% was higher than accuracy 0.46%. Adding more layers, increased neurons and different activation function did not help the model to thrive.

## Summary:

- The overall model performance was poor, considering all the effort to optimize the model, provided the resources to setup the model.  The classification between data was tricky but features to the model were at question with regards to how well it might corelate with outcome from whoever had received funding through Alphabet Soup.

- Decision trees might improve the quality of classification problem in neural network. Decision trees work through if-else conditions to visualize the data and classify according to the conditions. For any classification model to succeed, the input should be suitable for feature regards to corelated with the successful outcomes.

 
