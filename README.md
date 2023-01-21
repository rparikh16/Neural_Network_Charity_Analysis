# Neural_Network_Charity_Analysis
## Overview of the Analysis
The goal of this analysis is to use deep machine learning models and neural networks on the different features of the provided Alphabet Soup's dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. 

## Results
Data Preprocessing
1. The target variable in my model is to see if the applicant is marked as successful in the DataFrame 
2. The IS_SUCCESSFUL column is the main feature in my model
3. The EIN, NAME, STATUS, and SPECIAL_CONSIDERATIONS variables will be removed from my model as they provide little information for the model

Compiling, Training, and Evaluating the Model
1. The optimized model has five hidden layers, layer 1 started with 110 neurons with a sigmoid activation, layer 2 has 80 neurons with a relu activation, layer 3 has 40 neurons with a relu activation, layer 4 has 20 neurons with a relu activation, layer 5 has 10 neurons with a relu activation. The output layer has 1 neuron, with a sigmoid activation. This model setup was chosen from trial and error making sure to not overfit the data while keeping accuracy high. 

<img width="858" alt="Screen Shot 2023-01-21 at 3 42 48 PM" src="https://user-images.githubusercontent.com/111692952/213886461-28e43567-fdd5-44cf-abdf-65e912548f5b.png">
<img width="800" alt="Screen Shot 2023-01-21 at 3 42 59 PM" src="https://user-images.githubusercontent.com/111692952/213886466-3df949f0-5678-4361-bcc2-d806f8c7adda.png">

2. The model was unable to achieve the target accuracy of 75%, the highest accuracy the model could achieve is 72.489798%
3. The steps taken were to remove columns that provided little input in model accuracy to increase the amount of hidden layers while using trial and error method to determine the best activation functions to use.


Trial # 2 - Overfit the data with too many hidden layers (relu activation):
<img width="849" alt="Screen Shot 2023-01-21 at 3 18 54 PM" src="https://user-images.githubusercontent.com/111692952/213886625-174aa694-5eac-4ee4-bdf8-572c12a0e953.png">
<img width="805" alt="Screen Shot 2023-01-21 at 3 19 03 PM" src="https://user-images.githubusercontent.com/111692952/213886627-f5a404d5-7945-4ce9-9bbf-b38d902a38ca.png">

Trial # 3 - Overfit the data with too many hidden layers (sigmoid activation): 
<img width="876" alt="Screen Shot 2023-01-21 at 3 18 15 PM" src="https://user-images.githubusercontent.com/111692952/213886643-e4b0b343-c273-4f58-be6c-9485e15dacac.png">
<img width="779" alt="Screen Shot 2023-01-21 at 3 18 25 PM" src="https://user-images.githubusercontent.com/111692952/213886645-68063479-ab01-4b8f-8a04-16b09141e7ca.png">


## Summary
This deep learning model was only able to get to an accuracy of 72.5% using a combination of relu and sigmoid activations. It is unlikely to get to the target accuracy of 75% using this type of deep-learning model. My recommendation would be to try the random forest classifier model as it is able to reduce outliers in the dataset and get a more accurate prediction.












