# credit-risk-classification20
Supervised Learning with Logistic Regression

 The project involves data preprocessing, model selection, and evaluation to identify creditworthiness of borrowers.
 
 The dataset contains information about loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt,and loan_status. The dataset is split into a training set and a testing set. 
 
 I used a logistic regression model as the baseline model and evaluate its performance using various metrics such as accuracy, precision, recall, and F1-score. 
 
 We separate the data into labels (y) and features (X) because this is a common data preparation step in machine learning. In a supervised learning task, we aim to train a model to predict the value of the target variable (in this case, "loan_status") based on the values of the input variables (in this case, all other columns except "loan_status").

To do this, we first need to split the data into two parts: the features, which are the input variables used to predict the target variable, and the labels, which are the target variable we are trying to predict.

By separating the data into labels and features, we can then use the features to train a machine learning model to predict the labels. The model can learn patterns and relationships in the features and their corresponding labels, and then use this knowledge to make predictions on new, unseen data.

Separating the data into labels and features is also useful for other data analysis tasks, such as exploratory data analysis and data visualization. It allows us to analyze and visualize the relationships between the input variables and the target variable separately, which can help us to better understand the data and identify potential patterns or trends.
 
 The logistic regression model uses a logistic function (also known as a sigmoid function) to transform the linear combination of the independent variables into a probability value between 0 and 1. This probability represents the likelihood that the input sample belongs to the positive class. The logistic function has an S-shaped curve that approaches 0 for very large negative values and approaches 1 for very large positive values, with a midpoint at 0.

The logistic regression model can be trained using a variety of optimization algorithms, such as gradient descent or Newton's method, to find the coefficients that minimize the difference between the predicted probabilities and the actual labels in the training data. Once the model is trained, it can be used to make predictions on new data by applying the logistic function to the linear combination of the independent variables and comparing the resulting probability to a decision threshold, usually set to 0.5.

Logistic regression is a widely used technique in many fields, such as medicine, economics, and social sciences, for tasks such as predicting the likelihood of a patient having a certain disease, classifying email messages as spam or not spam, or predicting the outcome of a political election.


