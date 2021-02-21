# Neural_Network_Charity_Analysis


## Overview of the analysis:
This analysis utilizes a machine learning model to help predict the successfulness of funding for Alphabet Soup charity foundation. Filtering the information to get a good dataset to pull from, allowed the model to gather if successfull applications were possible if funding was approved. The ultimate goal was to get as close to a 75% sucess rate as it could through manipulating the parameters of modeling. 

### Results
#### Data Preprocessing
##### What variable(s) are considered the target(s) for your model?

The Is_Successful variable column filtered the data so that the machine could predict which applicant was successful or not.

##### What variable(s) are considered to be the features for your model?

The model features were Application_Type, Affiliation, Classification, Use_Case, Organization, Status, Income_Amount, Special_Considerations and Ask_Amount. Columns that contained large amounts of unique values would be bucketed into an Other category.

##### What variable(s) are neither targets nor features, and should be removed from the input data?

The variables removed from the dataset were the "EIN" and "NAME" columns since these were did not help with the model's predictions.

#### Compiling, Training, and Evaluating the Model

##### How many neurons, layers, and activation functions did you select for your neural network model, and why?

For the original test I performed, I chose to use 2 hidden layers containing 8 and 5 neurons and Rectified Linear Unit (Relu) as the activation function. The test ran for 100 epochs. 

##### Were you able to achieve the target model performance?

No. On the original attempt, I was only able to achieve 60% predictive accuracy while the target was 75%.

##### What steps did you take to try and increase model performance?

Since boosting the accuracy of the model is trial and error, I attempted 3 different methods of boosting the predictive accuracy.

On attempt 1, I used number of neurons in each layer from 8 and 5. I only acheived 60% accuracy. 

For attempt 2, I changed the neurons to 4 and 5. This resulted in 53% predictive accuracy.

For the 3rd attempt, the neurons in each layer were 9 and 2. After running my test, it scored 45% predictive accuracy.

### Summary

Overall, the deep learning model performed pretty well when predicting applicant successfullness if funded by Aplhabet Soup in spite of it not reaching 75%. If given more time, I would probably experiment with attempt 1 some more by dropping more feature columns from the dataset such as the Application Type and Classification columns and re-running the test. I do not think the deep learning model was the best choice. Another choice with more cleaning might be better in predicting this type of outcome.
