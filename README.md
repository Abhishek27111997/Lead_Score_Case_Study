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

##Steps Followed
Data loading and preparation: We loaded the data into a Jupyter notebook and
performed missing value and outlier treatment for all columns. We also dropped
columns that had more than 45% missing values.

Exploratory Data Analysis (EDA): We conducted EDA on each categorical column to
visualize data imbalance and dropped high data imbalanced columns.

Train-test split and feature scaling: We performed train-test split using the sklearn
library and scaled the train data using Standard Scaler.

Feature selection: We used Recursive Feature Elimination (RFE) to select 20 features
for the model.

Logistic Regression: We used the statsmodels GLM method to perform Logistic
Regression on the selected features and checked coefficients, p-values, and Variance
Inflation Factor (VIF).

Model evaluation: We evaluated the model using accuracy, specificity, and sensitivity.
We also plotted the Receiver Operating Characteristic (ROC) curve to check the
balance between True Positive Rate (TPR) and False Positive Rate (FPR).

Cut-off selection: We selected the optimal cut-off point (0.34) for lead conversion by
plotting confusion matrix for different probability cut-offs.

Re-evaluation: We re-evaluated the model using the selected cut-off point and found
an accuracy of 90.6%, precision of 86.4%, and recall of 90%.

Model testing: We scaled the test data and performed prediction of lead conversion.
We evaluated the prediction on test data by accuracy, specificity and sensitivity
matrix, and we found accuracy -91.1%, precision – 85.6% and recall – 91.9%.

Lead Score Calculation: We created lead conversion score = (conversion probability * 100) to give a score between 0 to 100 where higher the value means the lead is “hot” and there is high possibility that the lead can be converted

## Details of files given
Lead Score Case Study Final .ipynb : The python file showing coding and data analysis
Assignment Subjective Questions Answer.pdf : Some subjective questions answered
Lead Score Case Study.pdf : Final Presentation
Leads.csv : Data worked on
Leads Data Dictionary.xlsx : Data Dictionary
Summary.pdf : Summary on what's done in the entire py file
