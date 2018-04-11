# This is a machine learning project of kaggle competiton “TalkingData Mobile User Demographics” <br>
https://www.kaggle.com/c/talkingdata-mobile-user-demographics

TalkingData is China’s largest third-party mobile data platform.
They provides **user's phone brand, phone model, app id, app label (type), app trigger time and geolocation data**, and aim to build a model to understand users’ age and gender.

The target group are **'F23-', 'F24-26', 'F27-28', 'F29-32', 'F33-42', 'F43+', 'M22-', 'M23-26', 'M27-28', 'M29-31','M32-38', and 'M39+'**

Identifying the demographic characteristics can help developers and brand advertisers better understand user behavior and build up user portrait.

## Project Overview
#### EDA
First, some basic exploratory analysis is conducted to understand the business.
Different age group and gender do have different preference on phone brand, phone model, APP's type, and usage time.

#### Modeling
Logistic regression, XGBoost, and random forest are built to predict the category. For each model, first, used grid search to find the optimized hyper parameters. Then, used cross validation to calculate log loss. Last, compaired the model performance and selected the best model based on log loss.

#### Model Visualization and Result
A graph is generated to explian what are the top variables that influence the result of each group. For example, a female younger than 23 will be moer likely to use Vivo or OPPO, or a APP under label "foreign language", and is less likely to use huawei, MI, and samsung.
