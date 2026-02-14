# Fraud Detection -- Machine Learning Project

**Author:** Ajay

------------------------------------------------------------------------

## 📌 Problem Statement

Develop a fraud detection model for financial transactions and provide
actionable business insights.

-   Dataset size: 6.3M transactions\
-   Fraud rate: \~0.13% (Highly Imbalanced)

------------------------------------------------------------------------

## 📂 Data Source
 Link: (https://www.google.com/url?sa=D&q=https://drive.google.com/uc%3Fexport%3Ddownload%26confirm%3D6gh6%26id%3D1VNpyNkGxHdskfdTNRSjjyNa5qC9u0JyV&ust=1771163160000000&usg=AOvVaw1dSKqFQf9m3mKm9_pVS05Z&hl=en-GB)

------------------------------------------------------------------------

## 📊 Data Cleaning

-   No missing values\
-   No duplicate rows\
-   Handled merchant structural imbalance\
-   Created features:
    -   `isMerchant`
    -   `error_balance_dest_clean`
    -   `error_balance_orig`
-   Dropped ID columns:
    -   `nameOrig`
    -   `nameDest`
-   Removed multicollinearity by dropping derived balance columns

------------------------------------------------------------------------

## 🤖 Models Tested

1.  Logistic Regression\
2.  Random Forest

### Final Selected Model: Random Forest

Reason: - High Precision\
- Good Recall\
- Operationally feasible

------------------------------------------------------------------------

## 📈 Model Performance (Test Set)

-   Precision (Fraud): 0.98\
-   Recall (Fraud): 0.75\
-   ROC-AUC: 0.98

Confusion Matrix: - True Fraud: 97\
- Missed Fraud: 32\
- False Positives: 2

------------------------------------------------------------------------

## 🔍 Key Fraud Predictors

-   Transaction Amount\
-   Destination Balance Error\
-   Origin Balance\
-   Transfer Type\
-   Cash-Out Type\
-   Time (step)

------------------------------------------------------------------------

## 🛡 Business Recommendations

-   Real-time monitoring of high-value transfers\
-   Flag abnormal balance inconsistencies\
-   Multi-factor authentication for large transactions\
-   Automated account freeze for suspicious behavior

------------------------------------------------------------------------

## 📦 Tech Stack

-   Python\
-   Pandas\
-   NumPy\
-   Scikit-learn\
-   Random Forest

------------------------------------------------------------------------

## 🚀 Conclusion

Random Forest model provides strong fraud detection with high precision
and good recall.\
Model aligns with real fraud behavior and is production-feasible.
