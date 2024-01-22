# The report should contain the following:

# Overview of the analysis: Explain the purpose of this analysis.

# Results: Using bulleted lists and images to support your answers, address the following questions:

#Data Preprocessing

1. What variable(s) are the target(s) for your model?

The Target is the "Is-Successful" column

2. What variable(s) are the features for your model?

NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION,	USE_CASE,	ORGANIZATION,	STATUS,	INCOME_AMT,	SPECIAL_CONSIDERATIONS,	ASK_AMT.

3. What variable(s) should be removed from the input data because they are neither targets nor features?

EIN

#Compiling, Training, and Evaluating the Model

1. How many neurons, layers, and activation functions did you select for your neural network model, and why?


Employing three hidden layers with a multitude of neurons is motivated by the observed increase in accuracy beyond 75%, albeit at a significant computational cost. The initial activation function is relu, while subsequent layers utilize sigmoid, a choice anticipated to potentially enhance accuracy. Additionally, fine-tuning the data through techniques like one-hot encoding, specifically using 'get_dummies', may factor into achieving improved accuracy scores.

2. Were you able to achieve the target model performance?

Yes we were able to increase the accuracy.

3. What steps did you take in your attempts to increase model performance?

To enhance efficiency, it is necessary to convert the "NAME" attribute into data points with a significant impact. However, this process comes with a cost, as it involves adding a third layer with a sigmoid activation function. This strategic adjustment is expected to yield improvements in efficiency, albeit at an increased computational expense.

#Summary: Summarize the overall results of the deep learning model.

Overall, achieving an accuracy rate above 75% indicates successful classification in the test dataset 75% of the time. Specifically, an applicant stands an 80% chance of success if they adhere to the following criteria: the applicant's name appears more than 5 times, and the type of applications falls within the categories T3, T4, T5, T6, T7, T8, T10, and T19. These conditions contribute to a higher likelihood of successful classification based on the given format.

#Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.


Utilizing either a RandomForest model or a decision model is a viable approach to test accuracy. Employing multiple models enhances our understanding of how well each fits the data and whether there's a risk of overfitting. By exploring various models, we can identify the one that best suits our dataset, balancing the need for high accuracy without overfitting to ensure robust performance.
