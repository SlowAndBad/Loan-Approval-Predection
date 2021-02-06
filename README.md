# Loan-Approval-Predection
I have worked on a Bank Data set to predict the the loan approval of applicants.  I have analysed and cleaned the data. I have removed the skewness and munged all the numerical fields of data using logarithmic conversion. I have tried to predict the loan approval status Logistic regression , decision tree classifier and random forest classifier. Almost all the models give nearly the same accuracy and k fold cross validation score. But random forest classifier would be the best model for this dataset with Accuracy : 83.388% and Cross-Validation Score : 80.786%. I have also analysed an interesting fact about this dataset, the Credit_History feature plays an vital role in loan approval. I trained a logistic regression model with only credit history as the feature and the model came up with an Accuracy : 80.945% and Cross-Validation Score : 80.937%. I later tried to analyse the feature importance of my features and got the following scores :-
Credit_History      0.288946
TotalIncome_log     0.248168
LoanAmount_log      0.218557
Dependents          0.053301
Property_Area       0.050651
Loan_Amount_Term    0.050354
Married             0.024307
Self_Employed       0.022627
Education           0.022573
Gender              0.020517
Based on this, my final feature vector for my model consisted only of credit history, log(totalIncome),log(LoanAmount), no: of dependents and property area in posession.
