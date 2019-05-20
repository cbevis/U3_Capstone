# NY State Controverted Workers' Compensation Claims

Data Sources: <br>
https://www.kaggle.com/new-york-state/nys-assembled-workers'-compensation-claims <br> https://data.ny.gov/Government-Finance/Assembled-Workers-Compensation-Claims-Beginning-20/jshw-gkgu

This projected used supervised learning to analyze New York State workers' compensation claims in order to predict whether or not the claim was controverted, or disputed by the insurance companies. Some of the things looked at include type of injury and when the injury occurred.  

Types of models:
I used random forest, gradient boosting, light gradient boosting, and logistic regression to model the data.  Light gradient boosting performed the best as measured by area under the curve.  The data set is unbalanced.  Far more claims are not controverted than are controverted.  As a result, I under sampled the majority class in the final model. 

Looking at the feature importances of the light gradient boosting model, the average weekly wage, the type of injury, and the part of the body injured were the most important features for predicting whether or not a case would be controverted.
