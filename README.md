# Lead_Score_Case_Study
## Objective
An education company named X Education sells online courses to industry professionals. The
company markets its courses on several websites and search engines like Google. Once these
people land on the website, they might browse the courses or fill up a form for the course or
watch some videos. When these people fill up a form providing their email address or phone
number, they are classified to be a lead. Now, although X Education gets a lot of leads, its lead
conversion rate is very poor. For example, if, say, they acquire 100 leads in a day, only about 30
of them are converted. To make this process more efficient, the company wishes to identify the
most potential leads, also known as ‘Hot Leads’.

## Steps Followed
1) Data loading and preparation: We loaded the data into a Jupyter notebook and
   performed missing value and outlier treatment for all columns. We also dropped
   columns that had more than 45% missing values.

2) Exploratory Data Analysis (EDA): We conducted EDA on each categorical column to
   visualize data imbalance and dropped high data imbalanced columns.

3) Train-test split and feature scaling: We performed train-test split using the sklearn
   library and scaled the train data using Standard Scaler.

4) Feature selection: We used Recursive Feature Elimination (RFE) to select 20 features
   for the model.

5) Logistic Regression: We used the statsmodels GLM method to perform Logistic
   Regression on the selected features and checked coefficients, p-values, and Variance
   Inflation Factor (VIF).

6) Model evaluation: We evaluated the model using accuracy, specificity, and sensitivity.
   We also plotted the Receiver Operating Characteristic (ROC) curve to check the
   balance between True Positive Rate (TPR) and False Positive Rate (FPR).

7) Cut-off selection: We selected the optimal cut-off point (0.34) for lead conversion by
   plotting confusion matrix for different probability cut-offs.

8) Re-evaluation: We re-evaluated the model using the selected cut-off point and found
   an accuracy of 90.6%, precision of 86.4%, and recall of 90%.

9) Model testing: We scaled the test data and performed prediction of lead conversion.
   We evaluated the prediction on test data by accuracy, specificity and sensitivity
   matrix, and we found accuracy of 91.1%, precision of 85.6% and recall of 91.9%.

10) Lead Score Calculation: We created lead conversion score = (conversion probability * 100) to give a score between 0 to 100 where higher the value means the lead is     “hot” and there is high possibility that the lead can be converted

## Details of files given
1) Assignment Subjective Questions_Answer.pdf : Some subjective questions answered
2) Lead_Score_Case_Study_Final.ipynb : The python file showing coding and data analysis
3) Lead_Score_Case_Study_ppt.pdf : Final Presentation
4) Summary_report_Lead_Score_Case_Study.pdf : Summary on what's done in the entire py file
