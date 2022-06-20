# Credit Risk Analysis
## Overview
In this project, lending data was used to create machine learning models to determine loan approval based on credit risk features. Modeling techniques of, Random Oversampling, SMOTE, Cluster Centroids, SMOTEENN, Balanced Random Forest Classifier, and Easy Ensemble Classifier were used to combat the class imbalance of good credit application vs bad credit applications. These techniques were evaluated and assesed based on accuracy, precision, senstivity, F1 score. 

### Purpose
The purpose of this repository was to evaluate different techniques to combat class imbalance in Machine Learning models. 

### Resources
**Data resource:** [Loan Stats](/Module-17-Challenge-Resources/LoanStats_2019Q1.csv)
**Tools:** Python, PANDAS, Matplotlib, SciKit-Learn, Imbalanced-Learn
**ML Sampling Techniques:** Random Oversampling, SMOTE, Cluster Centroids, SMOTEENN
**ML Model:** Logistic Regression, Balanced Random Forest Classifier, and Easy Ensemble Classifier
<br>

## Results
### Sampling Techniques
As shown in [Credit Resample File](/Module-17-Challenge-Resources/credit_risk_resampling.ipynb), Random Oversampling, SMOTE, Cluster Centroids, and SMOTEEN techniques were used in efforts to increase performance of ML model in classic class imbalance of determining credit risk applicants. Below are the classification reports detailed from each technique.

<br>**Image 1. Random Oversampling Classification Report**
<br>![CR_ROS](/img/cr_ros.png)
<br>Image 1. Classifcation report shows precision of 1% of determining high-risk applicants and 66% sensitivity detection.
<br>
<br>**Image 2. SMOTE Classification Report**
<br>![CR_ROS](/img/cr_smote.png)
<br>Image 2. Classifcation report shows precision of 1% of determining high-risk applicants and 61% sensitivity detection.
<br>
<br>**Image 3. Cluster Centroids Classification Report**
<br>![CR_ROS](/img/cr_ccus.png)
<br>Image 3. Classifcation report shows precision of 1% of determining high-risk applicants and 69% sensitivity detection.
<br>
<br>**Image 4. SMOTEENN Classification Report**
<br>![CR_ROS](/img/cr_se.png)
<br>Image 4. Classifcation report shows precision of 1% of determining high-risk applicants and 75% sensitivity detection.
<br>
<br>Sampling Techniques Overview:
 - All sampling techniques resulted in 1% precision of determing high-risk applicants 
 - Oversampling techniques ROS and SMOTE are relatively consistent to each other.
    - ROS shows 66% sensitivity with an index balanced accuracy score of 41% for high-risk applicants.
    - SMOTE shows 61% sensitivity with an index balanced accuracy score of 42% for high-risk applicants.
 - Undersampling techniques, cluster centroid, showed elevated sensitivity of 69% for high-risk applicant detection but extremely lowered sensitivity for low-risk applicants of 40% (compared to ~60%). The index balanced accuracy is also decreased compared to others scoring 27% average.
 - SMOTEEN, combination technique, showed the highest sensitivite to high-risk applicants of 75%, while maintaining base sensitivity to low-risk applicants at 56%.
  
### Ensemble Techniques
As shown in [Credit Ensemble File](/Module-17-Challenge-Resources/credit_risk_ensemble.ipynb), BalancedRandomForest(BRF) and Easy Ensemble Classifier(EEC)techniques were used to strengthen performance of ML model through ensemble decision tree. Below are the classification reports detailed from each technique.

<br>**Image 5. Balanced Random Forest Classification Report**
<br>![CR_ROS](/img/cr_brf.png)
<br>Image 5. Classifcation report shows precision of 3% of determining high-risk applicants and 70% sensitivity detection.
<br>
<br>**Image 6. Easy Ensemble AdaBoost Classifier Classification Report**
<br>![CR_ROS](/img/cr_eec.png)
<br>Image 6. Classifcation report shows precision of 9% of determining high-risk applicants and 92% sensitivity detection.

<br>Ensemble Techniques Overview:
 - Ensemble techniques showed increased performance for precision, sensitivity, F1 score, and index balanced accuracy compared to all sampling techniques.  
 - BRF resulted in 3% precision, 70% sensitivity, and 60% index balanced accuracy in detemining high-risk applicants. 
 - EEC resulted in 9% precision, 92% sensitivity, and 87% index balanced accuracy in detemining high-risk applicants. 

## Summary
<<<<<<< HEAD
In summary, the Ensemble Techniques performed better than all the sampling techniques. The EEC model outperformed BRF model with increased precision, sensitivity, and accuracy. Although, a precision of 9% is very low in determining results, the sensitvity score of 94% with the maintained precision and sensitivities of low-risk applicant determination, make this model a good contender to be used at assessing loan applications. 
=======
In summary, the Ensemble Techniques performed better than all the sampling techniques. The EEC model outperformed BRF model with increased precision, sensitivity, and accuracy. Although, a precision of 9% is very low in determining results, the sensitvity score of 94% with the maintained precision and sensitivities of low-risk applicant determination, make this model a good contender to be used at assessing loan applications. 
>>>>>>> 6dcd2e343992d4025815a3de0a8219125fbcca37
