# Term Deposit Marketing.

Given data to  develop a machine learning system that leverages information coming from call center data to improve the success rate for calls made to customers for any product clients offer. Design a machine learning product that offers high success outcomes while offering interpretability for  clients to make informed decisions.The calls are to ensure customers subscribe to term deposit.

#Data Description
The data is from   marketing efforts of a European banking institution which contains the following features:
age |job | marital
education | default-credit in default? 
balance, in euros | housing-housing loan?
loan-personal loan? | contact
day: last contact |month: last contact
duration: last contact  in seconds |campaign: number of contacts performed 

Output (desired target):
y - has the client subscribed to a term deposit? (binary)

#Approach
Due to the  imbalance in data with a 93% majority  and 7% minority I performed an upsampling to the minority class and added class weights. I trained several modls including XGBoost Classifier,Random Forest,Decision tree,Logistic regression,Perceptron,Linear SVC and Stochastic Gradient Classifier.
XGBoost gave the best values of F1 score  56% on minority class followed by Random Forest Classifier with f1 score of 46%.

I perfored a Hyperparameter tuning on the two models and Random Forest improved giving the best  f1 score value of 58%.And an overall accuracy of 93%.
Probability prediction on classes shows that at probability threshhold of 0.4 the model gave the best values of f1 scores.


