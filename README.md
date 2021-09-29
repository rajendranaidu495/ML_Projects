# PROJECTS

1. [Healthcare provider Fraud Detection](https://github.com/rajendranaidu495/ML_Projects/tree/main/HealthCare_Provider_Fraud_Detection)
2. [Heart Disease Detection](https://github.com/rajendranaidu495/ML_Projects/tree/main/Heart_Disease_Detection)
3. [Robust Sentiment Analysis on Twitter feeds](https://github.com/rajendranaidu495/ML_Projects/tree/main/Robust_Sentiment_Analysis)

## 1. Healthcare provider Fraud Detection

#### Problem Statement
The goal of this project is to " predict the potentially fraudulent providers " based on the claims filed by them.along with this, we will also discover important variables helpful in detecting the behaviour of potentially fraud providers. further, we will study fraudulent patterns in the provider's claims to understand the future behaviour of providers.

#### Introduction to the Dataset
For the purpose of this project, we are considering Inpatient claims, Outpatient claims and Beneficiary details of each provider. Lets s see their details :

#### A) Inpatient Data

This data provides insights about the claims filed for those patients who are admitted in the hospitals. It also provides additional details like their admission and discharge dates and admit d diagnosis code.

#### B) Outpatient Data

This data provides details about the claims filed for those patients who visit hospitals and not admitted in it.

#### C) Beneficiary Details Data

This data contains beneficiary KYC details like health conditions,regioregion they belong to etc.

### Data Analysis:
Understand the features in all 4 datasets and identify the missing values. derived new features like age and AdmitForDays to fill the missing values based on scenario.

Merged all sub datasets into one big Datasets to perform the Exploratory Data Analysis. 
Used Matplotlib and seaborn to plot graphs based on potential fraud class vs non fradulent class where the proportion of fradulent claim transactions are more compared to non fraud providers.
So i have deep drive into all other features such as number of claim transactions and amounts involved per - Beneficiary | Beneficiary + Physician |Physician | Diagnosis | Procedure etc
PLot the frequencies of Statewise beneficiaries and race-wise beneficiaries where more than 80% beneficiaries are of same race which is Race 1 which means Maximum population in the dataset originated from same race. 
plot the Top-10 Procedures invloved in Healthcare Fraud and Top-20 Attending Physicians invloved in Healthcare Fraud. 
we see that occurance of fraud cases is more frequent in lower age groups(30-70 years) compared to higher age groups(70+ years).Age is one of the important feature for differentiating between fraud abd non fraud behaviour.

Create new features from combining the exsiting feature.
Used simple method that is 'Grouping based on Similarity'. In this method, I basically group all the records by the ProcedureCodes, DiagnosisCodes,Provider.
take the Average Features based on grouping variables such as Average features grouped by Provider, Average Feature based on grouping based on combinations of different variables, etc.

Create dummies to convert categorrical features into numeric. 
Applied StandardScaler to transform values from its z form to mean 0 and scales the data to unit variance.  

Since data is unblanced, i have split the train and test data using stratify method. 

### Models:
Appiled multiple machine learning Models which are LogisticRegression, Support vector machine, Adaboosting, Decision tree, 
GradientBoosting, xGBoosting, Random Forest.

### Model Evalution 
Precision, recall, f1- scores, ROC.

### Feature Importance 
Studied behaviour of Providers and found following important features impactful in predicting Fraud/NonFraud are folowing:

1) PerProviderAvg_InscClaimAmtReimbursed( Importance: 8%)
2) InscClaimAmtReimbursed (Importance: 7%)
3) PerAttendingPhysicianAvg_InscClaimAmtReimbursed (Importance: 7%)
4) PerOperatingPhysicianAvg_InscClaimAmtReimbursed (Importance: 6%)
5) PerClmAdmitDiagnosisCodeAvg_InscClaimAmtReimbursed (Importance: 4%)

### Conclusion: 
Logistic regression model is performing better compared to other models. LR model consistentently performed with ~0.90 Accuracy, ~0.80 AUROC score.

## 2. Heart Disease Detection

[Heart Disease Detection](https://github.com/rajendranaidu495/ML_Projects/tree/main/Heart_Disease_Detection)

## 3. Robust Sentiment Analysis on Twitter feeds 
[Robust Sentiment Analysis on Twitter feeds](https://github.com/rajendranaidu495/ML_Projects/tree/main/Robust_Sentiment_Analysis)

## Author

- [@RajendraMannam](https://github.com/rajendranaidu495)

  