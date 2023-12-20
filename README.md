# Identifying-Age-Related-Conditions

About this Notebook

The "ICR: Identify Age-Related Conditions” task challenges participants to develop predictive models that can accurately identify age-related conditions in individuals. With access to a provided dataset containing demographic and medical information, participants create machine learning models to predict the presence or likelihood of age-related conditions. 

Summary

The distribution of the target feature is analyzed to assess the imbalance between the values 1 and 0, which helps determine if oversampling is necessary.
   
An analysis of missing values is conducted to check for presence of missing values, which will impact machine learning at later process.
   
Histograms and box plots are employed to visualize the skewness and identify outliers, aiding in the selection of appropriate methods for data standardization.
   
For data processing, the Robust Scaler is chosen to standardize the numerical features, taking into account outlier handling. Additionally, the CatBoost Encoder is utilized for encoding categorical features, and the kNN Imputer is employed for handling missing values.

In order to address the class imbalance, the SMOTE (Synthetic Minority Over-sampling Technique) is employed for oversampling the minority class, generating synthetic samples to balance the dataset.

SelectKBest feature selection method is used to select those features with low p-value with the taget label.   

Lastly, various base classifiers with hyperparameter tuning are applied.

