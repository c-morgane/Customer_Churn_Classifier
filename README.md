# CUSTOMER CHURN CLASSIFIER

---

![](https://images.unsplash.com/photo-1521791136064-7986c2920216?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80)

Photo by [Cytonn Photography](https://unsplash.com/@cytonn_photography)

# Context 

The project is about a telecom company 🛰 : they want to **predict if a customer is about to leave**. I will combine both unsupervised and supervised approaches in order to build a **customer churn classifier**.

# Content

The dataset contains about **7000 customers** with **19 features**.

**Features** :
- `customerID`: a unique ID for each customer
- `gender`: the gender of the customer
- `SeniorCitizen`: whether the customer is a senior (i.e. older than 65) or not
- `Partner`: whether the customer has a partner or not
- `Dependents`: whether the customer has people to take care of or not
- `tenure`: the number of months the customer has stayed
- `PhoneService`: whether the customer has a phone service or not
- `MultipleLines`: whether the customer has multiple telephonic lines or not
- `InternetService`: the kind of internet services the customer has (DSL, Fiber optic, no)
- `OnlineSecurity`: what online security the customer has (Yes, No, No internet service)
- `OnlineBackup`: whether the customer has online backup file system (Yes, No, No internet service)
- `DeviceProtection`: Whether the customer has device protection or not (Yes, No, No internet service)
- `TechSupport`: whether the customer has tech support or not (Yes, No, No internet service)
- `StreamingTV`: whether the customer has a streaming TV device (e.g. a TV box) or not (Yes, No, No internet service)
- `StreamingMovies`: whether the customer uses streaming movies (e.g. VOD) or not (Yes, No, No internet service)
- `Contract`: the contract term of the customer (Month-to-month, One year, Two year)
- `PaperlessBilling`: Whether the customer has electronic billing or not (Yes, No)
- `PaymentMethod`: payment method of the customer (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))
- `MonthlyCharges`: the amount charged to the customer monthly
- `TotalCharges`: the total amount the customer paid

**Target** :
- `Churn`: whether the customer left or not (Yes, No)

Many features are **categorical** data with more than 2 values => need to handle it.

# Sections

1. **EDA and Data preparation** (loading and cleaning, dummies, scalling, concatenation)
2. **Feature engineering** (PCA, split)
3. **Market segmentation** : different clusterings models are used to determine meaningful clusters of customers and I try to label them according to their main characteristics.(Logistic regression, SVM, Random Forest, Gradient Boosting, xGB/ Hyperparameter optimization/ SMOTE)
4. **Churn prediction** : the best prediction model according to the F1-score.