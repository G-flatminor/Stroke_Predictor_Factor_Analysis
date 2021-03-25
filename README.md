# ANALYSIS OF STROKE PREDICTING FACTORS
Analyze determining factors which increase risk of stroke

## DATA

Data downloaded from  https://www.kaggle.com/fedesoriano/stroke-prediction-dataset

+ ID
+ Gender (male or female)
+ Age
+ Hypertension (yes or no)
+ Heart disease (yes or no)
+ Ever married (true or false)
+ Work type (private, self-employed, other)
+ Residence type (rural or urban)
+ Average glucose level
+ BMI
+ Stroke (yes or no)

## Analysis_Sample
+ Male    2994  (59.60 %, 0-82 yrs old)
+ Female  2115  (41.40 %, 0-82 yrs old)
+ Unknown 1

### Age distribution
![age_distribution](https://user-images.githubusercontent.com/46631208/111081669-cfdc7280-84da-11eb-81d3-3dae1dec07d3.png)


## Categorical variable responses

| Item | Answer | Response | Ratio |
| ---- | ------ | -------- | ----- |
| Hypertension | Yes | 498 | 9.75% |
|   | No | 4612 | 90.25% |
| Heart disease | Yes | 276 | 5.40% |
|   | No | 4834 | 94.60% |
| Ever married | Yes | 3353 | 65.62% |
|   | No | 1157 | 34.38% |
| Residence type | Rural | 2514 | 49.20% |
|  | Urban | 2596 | 50.80% |
| Stroke | Yes | 249 | 4.87% |
|  | No | 4861 | 95.13% |

## Categorical variable responses (details)

### Hypertension:
+ Chances of hyptertension are increasing over age groups for both male and female (except for male at 81-90)
+ In each group, the ratio seems different between male and female

![hypertension](https://user-images.githubusercontent.com/46631208/111082236-90635580-84dd-11eb-9510-5a259a18d095.png)

### Heart disease:
+ Chances of heart disease start increasing from 40s and keep increasing for both gender
+ Male ratio is higher in all age groups

![heart_disease](https://user-images.githubusercontent.com/46631208/111082275-c7d20200-84dd-11eb-97cd-ea4a453111d0.png)

### Stroke:
+ Chances of stroke start increasing from 40s and keeps increasing
+ Male chance is higher for all age groups but 30s

![stroke](https://user-images.githubusercontent.com/46631208/111082340-1d0e1380-84de-11eb-8dc0-3bf27010cf46.png)

## Numerical variables summary by age and gender

### BMI
+ the age group transitions seem similar between male and female
+ BMI average for both gender increases towards 30/40s
+ It declines from 60s
+ Average BMI in each age group is not much different between male and female

![BMI](https://user-images.githubusercontent.com/46631208/111082462-ce14ae00-84de-11eb-9a24-fe8113d188ab.png)


### Glucose level
+ Both male and female constantly increases the glucose level from 0-10 years of age to 81-90 years of age
+ In each age group, male average is higher than female average

![glucose_level](https://user-images.githubusercontent.com/46631208/111082503-103def80-84df-11eb-897e-b925c11a58b7.png)

## ANALYSIS

## Distribution pairplot
+The figures show they potentially influence the stroke probability 

![pairplot](https://user-images.githubusercontent.com/46631208/112248535-7687e800-8c2c-11eb-96eb-ac4daea18456.png)

## Correlations
+ Correlation heatmap is shown below
+ Age seems highly correlated with stroke

![correlation_heatmap](https://user-images.githubusercontent.com/46631208/112248033-a4206180-8c2b-11eb-9b27-169277efc422.PNG)

## Causal relationship: Determinination of stroke predictors
+ Conducted Logistic Regression Analysis

[output]
LogisticRegression(C=1.0, class_weight=None, dual=False, fit_intercept=True,
                   intercept_scaling=1, l1_ratio=None, max_iter=100,
                   multi_class='auto', n_jobs=None, penalty='l2',
                   random_state=None, solver='lbfgs', tol=0.0001, verbose=0,
                   warm_start=False)














