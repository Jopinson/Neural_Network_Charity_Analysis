# Neural_Network_Charity_Analysis Overview
I was tasked by Beks and her company Alphabet Soup, an investment firm, to create a machine learning and neural network program that uses the features in a dataset containing more than 34,000 organizations that have received funding from Alphabet Soup over the years to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Data Preprocessing
- In testing we considered IS_SUCCESSFUL as the target varible. 
- The varibles that we considered features were APPLICATION_TYPE, AFFILITATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, ASK_AMOUNT, and STATUS
- We found the varibles EIN, NAME, and SPECIAL_CONSIDERATIONS to not be helpful and removed them from the test. 

## Compiling, Training, and Evaluating the Model
-Our intial test featured two hidden layers of 80 and 30 neurons. The hidden layers used the relu activation and our outer layer used sigmoid. The ReLU function is ideal for looking at positive nonlinear input data for classification or regression and sigmoiod is perfect for binary classification
- We were not able to achieve our target goal of 75%, our best score was 74%
-In order to try and optimze our neural network, we removed the SPECIAL_CONSIDERATIONS varible, which did not help very much. Then we added a new hidden layer and increased the number of neurons to 120,100, and 80, as well as increasing the number of epochs to 200 and our score only went up slightly, still rounded to 73%. Lastly I changed the activation functions to tanh and that also dropped my score. 

# Summary
Ultimately our model did not hit the target goal of 75%, but I do believe it is possible to achieve that score. There are a varity of ways we could increase optimation, including adding more neurons, taking away neurons, changing the activation functions, or more hidden layers. With more hidden layers we may be able to use more neurons to increase our score. 
