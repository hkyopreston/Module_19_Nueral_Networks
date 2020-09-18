# Module_19_Challenge: Alphabet Soup
----------------------------------------------------------------

## Project Overview
-----------------------------------------------------------------
In this project, I built my own machine learning model that will predict the success of a venture paid by Alphabet Soup. The model will be used to determind if ventures will be succesful in receiving future funding from Alphabet Soup. 

The main portions of this project were to: 
  - Import, analyze, clean, and preprocess a "real-world" classification dataset
  - Select, design, and train a binary classification model of your choosing
  - Optimize model training and input data to achieve desired model performance
  - Achieve 75% or higher accuracy
-----------------------------------------------------------------

1. How many Neurons and layers did you select for your neural network model?
  - In my original neural network and all optimization models, I added teh number of input features equal to the number of variables in the feature DataFrame. In the original neural network, I created two hidden layers. The first with 8 neurons and the second layer with 5 neurons. Each input layer used the ReLu activation function and the output layer used the sigmoid activation function. The sigmoid function is helpful to predict whether or not an applicant will be successful if funded by Alphabet Soup. 

2. Were you able to achieve target model performance?
  - I was unable to achieve the target model performance of 75%. Each neural network I created was about to correctly identify applicants who will be successful approximately 72.5% of the time. My original model (before optimization attempts) could predict accuracy at 72.57%

3. What steps did you take to try and increase model performance?
  - I took three steps to increase model performance. 
  - The first step was to add neurons to my hidden layers. I increased the first hidden layer to 12 neurons and increased the second hidden layer to 6 neurons. This produced a model that could predict accuracy at 72.93%
  - The second step I took was to add a third hidden layer. I kept the first two hidden layer neurons at 12 and 6, then added a third hidden layer with 3 neurons. This decreased neurons in each hidden layer by half. This model could predict accuracy at 72.64%
  - The third optimization step I took was to change the activation function in hidden layers. I reverted back to two hidden layers with 8 and 5 neurons respectively. I also changed the input layers to sigmoid activation. This produced an accuracy of 72.58%. 
  
 Overall, all three models were very close in accuracy. The model with 3 hidden layers was marginally beter at 72.64%. 

4. If you were to implement a different model to solve this classification problem, which would you choose and why?

  - I would us a Random forest classifier. Random forest classifiers are a type of ensemble learning model that combines multiple smaller models into a more robust and accurate model. They use a number of weak learner algorithms and combine their output to make a final classification decision. Random forest models have been popular in machine learning algorithms for many years due to their robustness and scalability. Both output and feature selection of random forest models are easy to interpret, and they can easily handle outliers and nonlinear data.
