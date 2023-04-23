# Predicting Cross Sell Promotion Success for Apprentice Chef Inc.

## Project Description

Modeling Criteria and Violation Penalties-

<b>Criterion 1 - Train-Test Gap</b><br>
In the previous assignment, you were expected to keep your final model's train-test gap below 0.05. In this assignment, you are expected to minimize it as much as is feasible.

Gap Penalty
Your final model points will be reduced by the absolute value of the train-test gap.

<b>Criterion 2 – Response Variable Usage</b><br>
The response variable cannot be used in any form as an explanatory variable (the y-variable cannot be used on the X-side). This includes logarithmic versions of the y-variable, and features that were engineered using the y-variable.

Violation Penalty
The following will occur if the response variable was used as an explanatory variable:
The model will be rescored after such variables has been removed. This will likely result in a major reduction in your final score, so be careful!
The best model in your final model table that does not include the y-variable on the X-side will be assessed.
Your grade for this deliverable will be reduced by one letter grade (-10 points).

<b>Criterion 3 – Model Types</b><br>
Model types are appropriate for the task at hand and come from scikit-learn (other packages and/or engines are not permitted). However, you may use statsmodels to evaluate your model statistics, as long as your final model is in scikit-learn.

Permitted Model Types
You may only use the model types presented in class and must use them from statsmodels or sklearn. Note that you are permitted to adjust the optional arguments of the permitted model types. Below is a list of permitted model types linked to their respective scikit-learn documentation.

Logistic Regression
Decision Tree Classifier
Random Forest Classifier
Gradient Boosting Classifier
KNeighbors Classifier

Violation Penalty
Final models that are not in the list of permitted model types will be discarded and the last appropriate model that ran in your code will be used as your final model. Final model points will be reduced by 0.025.

<b>Criterion 4 – Errors, Code Comments and  Markdown</b><br>
For this assignment, aim for a minimum one quality comment for every 5 lines of code.
Make sure to include the following in your markdown:
A markdown version of your confusion matrix that shows what happened in each box. There is an example in Script 7 for the Titanic dataset ("We predicted someone would get in a lifeboat, but they didn't", etc.).
An interpretation of each error from the confusion matrix. For example, if we predicted someone would not subscribe to the wine promotion and they did, what is the drawback/risk for the company? Also, which error should the company be more interested in minimizing?

Violation Penalty
Not being well-commented will reduce your final model points by 0.025.
Not being within the markdown limit will reduce your final model points by 0.025.
Submitting a code with at least one error will reduce your final model points by 0.025.
 
<b>Criterion 5 – Code Processing Time</b><br>
Your code must process from beginning to end in 240 seconds or less, based on your computer’s processing speed. Watch out for your hyperparameter tuning!

Violation Penalty
Not meeting this criteria will reduce your final model points by 0.025.

<b>Criterion 6 – Model Output</b><br>
Model results are outputted as a dynamic string (i.e., f-string) at the end of your script. This must be the very last thing that your Jupyter Notebook outputs. DO NOT write this in a markdown cell or export as an Excel file. This must be a dynamic string.

Output table of candidate models is well-formatted and contains the following information:
- Model Type
- Training Accuracy
- Testing Accuracy
- Train-Test Gap
- AUC Score
- Confusion Matrix
- It is clear which model is your final model (label it accordingly). The final model MUST be labeled in your dynamic string to meet this criterion.

Violation Penalty
Not including all of the above information in a well-formatted dynamic string will result in a 0.025 reduction in model points.
If it is unclear which model was selected as the final model, the following will occur, the last model in the dynamic string will be utilized as your final model.

<b>Criterion 7 – X-Variable Usage</b><br>
The original and logarithmic versions of an x-variable may not be used in the same model. You must choose one or the other. This does not include engineered features based on these variables.
No exponential or polynomial versions of the x-variables are allowed. In other words you are not allowed to square any of the x-variables in feature engineering (use any other exponents on them).
The removal of at least one category when using categorical variables.

Violation Penalty
If either of the above are violated, all but the original version of the x-variable will be removed from your model and it will be rerun again. Your final model points will also be reduced by 0.025.

<b>Criterion 8 - Full Dataset Usage</b><br>
You are not permitted to remove or modify any observations from the original dataset, with the exception of imputing missing values (you are not permitted to remove observations with missing values). Also, your Jupyter Notebook must be able to be run from the original dataset (no feature engineering or alterations in Excel or other tools are permitted).

Violation Penalty
If the above is violated, your Jupyter Notebook will be rerun from the original dataset and any errors that result from this will be subject to Criterion 4 above.
Your final model points will be reduced by 0.025.

<b>Criterion 9 – Model Parameter Requirements</b><br>
The following criteria must be met when developing your models:
- random_state is set to 219
- test_size is set to 0.25
- target variable is stratified
- max_depth for classification tree, random forest, and gradient boosted machine (GBM) models is less than or equal to 8

Violation Penalty
Not following the model parameter requirements will result in a one grade band reduction, and the random_state, test_size, and stratify arguments will be set appropriately before rerunning your model. Also, your model will be rerun with a max_depth of 8.

## Project Outcome

Developed a predicitve model using Gradient Boosting Classifier with roc_auc of 0.63
