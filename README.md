# Credit_Risk_Analysis
## Overview of the analysis:
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Apply machine learning to assess credit card risk. Then, evaluate the performance of these machine learning models and make a written recommendation on whether they should be used to predict credit risk.

## Resources: Jupyter Notebook, LoanStats_2019Q1.csv

## Results: 
#### Naive Random Oversampling
<img width="924" alt="naive random oversamp" src="https://user-images.githubusercontent.com/72039212/115650853-a855a280-a2ef-11eb-9a4b-d7b96f5e2519.png">

- Balanced Accuracy Score
  - 0.640324421824783 = 64%
- Precision
  - .99 = 99%
- Recall
  - .62 = 62%

#### SMOTE
<img width="919" alt="Smote" src="https://user-images.githubusercontent.com/72039212/115650962-e226a900-a2ef-11eb-927d-1416026aac15.png">

- Balanced Accuracy Score
  - 0.6514992150524688 = 65%
- Precision
  - .99 = 99%
- Recall
  - .69 = 69%

#### Undersampling
<img width="915" alt="Undersampling" src="https://user-images.githubusercontent.com/72039212/115650973-e5219980-a2ef-11eb-95b1-52c07a16ece8.png">

- Balanced Accuracy Score
  - 0.6514992150524688 = 65%
- Precision
  - .99 = 99%
- Recall
  - .40 = 40%

#### Combination/Over and Undersampling with SMOTEENN
<img width="916" alt="Combo SMOTEENN" src="https://user-images.githubusercontent.com/72039212/115650887-b86d8200-a2ef-11eb-8545-beec5ece8b3d.png">

- Balanced Accuracy Score
  - 0.5447046721744204 = 54%
- Precision
  - .99 = 99%
- Recall
  - .57 = 57%

#### Balanced Random Forest Classifier
<img width="936" alt="balanced rando forest" src="https://user-images.githubusercontent.com/72039212/115650900-bd323600-a2ef-11eb-9ddb-d057661010a2.png">

- Balanced Accuracy Score
  - 0.7734804087284313 = 77%
- Precision
  - .99 = 99%
- Recall
  - .88 = 88%

#### Easy Ensemble AdaBoost Classifier
<img width="897" alt="adaboost" src="https://user-images.githubusercontent.com/72039212/115650958-dfc44f00-a2ef-11eb-8017-2e4d07d8e44a.png">

- Balanced Accuracy Score 
  - 0.9316600714093861 = 93%   
- Precision
  - .99 = 99%
- Recall
  - .94 = 94%

## Summary: 
Oversampling, undersamping, and a combination of both yielded sub par results in comparison to both resampling machine learning models. The Easy Ensemble AdaBoost machine learning model is the clear front runner with the highest overall balanced accuracy score, 93%, and precision and recall scores with little variation, 99% and 94% respectively. The Balanced Random Forest machine learned model follows the Easy Ensemble AdaBoost machine learning model with the second highest accuracy score and little variation between precison and recall. All four of the oversampling, undersampling and combination of over and undersamping models showed high variation between precision and recall and accuracy scores less than 70%. The only recommended models are the Easy Ensemble AdaBoost and the Balanced Random Forest machine learning models.
